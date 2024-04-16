---
title: Understanding the OSI Model
author: Joey
tags:
  - Networking Concepts
  - The OSI Model
  - Professer Messer 
layout: post
date: 2024-04-13 10:10:09 -0500
---

<div class="container">
    <iframe class="responsive-iframe" width="560" height="315" src="https://www.youtube.com/embed/owDh6FNJUog?si=wejbeaMzPjl3eJCU" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe><br>
</div>

[Understanding the OSI Model – N10-008 CompTIA Network+ : 1.1](https://www.professormesser.com/?p=624596){:target="_blank"}

## The OSI Model

| Layer 7 Application  |
| Layer 6 Presentation |
| Layer 5 Session      |
| Layer 4 Transport    |
| Layer 3 Network      |
| Layer 2 Data Link    |
| Layer 1 Physical     |

- What is the OSI model?
    - Open Systems Interconnection Reference Model
- It's a guide / model
    - The OSI model is a way to describe how network traffic is moving from one part of the network to another
- This is not the OSI protocol suite
    - Most of the OSI protocols didn't catch on (we use TCP/IP)
- There are unique protocols at every layer
- You'll refer to the OSI model for the rest of your career
    - It's a common language within IT to describe how data is progressing from the very beginning of the traffic flow to the very end

## A [Mnemonic](https://www.merriam-webster.com/dictionary/mnemonic){:target="_blank"} To Remember the OSI Model

    7. Application      (All)
    6. Presentation     (People)
    5. Session          (Seem)
    4. Transport        (To)
    3. Network          (Need)
    2. Data Link        (Data)
    1. Physical         (Processing)

## Layer 1 - The Physical Layer

- The physics of the network
    - Signaling, cabling, connectors
    - This layer isn't about protocols
- "You have a physical layer problem."
    - Fix your cabling, punch-downs, etc.
    - Run loopback tests, test/replace cables, swap adapter cards

## Layer 2 - Data Link Layer

- The basic network "language"
    - The foundation of communication at the data link layer
- Data Link Control (DLC) protocols
    - MAC (Media Access Control) address on Ethernet
- The "switching" layer

## Layer 3 - Network Layer

- The "routing" layer
- Internet Protocol (IP)
- Fragments frames to traverse different networks

## Layer 4 - Transport Layer

- The "post office" layer
    - Parcels and letters
- Transport Protocols
    - TCP (Transmission Control Protocol)
    - UDP (User Datagram Protocol)

## Layer 5 - Session Layer

- Communication management between devices
    - Start, stop, restart
- Control protocols, tunneling protocols

## Layer 6 - Presentation Layer

- Character encoding
- Application encryption
- Often combined with the Application Layer

## Layer 7 - Application Layer

- The layer we see
- Application layer protocols
    - HTTP/S
    - S/FTP
    - DNS
    - POP3
    - SSH

## Real-world to OSI Model

| Layer 7 Application         | Your eyes                                                               |
| Layer 6 Presentation        | Application encryption (SSL/TLS)                                        |
| Layer 5 Session             | Control protocols, tunneling protocols                                  |
| Layer 4 Transport           | TCP segment, UDP datagram                                               |
| Layer 3 Network             | IP Address, Router, Packet                                              |
| Layer 2 Data Link           | Frame, MAC address, Extended Unique Identifier (EUI-48, EUI-64), Switch |
| Layer 1 Physical            | Cables, fiber, and the signal itself                                    |

## Follow the conversation

| Layer 7 Application         | https://mail.google.com                |
| Layer 6 Presentation        | SSL encryption                         |
| Layer 5 Session             | Link the presentation to the transport |
| Layer 4 Transport           | TCP encapsulation                      |
| Layer 3 Network             | IP encapsulation                       |
| Layer 2 Data Link           | Ethernet                               |
| Layer 1 Physical            | Electrical signals                     |