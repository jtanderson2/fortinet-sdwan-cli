# Fortinet SD-WAN CLI

## Overview

FortiManager is great (and recommended) for deploying and managing Fortinet SD-WAN, particularly for large environments. However, SD-WAN can be configured on the FortiGates via the GUI or CLI without any centralised management. This article describes configuring a small SD-WAN deployment using only the CLI.

This is not a full explanation of Fortinet SD-WAN technology and features; please see the official documentation here.
https://docs.fortinet.com/document/fortigate/7.4.6/administration-guide/19246/sd-wan

## Design Details

* Single Hub, 2 Spokes
* ADVPN
* Dual internet underlay at all sites
* DHCP on internet facing interfaces
* BGP dynamic routing in Overlay, using 'BGP on loopback' design
* ANY outbound internet access permitted from LANs at all sites
* ANY-to-ANY access permitted between LANs at all sites

### Diagrams

![](media/sdwan-cli.png)








