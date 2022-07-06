# Security & privacy advices for your home network
## Router configuration
- Change default passwords (for a secure one)
- Use the strongest authentication method (WPA3 if it's supported)
- Disable UPnP (if it's not necessary)
- Disable WPS
- Change the default DNS server (Cloudflare has a malware-blocking one, or you can create your own, for example with Pi-hole)
- Use secure DNS
- Use VLANs (with disabled DTP)
- Config firewall
- You can use mail log or something similar (encrypted!)
- MAC-filtering for admin interface (or the whole network)
- Keep remote admin disabled (this is the default setting)
- Sometimes check connected devices

## Firewalls & IPS
- [pfSense](https://www.pfsense.org/) - open-source firewall
- [Pi-hole](https://pi-hole.net/) - DNS-proxy, used to filter ads & suspicious sites (also open-source)
- [Snort](https://www.snort.org/) - open-source IPS

## Remote access tools
- [OpenVPN](https://openvpn.net/) - open source VPN system
- [WireGuard](https://www.wireguard.com/) - lightweight VPN-tunnel, can be faster than OpenVPN (open-source as well)