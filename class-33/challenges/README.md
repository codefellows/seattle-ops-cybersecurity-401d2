# Ops Challenge: Signature-based Malware Detection Part 3 of 3

## Overview

Detection and remediation of malware is the core function of many security products, and an optional secondary feature on others like perimeter firewalls and proxy servers.

VirusTotal is a respected vendor-neutral database of malware signatures. Today you will finish development of your own basic antivirus tool in Python by incorporating VirusTotal.

## Staging

- Copy and paste the demo script into a new Python file on your system.
- Download [virustotal-search.py](https://github.com/eduardxyz/virustotal-search) and place it in the same folder as the demo Python script.
- Sign up for an account at virustotal.com to get a free API key.
- To query the Virustotal API, you'll need to set your API key as an environment variable to avoid hard-coding it into your demo Python script, which is currently set to call "API_KEY_VIRUSTOTAL" in place of your literal API key. You can always hard-code it at first for testing, but don't leave it that way!
- Set the variable `hash` to whatever MD5 hash you wish to VirusTotal to evaluate.

> Note that this is one of many ways to interact with the VirusTotal API. If you are an advanced coder, try further optimizing your API query process.

## Demonstration

Ref. [DEMO.md](DEMO.md)

## Resources

- [Getting Started with Virustotal API](https://developers.virustotal.com/reference#file-scan){:target="_blank"}
- [VirusTotal API – Getting started with security automation](https://www.tines.io/blog/virustotal-api-security-automation){:target="_blank"}
- [Video - Python: VirusTotal Lookup Script](Python: Virus Total Lookup Script)
- [Virustotal Search GitHub Repo](https://github.com/eduardxyz/virustotal-search)
