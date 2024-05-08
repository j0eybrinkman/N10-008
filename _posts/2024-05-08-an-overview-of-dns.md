---
title: An Overview of DNS - N10-008 CompTIA Network+ &#58; 1.6
author: Joey
tags:
  - Section 1&#58; Networking Concepts
  - 1.6 An Overview of DNS
  - Network Services
  - Professer Messer 
layout: post
date: 2024-05-08 10:19:00 -0500
---

<div class="container">
    <iframe class="responsive-iframe" width="560" height="315" src="https://www.youtube.com/embed/LNGOkJPd5pM?si=xrLlLdhymY1iYryp&amp;start=100" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
</div>
[DHCP Overview - N10-008 CompTIA Network+ : 1.6](https://www.professormesser.com/network-plus/n10-008/n10-008-video/dhcp-overview-n10-008/#google_vignette){:target="_blank"}

## Domain Name System
- Translates human-readable names into computer-readable IP addresses
    - You only need to remember www.professormesser.com
- Hierarchial
    - Follow the path
- Distributed database
    - Many DNS servers
    - 13 root server clusters (Over 1,000 actual servers)
    - Hundreds of generic top-level domain (gTLDs) - .com, .org, .net, etc.
    - Over 275 country code top-level domains (ccTLDs) - .us, .ca, .uk, etc.

## The DNS hierarchy
[![The DNS hierarchy]({{site.baseurl}}/img/the_dns_hierarchy.png)](#){:target="_blank"}

## Fully Qualified Domain Name
[![Fully Qualified Domain Name]({{site.baseurl}}/img/fqdn.png)](#){:target="_blank"}

## Internal vs external DNS
- Internal DNS 
    - Managed on internal servers
    - Configured and maintained by the local team
    - Contains DNS information about internal devices
    - DNS service on Windows Server
- External DNS
    - Often Managed by a third-party
    - Does not have internal device information
    - Google DNS, Quad9

## Recursive and iterative DNS queries
- Many ways to get what you need
- Recursive query
    - Delegate the lookup to a DNS server
    - The DNS server does the work and reports back
    - Large DNS cache provides a speed advantage
- Iterative query
    - Do all of the queries yourself 
    - Your DNS cache is specific to you

## Recursive DNS query
[![Recursive DNS query]({{site.baseurl}}/img/recursive_dns_query.png)](#){:target="_blank"}

## Iterative DNS query
[![Iterative DNS query]({{site.baseurl}}/img/iterative.png)](#){:target="_blank"}

## The authority
- Authorative
    - The DNS server is the authority for the zone
- Non-authoritative
    - Does not contain the zone source files
    - Probably cached information 
- TTL (time to live)
    - Configured on the authoritative server
    - Specifies how long a cache is valid
    - A very long TTL can cause problems if changes are made

## Lookups 
- Forward lookup 
    - Provide the DNS server with an FQDN
    - DNS server provides an IP address
- Reverse DNS
    - Provide the DNS server with an IP address
    - The DNS server provides an FQDN