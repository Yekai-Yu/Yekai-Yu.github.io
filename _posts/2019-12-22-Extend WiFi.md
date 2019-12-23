---
layout: post
title: Extend WiFi
---

I am thinking about extending WiFi coverage at home.

The current configuration has only one wireless router to broadcast signal in a two-story condo. The signal degrades badly after going through only one wall.

There are two solutions I am thinkin'

- Using old wireless routers as AP by cable-connecting to the main router.
- Wirelessly using the repeater bridge, but I am not sure if I have any of those at home.

So, first __reset__ the device

- AP: need long cables and routing around the house
  - look up the IP address ip1 of the primary router R1
  - disconnect Internet and connect the old router R2 to computer by cable directly (LAN only)
  - switch to AP mode, probably it was already 
  - change the IP of R2 to any other unoccupied IP (1~254)
  - change the gateway of R2 to ip1
  - DISABLE DHCP of R2 - cuz R1 is running as DHCP already!
  - restart...should be good
- Repeater Bridge: retains the same SSID as R1, while AP solution could differ
  - Some product can automate the setup process
  - For mine, I guess it won't automate
  - switch to Repeater...Bridge...mode? Haven't tried, we will see (TODO: yk!!! Update this later)
  - should be pretty much the same...





Considering the thickness of the wall, I feel I will do the cable-AP way...at least for the kitchen...