---
title: IPv6 Addressing - N10-008 CompTIA Network+ &#58; 1.4
author: Joey
tags:
  - Section 1&#58; Networking Concepts
  - 1.4 IPv6 Addressing
  - IP Subnetting
  - Professer Messer 
layout: post
date: 2024-05-07 12:12:00 -0500
---

<div class="container">
    <iframe class="responsive-iframe" width="560" height="315" src="https://www.youtube.com/embed/mCo7Zg_0PP0?si=GVT_CTVMPvjkmlF9" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
</div>
[IPv6 Addressing - N10-008 CompTIA Network+ : 1.4](https://www.professormesser.com/network-plus/n10-008/n10-008-video/ipv6-addressing-n10-008/){:target="_blank"}

## IPv6 addresses
- Internet Protocol v6 - 128-bit address
- 340,282,366,920,938,463,463,374,607,431,768,211,456 addresses (340 undecillion)
- 6.8 billion people could have 5,000,000,000,000,000,000,000,000,000 addresses each

[![Subnet masks and subnets]({{site.baseurl}}/img/ipv6_addresses.png)](https://youtu.be/mCo7Zg_0PP0?si=bpgKtvrWq6TVjgvL){:target="_blank"}

- Your DNS will become very important!

## IPv6 address compression
- Groups of zeros can be abbreviated with a double colon
    - Only one of these abbreviations allowed per address
- Leading zeros are optional
- Full IPv6 Address
    - 2600:DDDD:1111:0001:0000:0000:0000:0001
- Abbreviated IPv6 Address
    - 2600:DDDD:1111:1::1

[![IPv6 address compression]({{site.baseurl}}/img/ipv6_shorthand.png)](https://youtu.be/mCo7Zg_0PP0?si=bpgKtvrWq6TVjgvL){:target="_blank"}

- Full IPv6 Address
    - 2601:04C3:4002:BE00:0000:0000:0000:0066
- Abbreviated IPv6 Address
    - 2601:4C3:4002:BE00::66

[![IPv6 address compression ex 1]({{site.baseurl}}/img/ipv6_shorthand_1.png)](https://youtu.be/mCo7Zg_0PP0?si=bpgKtvrWq6TVjgvL){:target="_blank"}

## Configuring IPv6 with a modified EUI-64
- Static addressing can be useful
    - The IP address never changes
- What other address never changes?
    - The MAC address
- Extended Unique Identifier (64-bit)
- Combined a 64-bit IPv6 prefix and the MAC address
    - Wait, the MAC address is only 48-bits long!
- You're going to need some extra bits
    - And a minor change to the MAC address

## The MAC address
- Ethernet Media Access Control address
    - The "physical" address of a network adapter\
- EUI-48 address
    - Extended Unique Identifier (48-bit)

[![MAC address]({{site.baseurl}}/img/mac_address.png)](https://youtu.be/mCo7Zg_0PP0?si=bpgKtvrWq6TVjgvL){:target="_blank"}

## Converting EUI-48 to EUI-64
- Split the MAC
    - Two 3-byte (24-bit) halves
- Put FFFE in the middle
    - The missing 16 bits
- Invert the seventh bith
    - Changes the address from globally unique/universal 
    - Turns the burned-in address (BIA) into a locally administered address
    - This is the U/L bit (universal/local)

## Modifying the MAC

[![Modifying the MAC]({{site.baseurl}}/img/modifying_the_mac.png)](https://youtu.be/mCo7Zg_0PP0?si=kaLGN-Krnv0x3jxJ&t=548){:target="_blank"}


## Building the IPv6 address

- The 64-bit IPv6 subnet prefix
- The EUI-64 address

[![Building the IPv6 address]({{site.baseurl}}/img/building_the_ipv6_address.png)](https://youtu.be/mCo7Zg_0PP0?si=4QPyN3xqhlkocUsx&t=602){:target="_blank"}

## Flipping the 7th bit
- Quickly convert the MAC address
    - Create a chart
- Count from 0 to F in hex
    - Two columns, groups of four
- Quickly convert the second character of the first hex byte
    - Change it to another value

[![Flipping the 7th bit]({{site.baseurl}}/img/flipping_the_7th_bit.png)](https://youtu.be/mCo7Zg_0PP0?si=4QPyN3xqhlkocUsx&t=602){:target="_blank"}

## Quick Conversions

[![Quick Conversions]({{site.baseurl}}/img/quick_conversions.png)](https://youtu.be/mCo7Zg_0PP0?si=AyrSB5LmnqG04zjd&t=757){:target="_blank"}





