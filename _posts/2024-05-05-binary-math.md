---
title: Network Connectors - N10-008 CompTIA Network+ &#58; 1.3
author: Joey
tags:
  - Section 1&#58; Networking Concepts
  - 1.4 Binary Math
  - Network Connectors
  - Professer Messer 
layout: post
date: 2024-05-05 10:21:15 -0500
---

<div class="container">
    <iframe class="responsive-iframe" width="560" height="315" src="https://www.youtube.com/embed/tEv2PKT5Lv8?si=DQJbHIQIdRynGvtk" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
</div>
[Binary Math - N10-008 CompTIA Network+ : 1.4](https://www.professormesser.com/network-plus/n10-008/n10-008-video/binary-math-n10-008/){:target="_blank"}

## Basics of Binary Math
- A bit - a zero or a one
    - One digit. Off or on. 0 or 1.
- A byte - Eight bits
    - Often called an "octet" to avoid ambiguity
- A binary-to-decimal conversion chart

| 128 | 64 | 32 | 16 | 8 | 4 | 2 | 1 |
|-----|----|----|----|---|---|---|---|

## Binary to Decimal 
- What is 00000010 in decimal?
    - answer: 2

| 128 | 64 | 32 | 16 | 8 | 4 | 2 | 1 |
|-----|----|----|----|---|---|---|---|
| 0   | 0  | 0  | 0  | 0 | 0 | 1 | 0 |

- What is 10000010 in decimal?
    - answer: 130

| 128 | 64 | 32 | 16 | 8 | 4 | 2 | 1 |
|-----|----|----|----|---|---|---|---|
| 1   | 0  | 0  | 0  | 0 | 0 | 1 | 0 |

- What is 11111111 in decimal?
    - answer: 255

| 128 | 64 | 32 | 16 | 8 | 4 | 2 | 1 |
|-----|----|----|----|---|---|---|---|
| 1   | 1  | 1  | 1  | 1 | 1 | 1 | 1 |

## Decimal to Binary Conversion

- What is decimal 154 in binary?
    - Start with largest number in chart (Is 128 less than or equal to 154?)
    - answer 10011010

[![Binary to Decimal Conversion]({{site.baseurl}}/img/binary_to_decimal_conversion.png)](https://youtu.be/tEv2PKT5Lv8?si=M_JIdTUdzeJvz3zd&t=394){:target="_blank"}

| 128 | 64 | 32 | 16 | 8 | 4 | 2 | 1 |
|-----|----|----|----|---|---|---|---|
| 1   | 0  | 0  | 1  | 1 | 0 | 1 | 0 |

## More Bits, More Addresses

[![More Bits, More Addresses]({{site.baseurl}}/img/more_bits_more_addresses.png)](https://youtu.be/tEv2PKT5Lv8?si=P6nBGfesbIbC5wTJ&t=431){:target="_blank"}

## Extending the Math
- Powers of two
    - Useful for binary calculations and subnetting

| 2^12 | 2^11 | 2^10 | 2^9 | 2^8 | 2^7 | 2^6 | 2^5 | 2^4 | 2^3 | 2^2 | 2^1 | 2^0 |
|------|------|------|-----|-----|-----|-----|-----|-----|-----|-----|-----|-----|
| 4096 | 2048 | 1024 | 512 | 256 | 128 | 64  | 32  | 16  | 8   | 4   | 2   | 1   |