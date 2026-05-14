\# VeilNet Architecture



\## Overview



VeilNet is a Raspberry Pi-based DNS filtering and private infrastructure appliance built using Docker, AdGuard Home, and Tailscale.



\## Network Flow



Devices

↓

Tailscale / Local Network

↓

VeilNet Raspberry Pi

↓

AdGuard Home

↓

Encrypted Upstream DNS (DoH)

↓

Internet



\## Core Components



\### Raspberry Pi

Hosts the VeilNet infrastructure stack.



\### Docker

Provides containerized deployment and service isolation.



\### AdGuard Home

Handles DNS filtering, query logging, and upstream DNS forwarding.



\### Tailscale

Provides encrypted remote mesh connectivity to the appliance.



\### Encrypted Upstream DNS

Uses DNS-over-HTTPS providers such as Quad9 and Cloudflare.

