# Security System Implementation 

This project is the result of a final year thesis aimed at setting up a security system for a company. It integrates various open-source solutions to enhance network security and system administration, focusing on virtualization, VPN setup, firewall configurations, and proxy servers.

**[Click here to view the full PDF of the project.](https://raw.githubusercontent.com/Ahmedhabaib/Setting-up-a-security-system/a7b254fac92aa9014936991c06e4a02143b3c5ac/Mise%20en%20place%20d%E2%80%99un%20syst%C3%A9me%20de%20s%C3%A9curit%C3%A9.pdf)**

## Project Overview

The main objectives of this project were:
1. **Virtualization**: Implementing a virtualized environment using Proxmox VE for flexible and cost-effective system management.
2. **VPN Setup**: Securing remote access via OpenVPN, ensuring secure communication between remote and internal systems.
3. **Firewall**: Configuring and deploying pfSense to monitor and control network traffic with robust filtering rules.
4. **Proxy Server**: Installing and configuring Squid proxy for improved network traffic management and user authentication.

### Key Features
- **Proxmox VE**: Provides a virtualization environment to host different servers in an efficient and isolated manner.
- **OpenVPN**: Ensures encrypted communication for remote connections to the internal network.
- **pfSense Firewall**: Provides network security through stateful packet inspection and traffic filtering.
- **Squid Proxy**: Enables network traffic filtering and user authentication for enhanced security and management.

## Tools and Technologies
- **Proxmox VE**: Virtualization platform.
- **OpenVPN**: Virtual Private Network (VPN) solution.
- **pfSense**: Firewall and router solution.
- **Squid**: Proxy server for web traffic filtering.
- **Linux Distributions**: Debian and Ubuntu used for hosting services.

## System Components
- **VPN Server**: Provides secure remote access.
- **FTP Server**: For file transfers, essential for VPN client setup.
- **Firewall Rules**: Configured using pfSense to filter and protect network traffic.
- **Proxy Server**: Configured using Squid for caching and filtering HTTP requests.

## Installation and Setup
The installation and configuration process involves several steps for each component:

1. **Proxmox VE Installation**:
   - Download and install the Proxmox VE distribution.
   - Configure virtual machines for different services.

2. **OpenVPN Installation**:
   - Install OpenVPN on a Debian-based VM.
   - Configure VPN access, assign IP addresses, and set up encryption.

3. **pfSense Firewall**:
   - Install pfSense on a virtual machine.
   - Configure WAN and LAN interfaces, filtering rules, and VPN pass-through.

4. **Squid Proxy Setup**:
   - Install Squid on Ubuntu.
   - Configure access control lists (ACLs) and user authentication.

## Network Architecture
The following changes were made to the network infrastructure:
- Implementation of a virtualized server architecture using Proxmox VE.
- Integration of VPN, FTP, Firewall, and Proxy services into the network for comprehensive security.

## Future Improvements
- **IDS/IPS Integration**: Implementing intrusion detection and prevention systems for enhanced security.
- **Monitoring Tools**: Adding network monitoring tools for real-time analysis.

## Contributors
- Ahmed HABAIB
- Islem KHLIFI

## License
This project is licensed under the [MIT License](LICENSE).

