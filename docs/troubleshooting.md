\## Invalid Docker Container Name



\### Problem



Docker Compose failed with:

Invalid container name (veilnet/adguard)



\### Cause



Docker container names cannot contain forward slashes (/).



\### Solution



Changed:

container\_name: veilnet/adguard

to:

container\_name: veilnet-adguard













\## ISP Router Prevented Custom DNS Configuration



\### Problem



COX router firmware did not allow changing LAN DNS distribution settings.



\### Impact



Devices could not automatically inherit VeilNet DNS settings through DHCP.



\### Workaround



Configured DNS manually per device and later integrated Tailscale for remote/private DNS access.











\## Safari Private Browsing Filtering Differences



\### Problem



DNS filtering behavior appeared inconsistent in Safari Private Browsing mode on iPhone.



\### Cause



Safari Advanced Tracking and Fingerprinting Protection altered request behavior.



\### Solution



Disabling:

Safari → Advanced → Advanced Tracking and Fingerprinting Protection



restored expected filtering behavior.

