# Packet Tracer – Use Telnet and SSH

## Overview
This lab demonstrates remote router access using Telnet and Secure Shell (SSH). It highlights the security difference between an unencrypted remote-access protocol and an encrypted alternative.

## Objectives
- Verify DHCP addressing on client PCs.
- Test connectivity to a router using ping.
- Attempt remote access using Telnet.
- Access the router securely using SSH.

## Network Configuration

| Device | Interface | IP Address |
|---|---|---|
| HQ | G0/0/1 | 64.100.1.1 |
| PC0 | NIC | DHCP |
| PC1 | NIC | DHCP |

## Procedure

### 1. Verify IP Configuration
Used the following command on a client PC:

`ipconfig`

Verified that the PC received an IP address through DHCP.

### 2. Verify Connectivity
Used ping to test connectivity to the HQ router:

`ping 64.100.1.1`

### 3. Test Telnet Access
Attempted to connect to the router using:

`telnet 64.100.1.1`

The router did not permit insecure Telnet access.

### 4. Connect Using SSH
Established a secure remote connection using:

`ssh -l admin 64.100.1.1`

Entered the lab-provided password when prompted. The router displayed its command-line prompt after successful authentication.

## Key Concepts Learned
- DHCP addressing
- ICMP and ping connectivity testing
- Remote device administration
- Telnet versus SSH
- Secure authentication and encrypted management sessions

## Security Notes
Telnet transmits data, including credentials, without encryption. SSH encrypts the remote management session and is preferred for securely administering network devices.

## Evidence
Add screenshots showing the IP configuration, ping results, Telnet failure, and successful SSH login.

## Skills Demonstrated
Cisco Packet Tracer, TCP/IP, DHCP, ICMP, Telnet, SSH, and network security fundamentals.
