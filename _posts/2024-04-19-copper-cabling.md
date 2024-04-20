---
title: Copper Cabling - N10-008 CompTIA Network+ &#58; 1.3
author: Joey
tags:
  - Section 1&#58; Networking Concepts
  - 1.3 Cables and Connectors
  - Copper Cabling
  - Professer Messer 
layout: post
date: 2024-04-19 19:21:15 -0500
---
 
<div class="container">
  <iframe class="responsive-iframe" width="560" height="315" src="https://www.youtube.com/embed/UO57e6cv5SA?si=rMjrR84HM9xPIgK3" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
</div>
[Copper Cabling - N10-008 CompTIA Network+ : 1.3](https://www.professormesser.com/network-plus/n10-008/n10-008-video/copper-cabling-3/){:target="_blank"}

## The Importance of Cable
- Fundamental to network communication
  - Incredibly important function
- Usually only get one good opportunity at building cabling infrastructure
  - Make it good!
- The vast majority of wireless communication uses cables 
  - Unless you're an amateur radio operator

## Twisted Pair Copper Cabling
- Balance pair operation
  - Two wires with equal and opposite signals
  - Transmit+, Transmit- / Receive+, Receive-
- The twist is the secret!
  - Keeps a single wire constantly moving away from interference
  - The opposite signals are compared on the other end
- Pairs in the same cable have different twist rates

## Copper Cable Categories

| Ethernet Standard | Cable Category             | Maximum Supported Distance                 |
|-------------------|----------------------------|--------------------------------------------|
| 1000BASE-T        | Category 5                 | 100 meters                                 |
| 1000BASE-T        | Category 5e (enhanced)     | 100 meters                                 |
| 10GBASE-T         | Category 6                 | Unshielded: 55 meters Shielded: 100 meters |
| 10GBASE-T         | Category 6A (augmented)    | 100 meters                                 |
| 10GBASE-T         | Category 7 (Shielded only) | 30 meters                                  |
| 40GBASE-T         | Category 8 (Shielded only) | 30 meters                                  |

## Coaxial Cables
- Two or more forms share a common axis
- RG-6 used in television/digital cable
  - And high-speed Internet over cable

## Twinaxial Cable
- Two inner conductors
  - Twins
- Common on 10 Gigabit Ethernet SFP+ cables
  - Full duplex
  - Five meters
  - Low cost
  - Low latency compared to twisted pair

## Structured Cabling Standards
- International ISO/IEC 11801 cabling standards
  - Defines classes of networking standards
- Telecommunications Industry Association (TIA)
  - Standards, market analysis, trade shows, governmetn affairs, etc.
  - ANSI/TIA-568: Commercial Building Telecommunications Cabling Standard
    - [http://www.tiaonline.org](http://www.tiaonline.org){:target="_blank"}
  - Commonly referenced for pin and pair assignments of eight-conductor 100-ohm balanced twisted pair cabling
  - T568A and T568B

## T568A and T568B Termination
- Pin assignments from T568-B standard
  - Eight conductor 100-ohm balanced twisted-pair cabling
- T568A and T568B are different pin assignments for 8P8C connectors
  - Assigns the T568A pin-out to horizontal cabling
- Many organizations traditionally use 568B
  - Difficulty to change in mid-stream
- You can't terminate one side of the cable with 568A and the other with 568B
  - You'll most likely run into confusion and technical problems

[![568A and 568B termination](/img/568A_568B_graphic.png)](https://youtu.be/UO57e6cv5SA?si=MCfuOXzh_gm56_MZ&t=471){:target="_blank"}