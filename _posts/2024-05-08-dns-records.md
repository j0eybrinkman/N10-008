---
title: DNS Record Types - N10-008 CompTIA Network+ &#58; 1.6
author: Joey
tags:
  - Section 1&#58; Networking Concepts
  - 1.6 DNS Record Types
  - Network Services
  - Professer Messer 
layout: post
date: 2024-05-08 11:00:00 -0500
---

<div class="container">
    <iframe class="responsive-iframe" width="560" height="315" src="https://www.youtube.com/embed/NijONS9gMZ0?si=ETz5gUDQQ1T5cpA9&amp;start=100" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
</div>
[DNS Record Types - N10-008 CompTIA Network+ : 1.6](https://www.professormesser.com/network-plus/n10-008/n10-008-video/dns-record-types-n10-008/){:target="_blank"}

## DNS records
- Resource Records (RR)
    - The database records of domain name services
- Over 30 record types
    - IP addresses, certificates, host alias, etc.

## Sample forward lookup file
[![The DHCP lease process]({{site.baseurl}}/img/sample_forward_lookup_file.png)](#){:target="_blank"}

## Start of Authority (SOA)
- Describes the DNS zone details
- Structure 
    - In SOA (Internet zone, Start of Authority) with name of zone
    - Serial number
    - Refresh, retry, and expiry timeframes
    - Caching duration/TTL (Time To Live)j

## Address records (A)(AAAA)
- Defines the IP address of a host
    - This is the most popular query
- A records are for IPv4 addresses
    - Modify the A record to change the host name to IP address resolution
- AAAA records are for IPv6 addresses
    - The same DNS server, different records

## Canonical Name Records (CNAME)
- A name is an alias of another, canonical name
    - One physical server, multiple services

## Service records (SRV)
- Find a specific service
    - Where is the Windows Domain Controller?
    - Where is the instant messaging server?
    - Where is the VoIP controller?

## Mail exchanger record (MX)
- Determines the host name for the mail server
    - This isn't an IP address; it's a name

## Name server records (NS)
- List the name servers for a domain
    - NS records point to the name of the server

## Pointer record (PTR)
- The reverse of an A or AAAA record
    - Added to a reverse map zone file

## Text records (TXT)
- Human-readable text information
    - Useful public information
- SPF protocol (Sender Policy Framework)
    - Prevent mail spoofing
    - Mail servers check that incoming mail really did come from an authorized host
- DKIM (Domain Keys Identified Mail)
    - Digitally sign your outgoing mail
    - Validated by the mail server, not usually seen by the end user
    - Put your public key in the DKIM TXT record

## Zone transfers
- Replicate a DNS database
    - The primary DNS server has the primary copy of the zone information
- Synchronize to a secondary server
    - Provide redundancy 
- Triggered by referencing the serial number 
    - If the serial number increases, there must have been a change
- Full zone transfers can be a security risk
    - Attackers can use the data as reconnaissance