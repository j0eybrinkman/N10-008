---
title: Network Architectures - N10-008 CompTIA Network+ &#58; 1.7
author: Joey
tags:
  - Section 1&#58; Networking Concepts
  - 1.7 Network Architectures
  - Network Services
  - Professer Messer 
layout: post
date: 2024-05-08 11:34:00 -0500
---

<div class="container">
    <iframe class="responsive-iframe" width="560" height="315" src="https://www.youtube.com/embed/23H0nA-_4YE?si=LGZrPx1IAcO239uT&amp;start=100" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
</div>
[Network Architectures - N10-008 CompTIA Network+ : 1.7](https://www.professormesser.com/network-plus/n10-008/n10-008-video/network-architectures-n10-008/){:target="_blank"}

## Three-tier architecture 
- Core
    - The "center" of the network
    - Web servers, databases, applications
    - Many people need access to this
- Distribution
    - A midpoint between the core and the users
    - Communication between access switches
    - Manage the path to the end users
- Access
    - Where the users connect
    - End stations, printers

[![Three-tier architecture]({{site.baseurl}}/img/three-tier-architecture.png)](#){:target="_blank"}
[![Three-tier architecture]({{site.baseurl}}/img/three-tier-architecture1.png)](#){:target="_blank"}

## SDN (Software Defined Networking)
- Networking devices have different functional planes of operation
    - Data, control, and management planes
- Split the functions into separate logical units
    - Extend the functionality and management of a single device 
    - Perfectly built for the the cloud
- Infrastructure layer / Data plane
    - Process the network frames and packets
    - Forwarding, trunking, encrypting, NAT
- Control layer / Control plane
    - Manages the actions of the data plane
    - Routing tables, session tables, NAT tables
    - Dynamic routing protocol updates
- Application layer / Management plane
    - Configure and manage the device

## Extend the physical architecture
[![Extend the physical architecture]({{site.baseurl}}/img/extend_the_physical_architecture.png)](#){:target="_blank"}

## SDN Data Flows
[![SDN Data Flows]({{site.baseurl}}/img/sdn_data_flows.png)](#){:target="_blank"}

## Spine and leaf architecture
- Each leaf switch connects to each spine switch
    - Each spine switch connects to each leaf switch
- Leaf switches do not connect to each other
    - Same for spine switches
- Top-of-rack switching
    - Each leaf is on the "top" of a physical network rack
    - May include a group of physical racks
- Advantages
    - Simple cabling
    - Redundant
    - Fast
- Disadvantages
    - Additional switches may be costly

## Traffic flows
- Traffic flows within a data center
    - Important to know where traffic starts and ends
- East-west
    - Traffic between devices in the same data center
    - Relatively fast response times
- North-south traffic
    - Ingress/egress to an outside device
    - A different security posture than east-west traffic

## Network locations
- Branch office
    - A remote location
    - Client devices, printers, switch/router/firewall
- On-premises data center
    - Technology is located in-house
    - Requires power, cooling, and ongoing monitoring
- Colocation
    - Share a data center with others
    - Local oversight and monitoring