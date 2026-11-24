---
layout: post
author: dan
title: Router settings for fibre internet for you own hardware
---

This post seeks to document the custom router settings that are required when you want to use your own hardware for fibre internet in Ireland.

## Vodafone
- Username: vodafone@vodafone.ie
- Password: vodafone
- Encapsulation: PPPoE
- VLAN ID: 10
- Connection Type: Routed PPPoE
- MTU: 1492 (standard for PPPoE)
- DNS: Can be set to automatic, or use public DNS like Google (8.8.8.8 / 8.8.4.4)

Source: 
https://cksolutions.ie/pppoe-details-for-fiber-to-the-home-business-nbi/

## Virgin Media
- VLAN ID: 10
- Mac Address Clone: get the mac address from the device supplied to you by Virgin Media
- IPV4: Leave as DHCP
- DNS: you can use auto, or set your own, e.g. 1.1.1.1 and 1.0.0.1

![alt text]({{ "/assets/images/231126_1117_1014.png" | relative_url }})

Virgin supports IPV6, so you can enable that:

![alt text]({{ "/assets/images/231126_1119_1015.png" | relative_url }})

Source: 
https://shanehastings.eu/blog/bypassing-the-virgin-media-ireland-hub-5x-using-an-xgs-pon-sfp-ont-module