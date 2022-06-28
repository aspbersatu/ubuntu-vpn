# Ubuntu VPN <img src="https://img.shields.io/badge/Markdown-000000?style=flat&logo=markdown&logoColor=white"/>
<p align="center">
<b>Shell autoscript for multiple VPN user menu installation on Ubuntu server</b>
</p>
<p align="center">
<img src="https://img.shields.io/badge/Shell_Script-121011?style=for-the-badge&logo=gnu-bash&logoColor=white"/>
<img src="https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black"/>
<img src="https://img.shields.io/badge/Ubuntu-20.04 LTS-informational?style=for-the-badge&labelColor=E95420&logo=ubuntu&logoColor=white"/>
</p>

## Prerequisites
1. A virtual private server (VPS) running **Ubuntu 20.04**. You can rent servers from providers such as **[UpCloud](https://upcloud.com/signup/?promo=8X94J9)**.

2. Your own **domain name**, which may be free or paid.

3. A **DNS type `A` record** pointing from the fully qualified domain name of your server to the server’s IP address.

> _If you are using **Cloudflare**, note that some Xray configurations require **DNS services only** and will not work with proxying._

## Recommendation
<p align="center">
<img src="https://img.shields.io/badge/Upcloud_Server-Sign?style=for-the-badge&color=purple&logo=upcloud&logoColor=white"/>
<img src="https://img.shields.io/badge/Linux-KVM-green?style=for-the-badge&labelColor=blue&logo=tryhackme&logoColor=white"/>
</p>

Sign up for a free 3-day trial and get a free **$25 credit**. You also will get a free access to a simple plan Linux cloud server with **1 GB Memory**, **1 CPU**, **25GB Storage**, and **1TB Transfer**.

> _Please note that during the trial, you need to making deposit at least **$10** to your account and then you can enjoy this total **$35** for lifetime in your UpCloud account._

Click here to > **[Sign Up](https://upcloud.com/signup/?promo=8X94J9)**

## Information
**1. List of VPN server:**

| Installed VPN Server | Port |
| :---: | :---: |
| OpenVPN (TCP) | 1194 |
| OpenVPN (UDP) | 1194 |
| Xray Vless (XTLS) | 443 |
| Xray Vless (WS) | 80 |
| WireGuard Server | 51820 |

<br>

**2. List of services:**

| Installed Services | Port |
| :--- | :---: |
| Dropbear | 85 |
| Stunnel | 465 |
| Squid Proxy | 8080 |
| OHP Server (Dropbear) | 3128 |
| OHP Server (OpenVPN) | 8000 |
| BadVPN UDPGW | 7300 |
| Nginx | 80 |
| Speedtest CLI | - |
| Fail2Ban | - |
| DDoS Deflate | - |
| rc-local | - |
| vnstat | - |

## Installation
1. Download autoscript
```bash
wget https://raw.githubusercontent.com/skynetcenter/meta-vpn/main/autoscript.sh
```

2. Execute and run autoscript
```bash
chmod +x autoscript.sh && ./autoscript.sh
```
