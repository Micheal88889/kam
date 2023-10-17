# Project KA

## Installed Services
|No.|Service|Port|Note|
|---|---|---|---|
|1|Dropbear|85|-|
|||465|TLS|
|2|dnstt|53|UDP|
|||853|TLS|
|3|UDP Custom|1-65535|Excluded ports: 7300, 53, 5300, 1194, 51820|
|4|BadVPN UDPgW|7300|-|
|5|Squid Proxy|8080|-|
|6|Open HTTP Puncher|3128|Dropbear|
|||3129|Dropbear (TLS)|
|||8000|OpenVPN|
|7|Python Proxy|8888|Dropbear|
|||8889|Dropbear (TLS)|
|||8989|OpenVPN|
|8|OpenVPN|194|TCP|
|||1194|UDP|
|9|WireGuard|51820|-|
|10|Xray Core|443|TLS|
|||80|HTTP|
|11|Nginx|443|TLS|
|||80|HTTP|
|12|Stunnel|465|Dropbear|
|||853|dnstt|
|||3129|Open HTTP Puncher|
|||8889|Python Proxy|
|||990|OpenVPN|

## Other Services
- Disable IPv6
- Enable BBR
- Time zone set to Asia/Kuala_Lumpur (GMT +8)
- Reset iptables
- Speedtest CLI
- Fail2Ban
- DDoS Deflate
- Vnstat
- Neofetch





## Installation
1. Update packages and reboot.
	```bash
	apt update && apt upgrade -y && apt install -y screen curl wget && reboot
	```
2. Run installation.
	```bash
	wget -O install.sh "https://raw.githubusercontent.com/iriszz1/kamui/main/install.sh" && chmod +x install.sh && screen ./install.sh
	```

	```bash
	wget -O install.sh "https://raw.githubusercontent.com/Micheal88889/kam/main/install.sh" && chmod +x install.sh && screen ./install.sh
	```
