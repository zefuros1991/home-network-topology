# Home Network Topology and Server Project

This repository documents the network topology and configurations used for setting up my home network and server using Docker, AdGuard, Home Assistant, and other tools. The purpose of this project is to create a secure, efficient, and scalable home network while using the project as part of my portfolio for future career opportunities.

## Network Topology Overview

The home network is structured to have critical devices with static IPs for easy management and redundancy. Below is a summary of the device roles and their static IPs:

### Device Breakdown
1. **PC (Main Device)**
   - Role: Main device running most containers (Home Assistant, AdGuard, SSH, VPN)
   - Static IP: `xxx.xxx.xxx.10` (Replace with your own IP)
2. **Laptop (Windows & Ubuntu)**
   - Role: Backup for the PC, capable of running containers in case of failure, and remote access to the network for configuration and deployment.
   - Static IP: Windows: `xxx.xxx.xxx.20`, Ubuntu: `xxx.xxx.xxx.30` (Replace with your own IP)
3. **Android Phone**
   - Role: Monitoring and media consumption, SSH access to the server
   - Static IP: `xxx.xxx.xxx.40`
4. **Other Devices**
   - Dynamic IPs for non-critical devices like TVs, Google Nest, Nintendo Switch and smart bulbs

## Services and Tools

This project uses various tools and services to provide functionalities like ad-blocking, home automation, VPN access, and more. Below is a list of tools and their official links:

- **Docker**: [Docker](https://www.docker.com/) - Platform to deploy and run containers.
- **AdGuard Home**: [AdGuard](https://adguard.com/) - DNS-based ad blocker to eliminate ads across the network.
- **Home Assistant OS**: [Home Assistant](https://www.home-assistant.io/) - Home automation platform to manage smart devices.
- **SSH**: Secure Shell to remotely access devices and servers.
- **Parsec**: [Parsec](https://parsec.app/) - Remote desktop application for gaming and productivity.
- **OpenVPN/WireGuard**: [OpenVPN](https://openvpn.net/) or [WireGuard](https://www.wireguard.com/) - VPN service to securely connect remotely to the home network.

## Security Considerations

1. **Change Default Credentials**: Never use default usernames or passwords for any service.
2. **Custom Ports**: Use non-standard ports for services to minimize exposure to attacks.
3. **Redundancy**: Services like DHCP and VPN should be able to switch automatically between devices (PC, laptop,or hosted on cloud) to ensure uptime.

## License

This repository contains only the documentation and configurations created for this project. The software tools (Docker, AdGuard, Home Assistant, etc.) are not included in this license and are the property of their respective owners. Please respect the licenses and terms of use provided by these third-party tools.

---

## Credits
Special thanks to the developers of the tools used in this project:
- [Docker](https://www.docker.com/)
- [AdGuard](https://adguard.com/)
- [Home Assistant](https://www.home-assistant.io/)
- [WireGuard](https://www.wireguard.com/)
- [Parsec](https://parsec.app/)


