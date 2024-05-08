---
title: An Overview of NTP - N10-008 CompTIA Network+ &#58; 1.6
author: Joey
tags:
  - Section 1&#58; Networking Concepts
  - 1.6 An Overview of NTP
  - Network Services
  - Professer Messer 
layout: post
date: 2024-05-08 10:19:00 -0500
---
<div class="container">
    <iframe class="responsive-iframe" width="560" height="315" src="https://www.youtube.com/embed/iBHRIu9MQr4?si=UIVN3f6C8k4OOMIU&amp;start=100" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
</div>
[An Overview of NTP - N10-008 CompTIA Network+ : 1.6](https://www.professormesser.com/network-plus/n10-008/n10-008-video/an-overview-of-ntp-n10-008/){:target="_blank"}

## NTP (Network Time Protocol)
- Switches, routers, firewalls, servers, workstations
    - Every device has its own clock
- Synchronizing the clocks becomes critical
    - Log files, authentication information, outage details
- Automatic updates
    - No flashing 12:00 lights
- Flexible
    - You control how clocks are updated
- Very accurate
    - Accuracy is better than 1ms on a local network

## NTP clients and servers
- NTP server
    - Listens on UDP/123, responds to time requests from NTP clients
    - Does not modify their own time
- NTP client
    - Requests time updates from NTP server
- NTP client/server
    - Requests time updates from an NTP server
    - Responds to time requests from other NTP clients
- Important to plan your NTP strategy
    - Which devices are clients, servers, and client/servers?

## NTP stratum layers
- Some clocks are better than others
    - Your distance from the original reference clock is a stratum
- Stratum 0
    - Atomic clock, GPS clock
    - Very accurate
- Startum 1
    - Synchronized to stratum 0 servers
    - Primary time servers
- Stratum 2
    - Sync'd to stratum 1 servers

## Configuring NTP
- NTP client
    - Specify the NTP server address (IP or hostname)
    - Use multiple NTP servers (if available) for redundancy 
- NTP server
    - You need at least one clock source
    - Specify the stratum level of the clock
    - If there's a choice, the lower stratum level wins 