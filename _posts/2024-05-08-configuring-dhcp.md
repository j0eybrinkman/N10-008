---
title: Configuring DHCP - N10-008 CompTIA Network+ &#58; 1.6
author: Joey
tags:
  - Section 1&#58; Networking Concepts
  - 1.6 Configuring DHCP
  - Network Services
  - Professer Messer 
layout: post
date: 2024-05-08 9:53:00 -0500
---

<div class="container">
    <iframe class="responsive-iframe" width="560" height="315" src="https://www.youtube.com/embed/0Ddl90OXYFo?si=4C05Hjg4jIfh2YHz&amp;start=100" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
</div>
[DHCP Overview - N10-008 CompTIA Network+ : 1.6](https://www.professormesser.com/network-plus/n10-008/n10-008-video/dhcp-overview-n10-008/){:target="_blank"}

## Scope properties 
- IP address range
    - And excluded addresses
- Subnet mask
- Lease durations
- Other scope options
    - DHCP server
    - Default gateway
    - VoIP server
- DHCP pools
    - Grouping of IP addresses
    - 192.168.1.0/24
    - 192.168.2.0/24
    - 192.168.3.0/24 
- A scope is generally a single contiguous pool of IP addresses
    - DHCP exceptions can be made inside of the scope
- DHCP address assignment
    - Dynamic assignment 
    - DHCP server has a big pool of addresses to give out
    - Addresses are reclaimed after a lease period
- Automatic assignment 
    - Similar to dynamic allocation
    - DHCP server keeps a list of past assignments
    - You'll always get the same IP address
- DHCP address allocation
    - Static assignment
        - Administratively configured
    - Table of MAC addresses
        - Each MAC address has a matching IP address
    - Other names
        - Static DHCP assignment
        - Static DHCP 
        - Address Reservation
        - IP Reservation
- DHCP leases
    - Leasing your address
        - It's only temporary 
        - But it can seem permanent
    - Allocation
        - Assigned a lease time by the DHCP server
        - Administratively configured
    - Reallocation
        - Reboot your computer
        - Confirms the lease
    - Workstation can also manually release the IP address
        - Moving to another subnet
- DHCP renewal
    - T1 timer 
        - Check in with the lending DHCP server to renew the IP address
        - 50% of the lease time (by default)
    - T2 timer
        - If the original DHCP server is down, try rebinding with any DHCP server
        - 87.5% of the lease time (7/8ths)

## The DHCP lease process

[![The DHCP lease process]({{site.baseurl}}/img/dhcp_lease_process.png)](#){:target="_blank"}
