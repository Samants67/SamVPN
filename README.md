<div align="center">

<img src="https://raw.githubusercontent.com/iiviirv/irnova-site/main/brand/nova-logo-gradient.svg" width="70" alt="SamVPN">

<div align="right">
  <a href="README.fa.md">🇮🇷 فارسی</a>
</div>

# 🌟 SamVPN Project

**SamVPN - Developed by Saman Taghavi (samants)**

A practical graphical panel to provide Worker subscriptions with VLESS, Trojan, and Warp proxies along with proxy chaining, full DNS settings, clean IP, and advanced routing for users of all platforms using Amnezia, Wireguard, Sing-box, Clash/Mihomo, and Xray cores.

[![License](https://img.shields.io/badge/license-MIT-green?style=for-the-badge)](LICENSE)
[![Version](https://img.shields.io/badge/version-3.6.3-blueviolet?style=for-the-badge)](#)

</div>

---

## 🌐 Contact Links

<div align="center">

[![Telegram](https://img.shields.io/badge/✈️%20Telegram-@irants67-0ea5e9?style=for-the-badge&logo=telegram)](https://t.me/irants67)

</div>

---

## 📖 What is SamVPN?

SamVPN is an **all-in-one personal anti-censorship proxy** that runs completely on Cloudflare Workers using the **Free Plan**. It combines a powerful proxy engine (VLESS, Trojan, Shadowsocks over WebSocket/gRPC/XHTTP) with a **comprehensive dual-language management panel** in a single Worker.

**What makes SamVPN different:**
- ⚡ **No Infrastructure Needed** — No VPS, no domain required to start.
- 🌍 **Clean IP per ISP** — Automatic optimization tailored for each Iranian network operator.
- 👥 **Multi-user Support** — Dedicated subscription links with traffic quotas, expiration dates, and toggle controls.
- 🤖 **Telegram Bot** — Complete control and management via Telegram.
- 🔗 **Proxy Chaining** — Support for SOCKS5, HTTP, HTTPS, TURN, SSTP.
- 🛡️ **Advanced Bypass** — ECH, TLS fragment, 0-RTT, fingerprinting.
- 🧩 **Backend Mode** — Connect to a personal Xray/sing-box VPS for native VLESS + video/voice calling support.

---

## ⚡ Quick Setup

After forking or uploading the code to your repository, you can customize the configuration based on the `wrangler.jsonc` documentation and deploy it using Wrangler commands.

---

## 🛰 Backend Mode (VLESS + Video/Voice Calls)

Cloudflare Workers cannot run native TCP proxies or handle UDP traffic directly. To enable these features, SamVPN supports **Backend Mode** — forwarding traffic to a personal Xray or sing-box VPS.

---

## 📋 Prerequisites

- A **Cloudflare Account** (Free tier) with Workers enabled.
- A **KV Namespace** (automatically created with auto-deploy or manually via Wrangler).
- (Optional) Node.js v18+ and Wrangler CLI for local testing.

---

## 🧬 SamVPN Admin Panel Features

| Feature | Status |
|--------|:--:|
| Auto subscription link generation | ✅ |
| Base64 format export | ✅ |
| Clash / Mihomo support | ✅ |
| sing-box support | ✅ |
| Loon support | ✅ |
| Surge support | ✅ |
| Load Balancing | ✅ |
| Health Check | ✅ |
| Ping test | ✅ |
| Best config selection | ✅ |
| QR Code generation | ✅ |
| Display config list | ✅ |
| DoH proxy | ✅ |
| DNS encryption | ✅ |
| Load Balance / Failover / Caching DNS | ✅ |
| Local DNS bypass | ✅ |
| Anti-Sanction DNS | ✅ |
| Fake DNS / IP | ✅ |
| Routing / GeoIP / GeoSite | ✅ |
| Domestic Bypass (Direct connection to Iranian sites) | ✅ |
| IPv6 support | ✅ |
| AdBlock + PornBlock | ✅ |
| Cloudflare custom ports | ✅ |
| Trojan direct link | ✅ |
| Clash direct link | ✅ |
| Global SOCKS5 mode | ✅ |
| Global HTTP mode | ✅ |
| Clean Cloudflare IP scanner | ✅ |
| Telegram notifications | ✅ |
| Telegram bot management | ✅ |
| Quantumult X support | ✅ |
| Mixed Auto-client detection | ✅ |
| Random Path / Wildcard Host | ✅ |
| Persian RTL responsive Admin dashboard | ✅ |
| Simple + Advanced mode toggle | ✅ |
| Dark mode | ✅ |
| JSON Config Editor | ✅ |
| Log Viewer | ✅ |
| Reset configuration | ✅ |
| VLESS + Trojan + Shadowsocks | ✅ |
| gRPC + XHTTP transport | ✅ |
| WebSocket Early Data | ✅ |
| mux=0 for Shadowsocks | ✅ |
| SOCKS5 chain | ✅ |
| HTTP/HTTPS CONNECT chain | ✅ |
| TURN + SSTP chain | ✅ |
| Global HTTPS / TURN / SSTP mode | ✅ |
| Whitelist domains | ✅ |
| Chain in subscription link | ✅ |
| TLS 1.3 / 1.2 support | ✅ |
| ChaCha20-Poly1305 / AES-GCM ciphers | ✅ |
| Custom ClientHello / ALPN | ✅ |
| SNI fragment / TLS fragment | ✅ |
| Fallback to ChaCha20 | ✅ |
| AES-128/256-GCM (Shadowsocks) | ✅ |
| Auto-detect / Dynamic session key | ✅ |
| Online Optimization / API / Custom IP list | ✅ |
| Random IP generation / Categorized results | ✅ |
| Save/Override scanning results | ✅ |
| Per-ISP clean-IP optimization | ✅ |
| Telegram Webhook / Bot settings in panel | ✅ |
| Cloudflare usage monitor / API Token tracking | ✅ |
| Custom Usage API | ✅ |
| VLESS + Shadowsocks direct link | ✅ |
| Subscription with token authentication | ✅ |
| Full clipboard copy (One-click) | ✅ |
| KV Storage configuration (Config, CF, TG, IPs, Logs) | ✅ |
| Password login / Auth Cookie | ✅ |
| UUID Validation / Token Auth (MD5) | ✅ |
| Speed test blocking | ✅ |
| Environment variables management | ✅ |
| Leaflet Map / Toast / Modal UI components | ✅ |
| Collapsible modules / SVG icons | ✅ |
| Concurrent TCP dial / 0-RTT | ✅ |
| Uplink/downlink traffic aggregation | ✅ |
| Upload queue limit | ✅ |
| Load Balance IP / Proxy Fallback | ✅ |
| Tokenless subscription link with named formats | ✅ |
| Permanent GitHub mirror for subscription | ✅ |
| Monolithic panel layout (Static Assets) | ✅ |
| Dual-language interface + Guided tour | ✅ |
| Malware / Phishing / Cryptominers blocking | ✅ |
| QUIC blocking | ✅ |
| Backend Mode (VLESS + UDP / Video Call) | ✅ |
| ECH (Encrypted SNI) | ✅ |
| Port-spread / Multi-transport | ✅ |
| Automatic domain update notification on Telegram | ✅ |
| Daily traffic charts + Upload/Download breakdown | ✅ |
| Dedicated user links + Total/Daily quota + Expiry + On/Off | ✅ |
| Subscription link with Username + Secret Key | ✅ |
| Read-after-write KV caching for instant updates | ✅ |
| NAT64 support / IPv6 transition | ✅ |
| Panel password change + 2FA (TOTP) + Recovery code | ✅ |
| Login attempt limit + Session management | ✅ |
| WARP registration + WARP+ License + WoW | ✅ |
| WARP endpoint modification + Iran endpoints | ✅ |
| Amnezia WARP mode + WARP Noise | ✅ |
| One-click Iran mode + Live config report | ✅ |
| Full settings backup and restore | ✅ |
| Middleware fallback (Non-Cloudflare nodes) | ✅ |
| Self-healing domain pool + Health check | ✅ |
| Country bypass (China, Russia, Sanctions) | ✅ |
| Custom routing rules | ✅ |
| Centralized management API + Fleet stats + Global broadcast | ✅ |
| Kill switch | ✅ |
| Instance heartbeat + Notification system | ✅ |
| D1 Database support (KV migration) | ✅ |
| Wizard installation /install + One-click deploy | ✅ |

---

## 🙏 Credits

Built with ❤️ for a free and open internet.

- [Cloudflare Workers](https://workers.cloudflare.com/)
- [Xray-core](https://github.com/XTLS/xray-core)

---

## License

MIT — See [LICENSE](LICENSE) file for details.

---

<div align="center">

Made for Iran <img src="https://raw.githubusercontent.com/IRNova/Nova-Proxy/main/flag-iran.svg" height="16" alt="Iran" /> — and everyone who needs a free internet.  
**No traffic log is stored. The proxy is entirely yours.**

📖 [نسخه فارسی / Persian version](README.fa.md)

</div>
