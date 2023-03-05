# unifi-tailscale-ip-rule-monitor
debian package for a daemon that reconciles an ip route rule for running Tailscale on the UDM line of products versions 2.x and later

## How To Install & Use Tailscale On Your Unifi UDM (Pro/SE) 

#### Prerequisites

- Your UDM MUST be upgraded to software version 2.x or newer. 
    They switched to a debian stretch based underlying system with systemd and this is critical!

#### Steps

1. Follow at least the first two steps of the Tailscale installation guide for debian stretch:
     https://tailscale.com/kb/1042/install-debian-stretch/
2. Click on releases on the right side of this repository page and download the .deb file from the latest release
3. Copy it to your UDM e.g. over SSH with scp or wget the download url directly on your UDM
4. Install with dpkg, `dpkg -i unifi-tailscale-ip-rule-monitor-*.deb`