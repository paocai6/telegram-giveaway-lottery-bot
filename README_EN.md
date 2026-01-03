# 🎰 Lucky Star Bot - Telegram Giveaway Bot

<p align="center">
  <img src="docs/images/IMG_1779.png" alt="Lucky Star Bot" width="600">
</p>

<p align="center">
  <a href="https://t.me/MyLuckyStar8_Bot">
    <img src="https://img.shields.io/badge/Telegram-Bot-blue?logo=telegram" alt="Telegram Bot">
  </a>
  <a href="[https://t.me/your_channel](https://t.me/MyLuckyStar6)">
    <img src="https://img.shields.io/badge/Telegram-Channel-blue?logo=telegram" alt="Telegram Channel">
  </a>
  <img src="https://img.shields.io/badge/Status-Active-brightgreen" alt="Status">
  <img src="https://img.shields.io/badge/Language-Go%20%7C%20React-informational" alt="Tech Stack">
</p>

<p align="center">
  <a href="README.md">🇨🇳 简体中文</a> | <b>🇺🇸 English</b>
</p>

---

## ✨ Features

### 🎁 Multiple Draw Modes
| Mode | Description |
|------|-------------|
| ⏰ **Timed Draw** | Set end time, auto-draw when time's up |
| 👥 **Participant Count** | Auto-draw when reaching target participants |
| 🎲 **Instant Draw** | Know the result immediately upon participation |

### 🏆 Prize Management
- 🎫 **Multi-Prize Support** - Set up multiple different prizes
- 🔑 **Auto Code Distribution** - Automatic activation code delivery with usage URL
- 👤 **Contact Mode** - Show contact info for manual prize distribution
- 📦 **CSV Bulk Import** - Add prizes in bulk via CSV file

### 📋 Entry Requirements
| Requirement | Description |
|-------------|-------------|
| 📢 Subscribe Channel/Group | Must follow specified channel or join group |
| 💬 Message Count | Send specified number of messages in group |
| 🔢 Keyword Entry | Enter by sending specific keyword |
| 💎 Points Consumption | Use points to participate |
| 🚀 Boost Channel | Need to boost specified channel |
| 💰 TON Wallet Balance | Hold specified amount of TON tokens |
| 🪙 Jetton Holdings | Hold specified Jetton tokens |
| 🖼️ NFT Ownership | Own NFTs from specified collection |

### 🌐 Multi-Language Support
Supports **14 languages**:
- 🇨🇳 Simplified Chinese / 🇹🇼 Traditional Chinese
- 🇺🇸 English / 🇪🇸 Spanish / 🇫🇷 French
- 🇩🇪 German / 🇮🇹 Italian / 🇵🇹 Portuguese
- 🇷🇺 Russian / 🇯🇵 Japanese / 🇰🇷 Korean
- 🇹🇭 Thai / 🇻🇳 Vietnamese / 🇹🇷 Turkish / 🇳🇱 Dutch

### 🔒 Provably Fair Drawing
- 🎲 **Verifiable Randomness** - Cryptographically secure random number generation
- 📜 **Draw Proofs** - Complete proof of drawing process
- 🔗 **Blockchain Entropy** - Integrated TON blockchain and drand beacon as external random sources

---

## 📱 Screenshots

<p align="center">
  <img src="docs/images/IMG_2069.png" alt="Home" width="250">
  <img src="docs/images/IMG_2070.png" alt="Create Giveaway" width="250">
  <img src="docs/images/IMG_2071.png" alt="Results" width="250">
</p>

---

## 🚀 Quick Start

### Option 1: Use Directly (Recommended)
1. Open Telegram and search [@MyLuckyStar8_Bot](https://t.me/MyLuckyStar8_Bot)
2. Click **Start** to begin
3. Add the bot as admin to your group/channel
4. Create giveaways via Mini App

### Option 2: Private Deployment
For private deployment, please contact us for commercial licensing.

---

## 💡 Use Cases

| Scenario | Description |
|----------|-------------|
| 📢 **Channel Promotion** | Grow followers quickly through giveaways |
| 👥 **Community Engagement** | Encourage member participation |
| 🎮 **Game Rewards** | Distribute game CDKs and redemption codes |
| 🛒 **E-commerce Promotions** | Coupon and discount code distribution |
| 🎉 **Holiday Events** | Seasonal giveaways to reward users |

---

## 📊 Technical Architecture

```
┌─────────────────────────────────────────────────────┐
│                   Telegram Mini App                  │
│                   (React + TypeScript)               │
└─────────────────────────────────────────────────────┘
                          │
                          ▼
┌─────────────────────────────────────────────────────┐
│                    Backend API                       │
│                    (Go + Fiber)                      │
├─────────────────────────────────────────────────────┤
│  • RESTful API      • WebSocket                     │
│  • Rate Limiting    • Init Data Validation          │
│  • Redis Caching    • PostgreSQL Storage            │
└─────────────────────────────────────────────────────┘
                          │
          ┌───────────────┼───────────────┐
          ▼               ▼               ▼
    ┌──────────┐   ┌──────────┐   ┌──────────────┐
    │ Telegram │   │   TON    │   │    drand     │
    │ Bot API  │   │Blockchain│   │   Beacon     │
    └──────────┘   └──────────┘   └──────────────┘
```

---

## 🛡️ Security Features

- ✅ **Telegram InitData Validation** - Prevent request forgery
- ✅ **Rate Limiting** - Prevent API abuse
- ✅ **AES-256-GCM Encryption** - Encrypted storage of sensitive data
- ✅ **CORS Protection** - Restricted origin domains
- ✅ **SQL Injection Prevention** - Parameterized queries

---

## 📞 Contact Us

| Channel | Link |
|---------|------|
| 📢 Official Channel | [@MyLuckyStar6](https://t.me/MyLuckyStar6) |
| 💬 Discussion Group | [@LuckyStar9988](https://t.me/LuckyStar9988) |
| 🤖 Bot | [@MyLuckyStar8_Bot](https://t.me/MyLuckyStar8_Bot) |
| 📧 Business Inquiries | [@paocai6](https://t.me/paocai6) |

---

## 📜 Changelog

### v2.5.0 (2026-01-03)
- ✨ Added activation code URL feature
- ✨ CSV bulk import now supports usage URL
- 🐛 Fixed prize data not pre-filling when editing

### v2.4.0 (2026-01-01)
- ✨ Added verifiable fair lottery system
- ✨ Added draw proof generation
- ✨ Integrated TON blockchain and drand beacon as random sources

[View Full Changelog](CHANGELOG.md)

---

## ⚖️ License

This project is **closed-source commercial software**.

- 🚫 Source code is not public
- ✅ Free to use the official bot
- 💼 Private deployment requires commercial license

For commercial licensing or private deployment, please reach out via the contact channels above.

---

<p align="center">
  <b>⭐ If you find this useful, please Star this repository ⭐</b>
</p>

<p align="center">
  Made with ❤️ by Lucky Star Team
</p>
