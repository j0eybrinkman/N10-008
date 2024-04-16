---
title: Network Topologies - N10-008 CompTIA Network+ &#58; 1.2
author: Joey
tags:
  - Networking Concepts
  - Network Topologies and Types
  - Professer Messer 
layout: post
date: 2024-04-15 21:38:23 -0500
---

## Network Topologies

- Useful in planning a new network
    - Physical layout of building or campus
- Assists in understanding signal flow
    - Troubleshooting problems

## Star
(A.K.A Hub and spoke)

[![Star Topology]({{site.baseurl}}/img/star-topology.jpg)](https://www.researchgate.net/publication/327897159/figure/fig1/AS:675274681221120@1538009438453/Some-Networks-Implement-a-Local-Ring-Topology-A-star-topology-is-a-LAN-architecture-in.jpg){:target="_blank"}

- Used in most large and small networks
- All devices are connected to a central device
- Switched Ethernet networks
    - The switch is in the middle

## Ring

[![Ring Topology]({{site.baseurl}}/img/ring-topology.svg)](https://svg.template.creately.com/Noe2M9jJsLM){:target="_blank"}

- Used in many popular topologies
    - Token Ring is no longer with us
- Still used in many
    - Metro Area Networks (MANs)
    - Wide Area Networks (WANs)
        - Dual-ring
        - Built-in fault tolerance

## Bus

[![Bus Topology]({{site.baseurl}}/img/bus_topology.png)](https://o.quizlet.com/mWWjIQrz6gd5gfIoeLr9Vw.png){:target="_blank"}

- Early local area networks
    - Coaxial cable was the bus
- Simple, but prone to errors
    - One break in the link disabled the entire network
- Controller Area Network
    - CAN bus
    - Used to connect various sensors and controllers in modern cars

## Mesh

[![Mesh Topology]({{site.baseurl}}/img/mesh-topology.png)](https://miro.medium.com/v2/resize:fit:554/1*SAPDKFI_ff0x4g4_u-0wgg.png){:target="_blank"}

- Multiple links to the same place
    - Fully connected
    - Partially connected
- Redundance, fault-tolerance, load balancing
- Used in wide area networks (WANs) 
- Fully meshed and partially meshed

## Hybrid

[![Hybrid Toplogy]({{site.baseurl}}/img/hybrid-topology.png)](https://media.geeksforgeeks.org/wp-content/uploads/20220616225313/hybrid1.jpg){:target="_blank"}

- A combination of one or more physical topologies
    - Most networks are a hybrid

## Wireless Topologies

- Infrastructure
    - All devices communicate through an access point 
    - The most common wireless communication mode
- Ad hoc networking
    - No pre-existing infrastructure
    - Devices communicate amongst themselves
- Mesh
    - Commonly used with IoT
    - Ad hoc devices work together to form a mesh "cloud"
    - Self form and self heal

