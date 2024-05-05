---
title: Network Communication - N10-008 CompTIA Network+ &#58; 1.4
author: Joey
tags:
  - Section 1&#58; Networking Concepts
  - 1.4 Network Communication
  - IP Subnetting
  - Professer Messer 
layout: post
date: 2024-05-05 12:18:00 -0500
---

<div class="container">
    <iframe class="responsive-iframe" width="560" height="315" src="https://www.youtube.com/embed/CCrY5SYtbz8?si=XOvJgZYbAhaQ7PZP&amp;start=281" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
</div>
[Network Communication - N10-008 CompTIA Network+ : 1.4](https://www.professormesser.com/network-plus/n10-008/n10-008-video/network-communication-n10-008/){:target="_blank"}

## Unicast
- One station sending information to another station
    - One-to-one
- Send information between two systems
- Web surfing, file transfers
- Does not scale optimally for real-time streaming media
- IPv4 and IPv6

## Broadcast
- Send information to everyone at once
    - One-to-all
- Once packet, received by everyone
- Limited scope
    - The broadcast domain
- Routing updates, ARP requests
- Used in IPv4
- Not used in IPv6
    - Uses multicast instead


## Multicast
- Delivery of information to interested systems
    -One-to-many-of-many
    - Multimedia delivery, stock exchanges, dynamic routing updates
    - Very specialized
        - Difficult to scale across large networks
    - Used in both IPv4 and IPv6
        - Extensive use in IPv6
## Anycast
- Single destination IP address has multiple paths or two or more endpoints
    - One-to-one-of-many
    - Used in IPv4 and IPv6
- Configure the same anycast address on different devices
    - Looks like any other unicast address
- Packets sent to an anycast address are delivered to the closest interface
    - Announce the same route out of multiple data centers, clients use the data center closest to them
- Anycast DNS