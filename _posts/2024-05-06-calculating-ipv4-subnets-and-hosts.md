---
title: Classful Subnetting - N10-008 CompTIA Network+ &#58; 1.4
author: Joey
tags:
  - Section 1&#58; Networking Concepts
  - 1.4 Calculating IPv4 Subnets and Hosts
  - IP Subnetting
  - Professer Messer 
layout: post
date: 2024-05-06 10:35:00 -0500
---

<div class="container">
    <iframe class="responsive-iframe" width="560" height="315" src="https://www.youtube.com/embed/4kMGs9-HDEk?si=1ZcoFs1M3BVaAmPo" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
</div>
[Calculating IPv4 Subnets and Hosts - N10-008 CompTIA Network+ : 1.4](https://www.professormesser.com/network-plus/n10-008/n10-008-video/calculating-ipv4-subnets-and-hosts-n10-008/){:target="_blank"}

## Why subnet the network?

Its very difficult to connect all devices over the internet under one network, instead we use router to send traffic over manageable and segmented networks. Makes it much simpler to manage.

[![Why subnet the network?]({{site.baseurl}}/img/why_subnet_the_network_diagram.png)](https://youtu.be/4kMGs9-HDEk?si=hnBlijG0A_8aXAJa&t=44){:target="_blank"}

## VLSM (Variable Length Subnet Masks)
- Class-based networks are inefficient
    - The subnet mask is based on the network classes
- Allow network administrators to define their own masks
    - Customize the subnet masks to specific network requirements
- Use different subnet masks in the same classful network
    - 10.0.0.0/8 is the class A network
    - 10.0.1.0/24 and 10.0.8.0/24 would be VLSM

## Defining subnets
- IP address: 10.0.0.0
    - Class A, subnet mask: 255.0.0.0
    - "Classful" addressing

## Calculating subnets and hosts
[![Calculating subnets and hosts]({{site.baseurl}}/img/calculating_subnets_and_hosts.png)](https://youtu.be/4kMGs9-HDEk?si=QDxGPN6N0tRPBp6-&t=297){:target="_blank"}

example 1

[![Calculating subnets and hosts]({{site.baseurl}}/img/calculating_subnets_and_hosts_1.png)](https://youtu.be/4kMGs9-HDEk?si=iVv5o-GK1pjgRU9J&t=376){:target="_blank"}

example 2

[![Calculating subnets and hosts]({{site.baseurl}}/img/calculating_subnets_and_hosts_2.png)](https://youtu.be/4kMGs9-HDEk?si=mdoUBg95EVINBdaE&t=411){:target="_blank"}

example 3

[![Calculating subnets and hosts]({{site.baseurl}}/img/calculating_subnets_and_hosts_3.png)](https://youtu.be/4kMGs9-HDEk?si=CA3u9rIbLkQnhYAc&t=492){:target="_blank"}