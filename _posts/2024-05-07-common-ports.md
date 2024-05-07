---
title: Common Ports - N10-008 CompTIA Network+ &#58; 1.5
author: Joey
tags:
  - Section 1&#58; Networking Concepts
  - 1.5 Common Ports
  - Ports and Protocols
  - Professer Messer 
layout: post
date: 2024-05-07 16:44:00 -0500
---

<div class="container">
    <iframe class="responsive-iframe" width="560" height="315" src="https://www.youtube.com/embed/S0dKMst-ED0?si=yyFrsDGgJXjhK7gj&amp;start=151" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
</div>
[Common Ports - N10-008 CompTIA Network+ : 1.5](https://www.professormesser.com/network-plus/n10-008/n10-008-video/common-ports-n10-008/){:target="_blank"}

## Telnet
- Telnet - Telecommunication Network
    - TCP/23
- Login to devices remotely
- Console access
- In-the-clear communication
- Not the best choice for production systems

## SSH - Secure Shell
- Encrypted communication link - TCP/22 
- Looks and acts the same as Telnet

## DNS - Domain Name System
- Converts names to IP addresses - UDP/53
    - www.professormesser.com = 104.22.73.108, 104.22.72.108, and 172.67.41.114
    - Large transfers may use TCP/53
- These are very critical resources
    - Usually multiple DNS servers are in production

## SMTP - Simple Mail Transfer Protocol
- SMTP - Simple Mail Transfer Protocol 
    - Server to server email transfer
    - TCP/25 (SMTP using plaintext)
    - TCP/587 (SMTP using TLS encryption)
- Also used to send mail from a device to a mail server
    - Commonly configured on mobile devices and email
- Other protocols are used for clients to receive email
    - IMAP, POP3

## POP / IMAP
- Receive emails from an email server
    - Authenticate and transfer
- POP3 - Post office Protocol version 3
    - TCP/110 (plaintext), TCP/995 (POP3 over TLS)
    - Basic mail transfer functionality
- IMAP4 - Internet Message Access Protocol v4
    - TCP/143 (plaintext), TCP/993 (IMAP over TLS)
    - Includes management of email inbox from multiple clients

## SFTP - Secure FTP
- Uses the SSH File Transfer Protocol
    - TCP/22
- Provides file system functionality
    - Resuming interrupted transfers, directory listings, remote file removal
- Encrypted communication
    - Uses SSH (port 22)

## File transfer application protocols
- FTP - File Transfer Protocol
    - TCP/20 (active mode data), TCP/21 (control)
    - Transfers files between systems
    - Authenticates with a username and password
    - Full-featured functionality (list, add, delete, etc.)
- TFTP - Trivial File Transfer Protocol
    - UDP/69
    - Very simple file transfer application
        - Read files and write files
    - No authentication
        - Not used on production systems

## DHCP - Dynamic Host Coniguration Protocol
- Automated configuration of IP address, subnet mask, and other options
    - UDP/67, UDP/68
    - Requires a DHCP server
        - Server, appliance, integrated into SOHO router, etc.
    - Dynamic / pooled 
        - IP addresses are assigned in real-time from a pool
        - Each system is given a lease and must renew at set intervals
    - DHCP reservation
        - Addresses are assigned by MAC address in the DHCP server
        - Quickly manage addresses from one location

## HTTP and HTTPS
- Hypertext Transfer Protocol
    - Communication in the browser
    - And by other applications
- In the clear or encrypted
    - SSL (Secure Sockets Layer) or TLS (Transport Layer Security)

| Protocol | Port    | Name                        | Description                              |
|----------|---------|-----------------------------|------------------------------------------|
| HTTP     | TCP/80  | Hypertext Transfer Protocol | Web server communication                 |
| HTTPS    | TCP/443 | HTTP over TLS or SSL        | Web server communication with encryption |

## SNMP - Simple Network Management Protocol
- Gather statistics from network devices
    - UDP/161
- v1 - The original 
    - Structured tables
    - In-the-clear
- v2 - A good step ahead
    - Data type enhancements
    - Bulk transfers
    - Still-in-the-clear
- v3 - A secure standard
    - Message integrity
    - Authentication
    - Encryption
- SNMP traps 
    - Alerts and notifications from the network devices
    - UDP/162

## Syslog
- Standard for message logging
    - Diverse systems, consolidated log
    - UDP/514
- Usually a central log collector
    - Integrated into the SIEM
- You're going to need a lot of disk space
    - No, more. More than that. 
    - Data storage from many devices over an extended timeframe

## RDP - Remote Desktop Protocol
- Share a desktop from a remote location over TCP/3389
- Remote Desktop Services on many Windows versions
- Can connect to an entire desktop or just an application
- Clients for Windows, MacOS, Linux, Unix, iPhone, and others

## NTP - Network Time Protocol
- Switches, routers, firewalls, servers, workstations
    - Every device has its own clock
    - UDP/123
- Synchronizing the clocks becomes critical 
    - Log files, authentication information, outage details
- Automatic updates
    - No flashing 12:00 lights
- Flexible - You control how clocks are updated
- Very accurate
    - Accuracy is better than 1ms on a local network

## SIP - Session Initiation Protocol 
- Voice over IP (Voip) signaling
    - TCP/5060 and TCP/5061
- Setup and manage VoIP sessions
    - Call, ring, hang up
- Extend voice communication
    - Video conferencing
    - Instant messaging
    - File transfer
    - etc.

## SMB - Server Message Block
- Protocol used by Microsoft Windows
    - File sharing, printer sharing
    - Also called CIFS (Common Internet File System)
- Direct over TCP/445 (NetBIOS-less)
    - Direct SMB communication over TCP without the NetBIOS transport

## LDAP / LDAPS - Lightweight Directory Access Protocol
- LDAP (Lightweight Directory Access Protocol)
    - TCP/389
    - Store and retrieve information in a network directory
- LDAPS (Lightweight Directory Access Protocol Secure)
    - A non-standard implementation of LDAP over SSL
    - TCP/636

## Databases
- Microsoft SQL Server
    - MS-SQL (Microsoft Structured Query Language)
    - TCP/1433
- Oracle SQL *Net
    - Also called Oracle Net or Net8
    - TCP/1521
- MySQL free and open-source database
    - Ultimately acquired by Oracle
    - TCP/3306