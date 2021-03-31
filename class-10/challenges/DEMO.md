# Demo: Ops Challenge 10

- Be sure to demonstrate for students [How to Install Zenmap to Kali Linux](https://www.youtube.com/watch?v=UoIfI1Pn1nk&ab_channel=TheLinuxOS) since we're having them load it on Kali.
  - First download zenmap at [Optional Zenmap GUI (all platforms): zenmap-7.80-1.noarch.rpm](https://nmap.org/download.html)
  - Should be in your downloads folder.
  - Then run these commands:
    - apt-get update
    - apt-get install alien
  - Go to your downloads folder cd Downloads
    - sudo alien "name of downloaded package.rpm"
    - sudo dpkg -i "name of converted package.deb"
    - zenmap

- Give students a quick tour of both Zenmap and the regular console-based Nmap. Explain how they compare/contrast.
