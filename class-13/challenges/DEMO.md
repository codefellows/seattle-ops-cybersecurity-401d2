# Demo: Ops Challenge Class 13

## Resource

- [Infosec](https://resources.infosecinstitute.com/topic/port-scanning-using-scapy/)

## Sample Code

Part 1 of 3: 

```python
#! /usr/bin/env python3

import random
from scapy.all import ICMP, IP, sr1, TCP

# Define end host and TCP port range
host = "192.168.40.1"
port_range = [22, 23, 80, 443, 3389]

# Send SYN with random Src Port for each Dst port
for dst_port in port_range:
    src_port = random.randint(1025,65534)
    resp = sr1(
        IP(dst=host)/TCP(sport=src_port,dport=dst_port,flags="S"),timeout=1,
        verbose=0,
    )

    if resp is None:
        print(f"{host}:{dst_port} is filtered (silently dropped).")

    elif(resp.haslayer(TCP)):
        if(resp.getlayer(TCP).flags == 0x12):
            # Send a gratuitous RST to close the connection
            send_rst = sr(
                IP(dst=host)/TCP(sport=src_port,dport=dst_port,flags='R'),
                timeout=1,
                verbose=0,
            )
            print(f"{host}:{dst_port} is open.")

        elif (resp.getlayer(TCP).flags == 0x14):
            print(f"{host}:{dst_port} is closed.")

    elif(resp.haslayer(ICMP)):
        if(
            int(resp.getlayer(ICMP).type) == 3 and
            int(resp.getlayer(ICMP).code) in [1,2,3,9,10,13]
        ):
            print(f"{host}:{dst_port} is filtered (silently dropped).")
```

Part 2 of 3:

```python
#!/usr/bin/env python3

# Purpose: Scapy scanning tool (2 of 3)

# Import libraries
import random
import ipaddress
from scapy.all import ICMP, IP, sr1, TCP, sr

# Declare variables

# Declare functions

# TCP Port Range Scanner
def tcp_port_scan():
    host = "scanme.nmap.org" # definining host IP
    port_range = [22, 23, 80, 443, 3389] # providing a port range

    for dst_port in port_range: # for each port in defined range...
        src_port = random.randint(1025,65534) # randomize TCP source port
        port_num = str(dst_port)
        response = sr1(IP(dst=host)/TCP(sport=src_port,dport=dst_port,flags="S"),timeout=1,verbose=0)
        if response is None:
            print ("\nPort " + port_num + ": The packet was filtered.")
            print (response)
        elif response.haslayer(TCP):
            if response.getlayer(TCP).flags == 0x12: #Port responding and open
                print("\nPort " + port_num + ": The port is OPEN and responding.")
                # send RST packet to graciously close connection
                send_rst = sr(IP(dst=host)/TCP(sport=src_port,dport=dst_port,flags="R"),timeout=10)
                print(response)
            if response.getlayer(TCP).flags == 0x14: #Port closed
                print("\nPort " + port_num + ": The port is CLOSED.")
                print(response)


# ICMP Ping Sweep Tool
def ping_sweep():
    network = "10.0.0.0/24"
    ip_list = ipaddress.ip_network(network)
    hosts_scanned = 0
    hosts_count = 0
    hosts_block = 0

    for host in ip_list.hosts(): # .hosts() suppresses network and broadcast addresses
        print("Pinging",host,", please wait...")
        response = sr1(
            IP(dst=str(host))/ICMP(),
            timeout=1,
            verbose=0
        )
        #print(response)

        if response is None:
            print (f"{host} is down/unresponsive")
            hosts_scanned+=1
        elif response.haslayer(ICMP):
            hosts_scanned+=1
            hosts_count+=1
            if (int(response.getlayer(ICMP).type) == 3 and
                int(response.getlayer(ICMP).code) [1,2,3,9,10,13]):
                hosts_block+=1
                print (f"{host} is currently blocking ICMP traffic")
            else:
                print(f"{host} is up. Total hosts online: {hosts_count}")
    
    # print total hosts online
    print (f"""
    {hosts_scanned} ip addresses scanned. 
    {hosts_count} hosts are up; 
    {hosts_block} are blocking ICMP traffic.
    """) 

# Main

if __name__ == "__main__": # when my computer runs this file...do this stuff
    while True:
        mode = input("""
        Network scanning tool: what would you like to do?
        1 - TCP Port Range Scanner
        2 - ICMP Ping Sweep
        3 - Exit
        Please enter a number: 
        """)

        if (mode == "1"):
            tcp_port_scan()
        elif (mode == "2"):
            ping_sweep()
        elif (mode == '3'):
            break
        else:
            print("Invalid selection...")    



#resource: https://docs.python.org/3.4/howto/ipaddress.html
#resource: https://thepacketgeek.com/scapy/building-network-tools/part-10/

# End
```
