# building-firewall-using-python
cyber security internship at elevate labs

A firewall is buliding using with python. This project implements a Python-based custom firewall designed for individual users and developers who want deeper visibility and control over the network packets traversing their system.

Unlike traditional firewalls, this tool gives real-time packet analysis, rule-based filtering, and a user-friendly graphical interface to add, remove, or manage firewall rules without diving deep into terminal commands or system configurations.

## Module Descriptions
### firewall.py
The core of the firewall. It uses Scapy to sniff network packets in real time and checks them against rules from walls.json. Based on the match, it allows or blocks packets and logs the activity.
### logger.py
Handles all logging functionality. Every packet decision (ALLOW or BLOCK) is logged in logs.txt with timestamp and details.
### iptables.py
Provides optional integration with Linux's iptables to block or allow traffic at the system level.
### Tkinter.py
A Tkinter-based GUI interface that lets you:
- Add or remove firewall rules
- View existing rules
- Control the firewall visually
### Walls.json
Contains all firewall rules in JSON format. These rules define which packets to allow or block.

## Requirements
- Python
- Scapy - For packet sniffing
- Tkinter -GUI
- JSON - Rule storage
- iptables - System level packet filtering

## Start
    python3 firewall.py

After installing the all requirements.Then we can start our project.
