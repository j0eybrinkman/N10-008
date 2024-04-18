---
title: Virtual Networks - N10-008 CompTIA Network+ &#58; 1.2
author: Joey
tags:
  - Networking Concepts
  - Virtual Networks
  - Professer Messer 
layout: post
date: 2024-04-17 17:07:07 -0500
---

<div class="container">
    <iframe class="responsive-iframe" width="560" height="315" src="https://www.youtube.com/embed/A29g5-Os-u8?si=ykwld7QpDsHeALeX" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
</div>
[Virtual Networks - N10-008 CompTIA Network+ : 1.2](https://www.professormesser.com/network-plus/n10-008/n10-008-video/virtual-networks/){:target="_blank"}

## Virtual Networks

- Server farm with 100 individual computers
  - It's a big farm
- All servers are connected with enterprise switches and routers
  - With redundancy
- Migrate 100 physical servers to one physical server
  - With 100 virtual servers inside

## Network Function Virtualization (NFV)
- Replace physcial network devices with virtual versions
  - Manage from the hypervisor
- Same functionality as a physical device
  - Routing, switching, load balancing, firewalls, etc.
- Quickly and easily deploy network functions
  - Click and deploy from the hypervisor
- Many different deployment options
  - Virtual machine, container, fault tolerance, etc.

## The Hypervisor 

- Virtual Machine Manager
  - Manages the virtual platform and guest operating systems
- Hardware management
  - CPU
  - Networking
  - Security
- Single console control
  - One pane of glass
- vSwitch
  - Virtual switch
  - Move the physical switch into the virtual environment
- Functionality is similar to a physical switch
  - Forwarding options
  - Link aggregation
  - Port mirroring
  - NetFlow
- Deploy from the hypervisor
  - Automate with orchestration

## Virtual Network Interface Card (vNIC)
  - A virtual machine needs a network interface
    - A vNIC
  - Configured and connected through the hypervisor
    - Enable additional features 
    - VLAN, aggregation, multiple interfaces