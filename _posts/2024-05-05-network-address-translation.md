---
title: Network Address Translation - N10-008 CompTIA Network+ &#58; 1.4
author: Joey
tags:
  - Section 1&#58; Networking Concepts
  - 1.4 Network Address Translation
  - IP Subnetting
  - Professer Messer 
layout: post
date: 2024-05-05 11:42:33 -0500
---

<div class="container">
    <iframe class="responsive-iframe" width="560" height="315" src="https://www.youtube.com/embed/NkCx8AnzBaI?si=K-pF7-hnOOZnToU_&amp;start=295" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
</div>
[Network Address Translation - N10-008 CompTIA Network+ : 1.4](https://www.professormesser.com/network-plus/n10-008/n10-008-video/network-address-translation-n10-008/){:target="_blank"}

## NAT (Network Address Translation)
- It is estimated that there are over 20 billion devices connected to the internet (and growing)
- IPv4 supports around 4.29 billion addresses
- The address space for IPv4 is exhausted
    - There are no available addresses to assign
- How does it all work?
    - Network Address Translation
- This isn't the only use of NAT
    - NAT is handy in many situations

## Public Addresses vs Private Addresses
- RFC 1918 private IPv4 Addresses

| IP address range              | Number of addresses | Classful description    | Largest CIDR block (subnet mask) | Host ID size |
|-------------------------------|---------------------|-------------------------|----------------------------------|--------------|
| 10.0.0.0 - 10.255.255.255     | 16,777,216          | single class A          | 10.0.0.0/8 (255.0.0.0)           | 24 bits      |
| 172.16.0.0 - 172.31.255.255   | 1,048,576           | 16 contiguous class Bs  | 172.16.0.0/12 (255.240.0.0)      | 20 bits      |
| 192.168.0.0 - 192.168.255.255 | 65,536              | 256 contiguous class Cs | 192.168.0.0/16 
(255.255.0.0)     | 16 bits      |

## Network Address Translation

[Watch NAT in Action](https://youtu.be/NkCx8AnzBaI?si=zgg1x0LdQWA2stUX&t=138){:target="_blank"}

## NAT Overload / PAT

[Watch PAT in Action](https://youtu.be/NkCx8AnzBaI?si=NHx-3xV5X_mOxNWt&t=281){:target="_blank"}
