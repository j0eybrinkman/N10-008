---
title: DHCP Overview - N10-008 CompTIA Network+ &#58; 1.6
author: Joey
tags:
  - Section 1&#58; Networking Concepts
  - 1.6 DHCP Overview
  - Network Services
  - Professer Messer 
layout: post
date: 2024-05-07 18:15:00 -0500
---

<div class="container">
    <iframe class="responsive-iframe" width="560" height="315" src="https://www.youtube.com/embed/ED99yLmMMfw?si=8wTFatlyJzrK5GCY&amp;start=315" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
</div>
[DHCP Overview - N10-008 CompTIA Network+ : 1.6](https://www.professormesser.com/network-plus/n10-008/n10-008-video/dhcp-overview-n10-008/){:target="_blank"}

## DHCP
- IPv4 address configuration used to be manual
    - IP address, subnet mask, gateway, DNS servers, NTP servers, etc.
- October 1993 - The bootstrap protocol
    - BOOTP
- BOOTP didn't automatically define everything
    - Some manual configurations were still required
    - BOOTP also didn't know when an IP address might be available again
- Dynamic Host Configuration Protocol
    - Initially released in 1997, updated through the years
    - Provides automatic address / IP configuration for almost all devices

## Step 1: Discover
[![Step 1: Discover]({{site.baseurl}}/img/step1_discover.png)](https://youtu.be/ED99yLmMMfw?si=l4treoXWyowzk04F&t=100){:target="_blank"}

## Step 2: Offer
[![Step 2: Offer]({{site.baseurl}}/img/step2_offer.png)](https://youtu.be/ED99yLmMMfw?si=l4treoXWyowzk04F&t=100){:target="_blank"}

## Step 3: Request
[![Step 3: Request]({{site.baseurl}}/img/step3_request.png)](https://youtu.be/ED99yLmMMfw?si=l4treoXWyowzk04F&t=100){:target="_blank"}

## Step 4: Acknowledgement
[![Step 4: Acknowledgement]({{site.baseurl}}/img/step4_acknowledgement.png)](https://youtu.be/ED99yLmMMfw?si=l4treoXWyowzk04F&t=100){:target="_blank"}

## Managing DHCP in the enterprise
- Limited Communication range
    - Uses the IPv4 broadcast domain
    - Stops at the router
- Multiple servers needed for redundancy
    - Across different locations
- Scalability is always an issue
    - May not want (or need) to manage DHCP servers at every remote location
- You're going to need a litte help(er)
    - Send DHCP request across broadcast domains

## DHCP relay
[![DHCP relay]({{site.baseurl}}/img/dhcp_relay.png)](https://youtu.be/ED99yLmMMfw?si=l4treoXWyowzk04F&t=100){:target="_blank"}

## Discover with DHCP relay
[![Discover with DHCP relay]({{site.baseurl}}/img/discover_with_dhcp_relay.png)](https://youtu.be/ED99yLmMMfw?si=l4treoXWyowzk04F&t=100){:target="_blank"}

[![Discover with DHCP relay]({{site.baseurl}}/img/discover_with_dhcp_relay1.png)](https://youtu.be/ED99yLmMMfw?si=l4treoXWyowzk04F&t=100){:target="_blank"}

## Offer with DHCP relay
[![Discover with DHCP relay]({{site.baseurl}}/img/offer_with_dhcp_relay.png)](https://youtu.be/ED99yLmMMfw?si=l4treoXWyowzk04F&t=100){:target="_blank"}
[![Discover with DHCP relay]({{site.baseurl}}/img/offer_with_dhcp_relay1.png)](https://youtu.be/ED99yLmMMfw?si=l4treoXWyowzk04F&t=100){:target="_blank"}


