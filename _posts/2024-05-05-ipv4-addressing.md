---
title: IPv4 Addressing - N10-008 CompTIA Network+ &#58; 1.4
author: Joey
tags:
  - Section 1&#58; Networking Concepts
  - 1.4 IPv4 Addressing
  - IP Subnetting
  - Professer Messer 
layout: post
date: 2024-05-05 11:15:43 -0500
---

<div class="container">
    <iframe class="responsive-iframe" width="560" height="315" src="https://www.youtube.com/embed/cHQCxQ_MC4E?si=qhHOTnHaT0qDDaRI&amp;start=431" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
</div>
[IPv4 Addressing - N10-008 CompTIA Network+ : 1.4](https://www.professormesser.com/network-plus/n10-008/n10-008-video/ipv4-addressing-n10-008/){:target="_blank"}

## Networking with IPv4
- IP Address, e.g., 192.168.1.165
    - Every device needs a unique IP address
- Subnet mask, e.g., 255.255.255.0
    - Used by the local device to determine what subnet it's on
        - The subnet mask isn't (usually) transmitted across the network
        - You'll ask for subnet masks all the time
            - What's the subnet mask of this network?
- Default gateway, e.g., 192.168.1.1
    - The router that allows you to communicate outside of your local subnet
    - The default gateway must be an IP address on the local subnet

## Special IPv4 Addresses
- Loopback address
    - An address to yourself
    - Ranges from 127.0.0.1 through 127.255.255.254
    - An easy-way to self-reference (ping 127.0.0.1)
- Reserved addresses
    - Set aside for future use or testing
    - 240.0.0.1 through 254.255.255.254
    - All "Class E" addresses
- Virtual IP Addresses (VIP)
    - Not associated with a physical network adapter
    - Virtual machine, internal router address

## IPv4 Addresses
- Internet Protocol version 4
    - OSI Layer 3 address
    - Since one bye is 8 bits, the max decimal value for each byte is 255
[![IPv4 Address]({{site.baseurl}}/img/ipv4_address.png)](https://youtu.be/cHQCxQ_MC4E?si=6YSc8zURmOMPtzSK&t=295){:target="_blank"}

## DHCP
- IPv4 address configuration used to be a manual process
    - IP address, subnet mask, gateway, DNS servers, NTP servers, etc.
- Dynamic Host Configuration Protocol
    - Provides automatic address and IP configuration for almost all devices

## Automatic Private IP Addressing (APIPA)
- A link-local address
    - Can only communicate to other local devices
    - No forwarding by routers 
- IETF has reserved 169.254.0.1 through 169.254.255.254
    - First and last 256 addresses are reserved 
    - Functional block of 169.254.1.0 through 169.254.254.255
