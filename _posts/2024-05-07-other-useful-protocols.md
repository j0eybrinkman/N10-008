---
title: Other Useful Protocols - N10-008 CompTIA Network+ &#58; 1.5
author: Joey
tags:
  - Section 1&#58; Networking Concepts
  - 1.5 Other Useful Protocols
  - Ports and Protocols
  - Professer Messer 
layout: post
date: 2024-05-07 17:48:00 -0500
---

<div class="container">
    <iframe class="responsive-iframe" width="560" height="315" src="https://www.youtube.com/embed/K0o4XDkDRHA?si=nKl8wMLLt-g87aWo&amp;start=670" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
</div>
[Other Useful Protocols - N10-008 CompTIA Network+ : 1.5](https://www.professormesser.com/network-plus/n10-008/n10-008-video/other-useful-protocols-n10-008/){:target="_blank"}

## ICMP
- Internet Control Message Protocol
    - "Text messaging" for your network devices
- Another protocol carried by IP
    - Not used for data transfer
- Devices can request and reply to administrative requests
    - Hey, are you there? / Yes, I'm right here.
- Devices can send messages when things don't go well
    - That network you're trying to reach is not reachable from here
    - Your time-to-live expired, just letting you know

## GRE 
- Generic Routing Encapsulation
    - The "tunnel" between two endpoints
- Encapsulate traffic inside of IP
    - Two endpoints appear to be directly connected to each other
    - No built-in encryption

## VPNs
- Virtual Private Networks
    - Encrypted (private) data traversing a public network
- Concentrator
    - Encryption/decryption access device 
    - Often integrated into a firewall
- Many deployment options
    - Specialized cryptographic hardware
    - Software-based options available
- Used with client software
    - Sometimes built into the OS

## IPSec (Internet Protocol Security)
- Security for OSI Layer 3
    - Authentication and encryption for every packet
- Confidentiality and integrity/anti-replay
    - Encryption and packet signing
- Very standardized
    - Common to use multi-vendor implementations
- Two core IPSec protocols
    - Authentication Header (AH)
    - Encapsulation Security Payload (ESP)

## Transport mode and tunnel mode

[![Transport mode and tunnel mode]({{site.baseurl}}/img/transport_mode_and_tunnel_mode.png)](https://youtu.be/K0o4XDkDRHA?si=TrNahu1JdJUXHL9i&t=235){:target="_blank"}

## Authentication Header (AH)
- Hash of the packet and a shared key
    - MD5, SHA-1, or SHA-2 are common
    - Adds the AH to the packet header

[![Authentication Header (AH)]({{site.baseurl}}/img/authentication_header.png)](https://youtu.be/K0o4XDkDRHA?si=oERPrOvaKZVYOhEP&t=315){:target="_blank"}

## Encapsulation Security Payload (ESP)
- Encrypts the packet
    - MD5, SHA-1, or SHA-2 for hash, and 3DES or AES for encryption
    - Adds a header, a trailer, and an Integrity Check Value

[![Encapsulation Security Payload (ESP)]({{site.baseurl}}/img/encapsulation_security_payload.png)](https://youtu.be/K0o4XDkDRHA?si=oERPrOvaKZVYOhEP&t=315){:target="_blank"}

## IPsec Transport mode and Tunnel mode

[![IPsec Transport mode and Tunnel mode]({{site.baseurl}}/img/ipsec_transport_mode_and_tunnel_mode.png)](https://youtu.be/K0o4XDkDRHA?si=oERPrOvaKZVYOhEP&t=315){:target="_blank"}
