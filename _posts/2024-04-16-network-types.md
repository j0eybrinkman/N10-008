---
title: Network Types - N10-008 CompTIA Network+ &#58; 1.2
author: Joey
tags:
  - Networking Concepts
  - Network Types
  - Professer Messer 
layout: post
date: 2024-04-16 21:07:14 -0500
---

<div class="container">
    <iframe class="responsive-iframe" width="560" height="315" src="https://www.youtube.com/embed/6a-roIeJ_a4?si=xJw8fK8LLUou-PFd" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
</div>
[Network Types - N10-008 CompTIA Network+ - 1.2](https://www.professormesser.com/network-plus/n10-008/n10-008-video/network-types-5/){:target="_blank"}

## Peer-to-peer
- All devices are both clients and servers
    - Everyone talks to everyone
- Advantages
    - Easy to deploy
    - Low cost
- Disadvantages
    - Difficult to administer
    - Difficult to secure

## Client-server
- Central server
    - Clients talk to the server
- No client-to-client communication
- Advantages
    - Performance, administration
- Disadvantages
    - Cost, complexity

## LAN
- Local Area Network
    - Local is relative
- A building or group of buildings
    - High-speed connectivity
- Ethernet and 802.11 wireless
    - Any slower and it isn't "local"

## MAN
- Metropolitan Area Network
    - A network in your city
    - Larger than a LAN, often smaller than a WAN
- Historically MAN-specific topologies
    - Everyone's moving to Metro Ethernet
- Common to see government ownership
    - They "own" the right-of-way

## WAN
- Wide Area Network
    - Spanning the globe
- Generally connects LANs across a distance
    - And generally much slower than the LAN
- Many different WAN technologies
    - Point-to-point serial, MPLS, etc.
    - Terrestrial and non-terrestrial

## WLAN 
- Wireless LAN
    - 802.11 technologies
- Mobility
    - Within a building
    - In a limited geographical area
- Expand coverage with additional access points 
    - Downtown area
    - Large campus

## PAN
- Personal Area Network
    - Your own private network
    - Bluetooth, IR, NFC
- Automobile
    - Audio output
    - Integrate with phone
- Mobile phone
    - Wireless headset
- Health
    - Workout telemetry, daily reports

## CAN
- Campus Area Network
    - Corporate Area Network
- Limited geographical area
    - A group of buildings
- LAN technologies
    - Fiber connected
    - High speed Ethernet
- Your fiber in the ground
    - No third-party provider

## NAS vs. SAN
- Network Attached Storage (NAS)
    - Connect to a shared storage device across the network 
    - File-level access
- Storage Area Network (SAN)
    - Looks and feels like a local storage device
        - Block-level access
            - Very efficient reading and writing
- Requires a lot of bandwidth
    - May use an isolated network and high-speed network technologies

## MPLS
- Learning from ATM and Frame Relay
    - Keep the advantages, ditch the disadvantages
- Packets through the WAN have a label
    - Routing decisions are easy
- Any transport medium, any protocol inside
    - IP packets, Ethernet frames
- A common WAN technology
    - Ready-to-network

## MPLS pushing and popping
- Labels are "pushed" onto packets as they enter the MPLS cloud
- Labels are "popped" off on the way out

[![MPLS]({{site.baseurl}}/img/mpls.png)](https://www.noction.com/wp-content/uploads/2018/03/BGP-VPN-i1.png){:target="_blank"}

## mGRE

- Multipoint Generic Router Encapsulation   
    - Used extensively for Dynamic Multipoint VPN (DMVPN)
    - Common on Cisco routers
- Your VPN builds itself
    - Remote sites communicate to each other
- Tunnels are built dynamically
    - on-demand
    - A dynamic mesh

## SD-WAN
- Software Defined Networking in a Wide Area Network
    - A WAN built for the cloud
- The data center used to be in one place
    - The cloud has changed everything
- Cloud-based applications communicate directly to the cloud
    - No need to hop through a central point