---
title: Magic Number Subnetting - N10-008 CompTIA Network+ &#58; 1.4
author: Joey
tags:
  - Section 1&#58; Networking Concepts
  - 1.4 Magic Number Subnetting
  - IP Subnetting
  - Professer Messer 
layout: post
date: 2024-05-06 11:24:00 -0500
---

<div class="container">
    <iframe class="responsive-iframe" width="560" height="315" src="https://www.youtube.com/embed/XMzLpGKTu50?si=yr7DToQ-qZ5m_DCk&amp;start=3" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
</div>
[Magic Number Subnetting - N10-008 CompTIA Network+ : 1.4](https://www.professormesser.com/network-plus/n10-008/n10-008-video/magic-number-subnetting-n10-008/){:target="_blank"}

## Subnetting the network
[![Subnetting the network]({{site.baseurl}}/img/subnetting_the_network.png)](https://youtu.be/XMzLpGKTu50?si=DSgRnd9ijPUuf5sk&t=3){:target="_blank"}

## Calculating subnet masks
- We have four networks with about 40 devices per subnet
[![Calculating subnet masks]({{site.baseurl}}/img/calculating_subnet_masks.png)](https://youtu.be/XMzLpGKTu50?si=8h8On07sn3KwYfi0&t=81){:target="_blank"}

## Subnetting the network

[![Calculating subnet masks]({{site.baseurl}}/img/subnetting_the_network_magic.png)](https://youtu.be/XMzLpGKTu50?si=HLEJZvDYMG0e57lL&t=149){:target="_blank"}

## Four important addresses
- Network address / subnet ID
    - The first address in the subnet
- Broadcast address
    - The last address in the subnet
- First available host address
    - One more than the network address
- Last available host address
    - One less than the broadcast address

## Subnetting the network

[![Subnetting the network]({{site.baseurl}}/img/subnetting_the_network_magic_1.png)](https://youtu.be/XMzLpGKTu50?si=DmVq7k-B1Hr8Zs7s&t=195){:target="_blank"}

## Magic number subnetting
- Very straightforward method
    - Can often perform the math in your head
- Subnet with minimal math
    - Still some counting involved
- Some charts might help
    - But may not be required
    - CIDR to Decimal 
    - Host ranges

## Some helpful charts
- CIDR to decimal chart 
    - Memorization will increase speed

[![CIDR to decimal chart ]({{site.baseurl}}/img/cidr_to_decimal_chart.png)](https://youtu.be/XMzLpGKTu50?si=wE8eMKhbuPu0EcmD&t=249){:target="_blank"}

[![CIDR to decimal chart ]({{site.baseurl}}/img/cidr_to_decimal_chart_1.png)](https://youtu.be/XMzLpGKTu50?si=wE8eMKhbuPu0EcmD&t=249){:target="_blank"}

[![CIDR to decimal chart ]({{site.baseurl}}/img/cidr_to_decimal_chart_2.png)](https://youtu.be/XMzLpGKTu50?si=wE8eMKhbuPu0EcmD&t=249){:target="_blank"}

- Host ranges
    - Larger blocks are easier to remember
    - Multiply quickly for the smaller blocks

[![Host ranges ]({{site.baseurl}}/img/cidr_to_decimal_chart_3.png)](https://youtu.be/XMzLpGKTu50?si=wE8eMKhbuPu0EcmD&t=249){:target="_blank"}

## The magic number process
- Convert the subnet mask to decimal (if necessary)
- Identify the "interesting octet"
- Calculate the "magic number"
    - 256 minus the interesting octet
- Calculate the host range
- Identify the network address
    - First address in range
- Identify the broadcast address
    - Last address in the range

[![Host ranges ]({{site.baseurl}}/img/cidr_to_decimal_chart_4.png)](https://youtu.be/XMzLpGKTu50?si=wE8eMKhbuPu0EcmD&t=249){:target="_blank"}

## Find the broadcast address
- IP address: 165.245.77.14
- Subnet mask: 255.255.240.0
- Subnet ID: 165.245.64.0

- If the mask is 255
    - copy the subnet ID
- If the mask is 0
    - Write 255
- Anything not 255 or zero is the interesting octet

- Subtract the interesting octect mask from 256
    - The magic number is 16 (256-240)
- Calculate Subnet ID + magic number - 1
    - 64 + 16 -1 = 79

[![Broadcast address]({{site.baseurl}}/img/cidr_to_decimal_chart_5.png)](https://youtu.be/XMzLpGKTu50?si=wE8eMKhbuPu0EcmD&t=249){:target="_blank"}
- IP address: 165.245.77.14
- Subnet mask: 255.255.240.0
- Subnet ID: 165.245.64.0
- Broadcast: 165.245.79.255

## Find the host range
- First host is subnet ID +1
    - 165.245.64.1
- The last host is the broadcast - 1
    - 165.245.79.254

## Speeding up the magic
- IP address: 172.16.242.133/27

[![Speeding up the magic]({{site.baseurl}}/img/speeding_up_the_magic.png)](https://youtu.be/XMzLpGKTu50?si=Sq-cdqicKNpmKCYf&t=1019){:target="_blank"}

