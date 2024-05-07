---
title: Introduction to IP - N10-008 CompTIA Network+ &#58; 1.5
author: Joey
tags:
  - Section 1&#58; Networking Concepts
  - 1.5 Introduction to IP
  - Ports and Protocols
  - Professer Messer 
layout: post
date: 2024-05-07 16:07:00 -0500
---

<div class="container">
    <iframe class="responsive-iframe" width="560" height="315" src="https://www.youtube.com/embed/NAI-gE51VXg?si=YFTLvbZZcjLQItKn&amp;start=335" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
</div>
[Introduction to IP - N10-008 CompTIA Network+ : 1.5](https://www.professormesser.com/network-plus/n10-008/n10-008-video/introduction-to-ip-n10-008/){:target="_blank"}

## A series of moving vans
- Efficiently move large amounts of data 
    - Use a shippinng truck
- The network topology is the road
    - Ethernet, DSL, cable system
- The truck is the Internet Protocol (IP)
    - We've designed the roads for this truck
- The boxes hold your data
    - Boxes of TCP and UDP
- Inside the boxes are more things
    - Application information

## IP - Internet Protocol

[![Internet Protocol]({{site.baseurl}}/img/ip.png)](https://youtu.be/NAI-gE51VXg?si=gMC2JMZkCJaiBml3&t=110){:target="_blank"}

## TCP and UDP
- Transported inside of IP 
    - Encapsulated by the IP protocol
- Two different ways to move data from place to place
    - Different features for different applications
- OSI Layer 4
    - The transport layer
- Multiplexing
    - Use many different applications at the same time
    - TCP and UDP

## TCP - Transmission Control Protocol 
- Connection-oriented
    - A formal connection setup and close
- Reliable delivery
    - Recovery from errors
    - Can manage out-of-order messages or retransmissions
- Flow control
    - The receiver can manage how much data is sent

## UDP - User Datagram Protocol
- Connectionless
    - No formal open or close to the connection
- Unreliable delivery
    - No error recovery
    - No reordering of data or retransmissions
- No flow control
    - Sender determines the amount of data transmitted

## Speedy delivery
- The IP delivery truck delivers from one (IP) address to another (IP) address
    - Every house has an address, every computer has an IP address
- Boxes arrive at the house / IP address
    - Where do the boxes go?
    - Each box has a room name
- Port is written on the outside of the box
    - Drop the box into the right room

## Lots of ports 
- IPv4 sockets 
    - Server IP address, protocol, server application port number
    - Client IP address, protocol, client port number
- Non-ephemeral ports - permanent port numbers
    - Ports 0 through 1,023
    - Usually on a server or service
- Ephemeral ports - temporary port numbers
    - Ports 1,024 through 65,535

## Port numbers
- TCP and UDP ports can be any number between 0 and 65,535
- Most servers (services) use non-ephemeral (not-temporary) port numbers
    - This isn't always the case
        - It's just a number.
- Port numbers are for communication, not security
- Service port numbers need to be "well known"
- TCP port numbers aren't the same as UDP port numbers

## Ports on the network
- Web server - TCP/80
- VoIP server - UDP/5004
- Email server - TCP/143

[![Ports on the network]({{site.baseurl}}/img/ports.png)](https://youtu.be/NAI-gE51VXg?si=XwK3x5HbMlT9bARb&t=670){:target="_blank"}

[![Ports on the network]({{site.baseurl}}/img/ports1.png)](https://youtu.be/NAI-gE51VXg?si=XwK3x5HbMlT9bARb&t=670){:target="_blank"}

