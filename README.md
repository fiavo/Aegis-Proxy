<div align="center">

# 🛡️ Aegis Proxy

**A smart, censorship-resistant proxy panel running entirely on Cloudflare Workers**

[![License](https://img.shields.io/badge/license-MIT-green?style=for-the-badge)](LICENSE)
[![Version](https://img.shields.io/badge/version-1.0.0-blueviolet?style=for-the-badge)](https://github.com/fiavo/Aegis-Proxy)
[![Stars](https://img.shields.io/github/stars/fiavo/Aegis-Proxy?style=for-the-badge&color=0ea5e9)](https://github.com/fiavo/Aegis-Proxy)

</div>

---

## ✨ Features

- ⚡ **Blazing Fast** — Runs entirely on Cloudflare's edge network
- 🔒 **Secure** — Strong encryption, no logs, privacy-first
- 🌍 **Clean IPs** — Automatic ISP-specific IP optimization for Iran
- 👥 **Multi-User** — Per-user quotas, expiry dates, and on/off toggle
- 🤖 **Telegram Bot** — Full management via Telegram
- 📱 **Cross-Platform** — Works on all devices and platforms
- 🆓 **Free Tier** — Runs on Cloudflare's free plan

---

## 📋 Supported Protocols

| Protocol | Description |
|----------|-------------|
| **VLESS** | Fast and secure |
| **Trojan** | Reliable and trusted |
| **Shadowsocks** | Classic and stable |
| **WireGuard** | Modern and fast |
| **Xray** | Flexible and powerful |

---

## 🚀 Quick Start

### Prerequisites

- [Node.js](https://nodejs.org/) v22+
- [Cloudflare Account](https://www.cloudflare.com/) (free)
- [Wrangler CLI](https://developers.cloudflare.com/workers/wrangler/)

### Installation & Deployment

```bash
# 1. Clone the repository
git clone https://github.com/fiavo/Aegis-Proxy.git
cd Aegis-Proxy

# 2. Install dependencies
npm install

# 3. Login to Cloudflare
wrangler login

# 4. Create D1 database
wrangler d1 create aegis-proxy-db

# 5. Edit wrangler.jsonc
# Replace the database_id with the one from step 4

# 6. Deploy
wrangler deploy

# 7. Initial setup
# Open the Worker URL and go to /install
```

---

## 📖 Documentation

### 🌐 Accessing the Panel

After deployment, the management panel is available at:

```
https://your-worker.workers.dev/install
```

### 👤 Creating Users

1. Login to the panel
2. Navigate to "Users"
3. Add a new user
4. Copy the subscription link

### 📱 Connecting via Telegram

1. Copy the subscription link
2. Send it in Telegram
3. Connection is established automatically

---

## ⚙️ Advanced Configuration

### Telegram Bot

```bash
# In the panel Settings section
TELEGRAM_BOT_TOKEN: your_bot_token
TELEGRAM_ADMINS: your_admin_id
```

### WARP Integration

```bash
# Enable WARP
Settings → WARP → Enable
```

### Custom Domain

```bash
# Add a custom domain
wrangler route add aegis-proxy.example.com/*
```

---

## 🔧 Troubleshooting

### Connection Issues

```bash
# Check logs
wrangler tail
```

### Database Issues

```bash
# List databases
wrangler d1 list
```

### Manual Update

```bash
# Redeploy
wrangler deploy
```

---

## 📊 Performance

| Metric | Value |
|--------|-------|
| Latency | < 50ms |
| Speed | > 100Mbps |
| Memory | < 128MB |
| Concurrent Users | > 1000 |

---

## 🤝 Contributing

We welcome contributions!

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Submit a Pull Request

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).

---

## 🙏 Acknowledgments

- [Cloudflare](https://www.cloudflare.com/) — Free infrastructure
- The open-source community

---

<div align="center">

**🛡️ Aegis Proxy — Protecting your privacy**

</div>
