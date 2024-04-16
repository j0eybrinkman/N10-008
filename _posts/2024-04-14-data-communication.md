---
title: Data Communication - N10-008 CompTIA Network+ &#58; 1.1
author: Joey
tags:
  - Networking Concepts
  - The OSI Model
  - Professer Messer 
layout: post
date: 2024-04-14 21:38:59 -0500
---

<div class="container">
    <iframe class="responsive-iframe" width="560" height="315" src="https://www.youtube.com/embed/jKjVTPpcZT0?si=Jpcq9tuH_KBtIcaA" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
</div>

[Data Communication – N10-008 CompTIA Network+ : 1.1](https://www.professormesser.com/network-plus/n10-008/n10-008-video/data-communication/){:target="_blank"}

## PDU (Protocol Data Unit)

- Transmission units
    - A different group of data at different OSI layers
- Ethernet operates on a frame of data
    - It doesn't care what's inside    
- IP operates on a packet of data
    - Inside is TCP or UDP, but IP doesn't really care

## TCP or UDP
- TCP segment
- UDP datagram

## Data Encapsulation
[![Data encapsulation](/assets/img/osi-encap.gif)](https://www.firewall.cx/images/stories/osi-encap.gif){:target="_blank"}

## Data Decapsulation
[![Data Decasulation](/assets/img/osi-decap.gif)](https://www.firewall.cx/images/stories/osi-encap-decap-2.gif){:target="_blank"}

## Dissecting a Frame
 - Each layer has a header and payload
[![Dissecting a Frame](/assets/img/dissecting_a_frame.png)](https://youtu.be/jKjVTPpcZT0?si=r5nqWxfWKd4AoBBF&t=230){:target="_blank"}

## TCP Flags
- The header describes or identifies the payload
    - Here's what you're about to see...
- The TCP header contains important control information
    - Includes a set of bits called TCP flags

[![TCP Flags](/assets/img/TCP_flags.png)](/assets/img/TCP_flags.png)

- The flags control the payload
    - SYN - Synchronize sequence numbers
    - PSH - Push the data to the application without buffering
    - RST - Reset the connection
    - FIN - Last packet from the sender

## Maximum Transmission Unit (MTU)
- Maximum IP packet to transmit
    - But not fragment

[![TCP Flags](/assets/img/mtu.png)](/assets/img/mtu.png)

- Fragmentation slows things down
    - Losing a fragment loses an entire packet
    - Requires overhead along the path
- Difficult to know the MTU all the way through the path
    - Automated methods are often inaccurate
    - Especially when ICMP is filtered

## Building an Ethernet Frame
[![Building an Ethernet Frame](/assets/img/building_an_ethernet_frame.jpg)](https://img1.daumcdn.net/thumb/R800x0/?scode=mtistory2&fname=https%3A%2F%2Ft1.daumcdn.net%2Fcfile%2Ftistory%2F9996AB4B5C17508B16){:target="_blank"}

## What is IP Fragmentation?

[![IP Fragmentation](/assets/img/ip_fragmentation.png)](https://upload.wikimedia.org/wikipedia/commons/c/cd/PDU_Fragmentation-en.png){:target="_blank"}

- Fragments are always in multiples of 8 because the number of fragmentation offsets bits in the IP header

## Troubleshooting MTU
- MTU sizes are usually configured once
    - Based on the network infrastructure and don't change often
- A significant concern for tunneled traffic
    - The tunnel may be smaller than your local Ethernet segment
- What if you send packets with Don't Fragment (DF) set?
    - Routers will respond back and tell you to fragment
    - Hope you get the ICMP message!
- Troubleshoot using ping
    - Ping with DF and force a maximum size 1472 bytes 
        - 1500 bytes - 8 byte ICMP header - 20 bytes IP address = 1472
            - Windows: `ping -f -l 1472 1.1.1.1`
            - Linux and macOS: `ping -D -s 1472 1.1.1.1 -c4`