\# VeilNet



VeilNet is a Raspberry Pi-based privacy appliance designed to provide simple, network-wide protection for home users.



\## Core Features



\- DNS filtering using AdGuard Home

\- Dockerized deployment

\- Encrypted upstream DNS (DoH)

\- Tailscale mesh network integration

\- Remote administration capability

\- Raspberry Pi deployment

\- Query logging and observability

\## What VeilNet Is



VeilNet is a local network filtering and privacy appliance.



It helps reduce tracking, block many advertisements, and prevent devices from connecting to known malicious domains.



\## What VeilNet Is Not



VeilNet does not make users anonymous.

VeilNet does not \*\*fully\*\* hide browsing activity from internet service providers.

VeilNet does not replace good cybersecurity practices.



\## Reason for Creation



\- To provide a subscription free, portable device that allows for a "cleaner" and more private web browsing experience. 

\- To learn  basic Linux OS handling on a real machine such as a Raspberry Pi rather than a virtual machine, as well as refining and discovering new IT/networking skillsets.

\- To attempt to create a more "plug and play" device that automates a VPN/Adware Blocker and leaves minimal human interaction. The majority of people are not well versed in hosting their own VPN on their own home machines. Therefore, it is speculated they would rather have a physical object that can simply plug into your computer or router and automate tasks for them.



\## MVP Stack



\- Raspberry Pi 4 (2GB+) or Raspberry Pi 5

\- Raspberry Pi OS Lite 64-bit

\- Docker

\- Docker Compose

\- AdGuard Home

\- Encrypted DNS upstreams

\- TailScale

\- Linux networking tools



\## Architecture



Devices

↓

Tailscale / Local Network

↓

VeilNet Raspberry Pi

↓

AdGuard Home

↓

Encrypted Upstream DNS

↓

Internet



\## Skills Demonstrated



\- Linux system administration

\- Containerized infrastructure deployment

\- DNS architecture and filtering

\- Overlay mesh networking

\- Remote infrastructure management

\- Git/GitHub workflow

\- Infrastructure troubleshooting

\- Documentation and reproducibility



\## Current Limitations



BLUF: Some modern applications and browsers may partially bypass DNS-layer filtering through encrypted DNS, hardcoded endpoints, or first-party content delivery systems. VeilNet improves DNS privacy and filtering behavior but is not intended to function as a complete traffic inspection or endpoint security platform.



\- Not a full VPN replacement (i.e. does not provide full "anonymity" like services such as Express VPN)

\- DNS-layer filtering only

\- Modern applications bypass DNS filtering (i.e. YouTube, TikTok, Instagram, Hulu, etc.) due to many modern apps using DoH, encrypted DNS, and private relay systems.

\- Require more manual configuration of DNS IP if internet router is from an ISP that locks out DNS IP manipulation

\- Some smart TVs may not be included if ISP router is unable to have DNS IP manipulated.



\## Future Improvements



&#x20;- SSD migration vice SD card

&#x20;- backup automation

&#x20;- SSH key authentication

&#x20;- Monitoring Improvements

&#x20;- installer automation (i.e. facilitate installer script)

&#x20;- improved onboarding docs



\## Project Status



Version: 0.1

Status: Initial prototype

