---
title: Classful Subnetting - N10-008 CompTIA Network+ &#58; 1.4
author: Joey
tags:
  - Section 1&#58; Networking Concepts
  - 1.4 Classful Subnetting
  - IP Subnetting
  - Professer Messer 
layout: post
date: 2024-05-06 09:10:00 -0500
---

<div class="container">
    <iframe class="responsive-iframe" width="560" height="315" src="https://www.youtube.com/embed/Q3wYfb3jnE8?si=mz7aRagZ8nzMhGGr" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
</div>
[Classful Subnetting - N10-008 CompTIA Network+ : 1.4](https://www.professormesser.com/network-plus/n10-008/n10-008-video/classful-subnetting-n10-008/){:target="_blank"}

## Classful Subnetting
- Very specific subnetting architecture
    - Not used since 1993
        - But still referenced in casual conversation
- Used as a starting point when subnetting
    - Standard values

[![Classful Subnetting]({{site.baseurl}}/img/classful_subnetting.png)](https://youtu.be/Q3wYfb3jnE8?si=KDcGwOn-F8TmzfvZ&t=67){:target="_blank"}

## Subnet classes

[![Classful Subnetting]({{site.baseurl}}/img/subnet_classes.png)](https://youtu.be/Q3wYfb3jnE8?si=5IZBWMpdXbHRuyEM&t=84){:target="_blank"}

## What IP class?

[![Classful Subnetting]({{site.baseurl}}/img/what_ip_class.png)](https://youtu.be/Q3wYfb3jnE8?si=BTZj_zgc2duXSkLS&t=299){:target="_blank"}

## The Construction of a subnet
- Network address
    - The first IP address of a subnet
    - Set all host bits to 0 (0 decimal)
    - First usable host address
        - One number higher than the network address
    - Network broadcast address
        - The last IP address of a subnet
        - Set all host bits to 1 (255 decimal)
    - Last usable host address
        - One number lower than the broadcast address

## Subnet calculations (ex 1)
- IP address: 10.74.222.11
    - Class A
    - Subnet mask 255.0.0.0
    - Network address (set all host bits to 0) 10.0.0.0
    - First usable host address (add one) 10.0.0.1
    - Network Broadcast Address (Set all host bits to 1) 10.255.255.255
    - Last usable host address (minus one) 10.255.255.254

[![Classful Subnetting calculation ex1]({{site.baseurl}}/img/subnet_calcultions_ex1.png)](https://youtu.be/Q3wYfb3jnE8?si=7PfnJdyVHBSyEBQs&t=524){:target="_blank"}

## Subnet calculations (ex 2)
- IP address: 172.16.88.200
    - Class B
    - Subnet mask: 255.255.0.0
    - Network address: 172.16.0.0
    - First usable host address: 172.16.0.1
    - Network broadcast address: 172.16.255.255
    - Last usable host address: 172.16.255.254

[![Classful Subnetting calculation ex2]({{site.baseurl}}/img/subnet_calcultions_ex2.png)](https://youtu.be/Q3wYfb3jnE8?si=gUNeFzus6pC96Sij&t=552){:target="_blank"}

## Subnet calculations (ex 3)
- IP address: 192.168.4.77
    - Class C
    - Subnet mask: 255.255.255.0
    - Network address: 192.168.4.0
    - First usable host address: 192.168.4.1
    - Network broadcast address: 192.168.4.255
    - Lat usable host address: 192.168.4.254

[![Classful Subnetting calculation ex3]({{site.baseurl}}/img/subnet_calcultions_ex3.png)](https://youtu.be/Q3wYfb3jnE8?si=gUNeFzus6pC96Sij&t=552){:target="_blank"}
