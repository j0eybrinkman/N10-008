---
title: Configuring IPv6 - N10-008 CompTIA Network+ &#58; 1.4
author: Joey
tags:
  - Section 1&#58; Networking Concepts
  - 1.4 Configuring IPv6
  - IP Subnetting
  - Professer Messer 
layout: post
date: 2024-05-07 12:12:00 -0500
---

<div class="container">
    <iframe class="responsive-iframe" width="560" height="315" src="https://www.youtube.com/embed/S0dKMst-ED0?si=yyFrsDGgJXjhK7gj&amp;start=151" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
</div>
[Configuring IPv6 - N10-008 CompTIA Network+ : 1.4](https://www.professormesser.com/network-plus/n10-008/n10-008-video/configuring-ipv6-n10-008/){:target="_blank"}

## Tunneling IPv6
- 6to4 addressing
    - Send IPv6 over an existing IPv4 network
    - Creates an IPv6 address based on the IPv4 address
    - Requires relay routers
    - No support for NAT
- 4in6 tunneling
    - Tunnel IPv4 traffic on an IPv6 network

## Teredo / Miredo
- Tunnel IPv6 through NATed IPv4
    - End-to-end IPv6 through an IPv4 network
    - No special IPv6 router needed
    - Temporary use 
        - We'll have IPv6 native networks soon (?)
- Miredo
    - Open-source Teredo for Linux, BSD Unix, and Mac OS X
    - Full functionality

## Dual-stack routing
- Dual-stack IPv4 and IPv6
    - Run both at the same time
    - Interfaces will be assigned multiple address types
- IPv4
    - Configured with IPv4 addresses
    - Maintains an IPv4 routing table
    - Uses IPv4 dynamic routing protocols

## Howdy, neighbor
- There's no ARP in IPv6
    - So how do you find out the MAC address of a device?
- Neighbor Solicitation (NS)
    - Sent as a multicast
- Neighbor Advertisement (NA)

[![Howdy, neighbor]({{site.baseurl}}/img/howdy_neighbor.png)](https://youtu.be/S0dKMst-ED0?si=8NtfjRzInmwH1QUa&t=236){:target="_blank"}

## NDP (Neighbor Discovery Protocol)
- No broadcasts!
    - Operates using multicast with ICMPv6
- Neighbor MAC Discovery
    - Replaces the IPv4 ARP
- SLAAC (Stateless Address Autoconfiguration)
    - Automatically configure an IP address without a DHCP server
- DAD (Duplicate Address Detection)
    - No duplicate IPs!
- Discover routers
    - Router Solicitation (RS) and Router Advertisement (RA)

## Finding Router
- Use the Neighbor Discovery Protocol 
- Routers also send unsolicited RA messages
    - From the multicast destination of ff02::1
- Transfers IPv6 address information, prefix value, and prefix length, etc.

[![Howdy, neighbor]({{site.baseurl}}/img/finding_router.png)](https://youtu.be/S0dKMst-ED0?si=KN_NW0TRV5QCc68i&t=335){:target="_blank"}




