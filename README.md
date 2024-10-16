Djagora Network Security System
Project Overview
This project aims to implement a robust network security system for the Djagora company. The project was part of our final year study in Computer Systems Engineering at the Faculty of Sciences of Sfax. The goal was to secure the company’s network infrastructure while allowing authorized remote access using open-source solutions.

Features
Virtual Private Network (VPN): Secure remote access using OpenVPN.
Firewall Configuration: Implemented a firewall using PFsense to monitor and control network traffic.
Proxy Server: Set up a proxy server for enhanced security and control over internet usage.
FTP Server: Installed and configured an FTP server for secure file transfer.
Technologies Used
PFsense: Open-source firewall and router software.
OpenVPN: For secure remote access.
Linux (Debian, Ubuntu): Operating system used for server installations.
Squid Proxy: Web proxy for controlling internet access.
FTP (vsftpd): For file transfer needs.
Installation Guide
Prerequisites
Linux Server: Ensure you have a Linux-based system (Debian or Ubuntu preferred) for the installations.
Internet Access: For downloading necessary software packages and updates.
Basic Network Infrastructure: Network switches, routers, and client machines.
Installation Steps
1. Install OpenVPN
Update the server:
bash
Copy code
sudo apt-get update && sudo apt-get upgrade
Download and install OpenVPN:
bash
Copy code
wget https://raw.githubusercontent.com/angristan/openvpn-install/master/openvpn-install.sh
chmod +x openvpn-install.sh
./openvpn-install.sh
2. Install PFsense
Download and install PFsense as a firewall.
Access PFsense through its web interface (https://192.168.1.1), and configure rules for VPN and other network traffic.
3. Install Squid Proxy Server
Install Squid:
bash
Copy code
sudo apt-get install squid
Configure Squid via its configuration file:
bash
Copy code
nano /etc/squid/squid.conf
4. Install and Configure FTP Server (vsftpd)
Install vsftpd:
bash
Copy code
sudo apt-get install vsftpd
Configure vsftpd:
bash
Copy code
nano /etc/vsftpd.conf
Usage
Remote Access: Authorized users can connect to the company’s network using the VPN for secure and encrypted communication.
Firewall: PFsense monitors and filters incoming and outgoing traffic to protect the network from unauthorized access.
Proxy Server: Controls internet access and monitors user activities.
FTP Server: Provides a secure method for file transfers between remote users and the company.
Future Improvements
Implement intrusion detection and prevention systems (IDS/IPS).
Expand the VPN service to handle more clients simultaneously.
Contributors
Ahmed Habaib
Islem Khlifi
License
This project is licensed under the MIT License.