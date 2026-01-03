# 🎰 Lucky Star Bot - Telegram 抽奖机器人

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
  <b>🇨🇳 简体中文</b> | <a href="README_EN.md">🇺🇸 English</a>
</p>

---

## ✨ 功能特性

### 🎁 多种抽奖模式
| 模式 | 说明 |
|------|------|
| ⏰ **定时开奖** | 设置结束时间，到时自动开奖 |
| 👥 **人数开奖** | 达到指定参与人数后自动开奖 |
| 🎲 **即时抽奖** | 参与即开，立刻知道中奖结果 |

### 🏆 奖品管理
- 🎫 **多奖品支持** - 可设置多个不同奖品
- 🔑 **卡密自动发放** - 支持激活码自动分发，附带使用地址
- 👤 **联系人模式** - 手动发奖时显示联系人信息
- 📦 **CSV批量导入** - 通过CSV文件批量添加奖品

### 📋 参与要求
| 要求类型 | 说明 |
|----------|------|
| 📢 订阅频道/群组 | 必须关注指定频道或加入群组 |
| 💬 发言数量 | 在群内发送指定数量消息 |
| 🔢 口令参与 | 发送特定关键词参与 |
| 💎 积分消耗 | 使用积分参与抽奖 |
| 🚀 Boost频道 | 需要Boost指定频道 |
| 💰 TON钱包余额 | 持有指定数量TON代币 |
| 🪙 Jetton持仓 | 持有指定Jetton代币 |
| 🖼️ NFT持有 | 持有指定NFT集合 |

### 🌐 多语言支持
支持 **14种语言**：
- 🇨🇳 简体中文 / 🇹🇼 繁体中文
- 🇺🇸 English / 🇪🇸 Español / 🇫🇷 Français
- 🇩🇪 Deutsch / 🇮🇹 Italiano / 🇵🇹 Português
- 🇷🇺 Русский / 🇯🇵 日本語 / 🇰🇷 한국어
- 🇹🇭 ไทย / 🇻🇳 Tiếng Việt / 🇹🇷 Türkçe / 🇳🇱 Nederlands

### 🔒 公平抽奖机制
- 🎲 **可验证随机性** - 基于密码学的随机数生成
- 📜 **开奖凭证** - 提供完整的开奖过程证明
- 🔗 **区块链熵源** - 集成TON区块链和drand信标作为外部随机源

---

## 📱 界面预览

<p align="center">
  <img src="docs/images/IMG_2073.png" alt="首页" width="250">
  <img src="docs/images/IMG_2074.png" alt="创建抽奖" width="250">
  <img src="docs/images/IMG_2075.png" alt="添加奖品" width="250">
</p>

---

## 🚀 快速开始

### 方式一：直接使用（推荐）
1. 打开 Telegram 搜索 [@MyLuckyStar8_Bot](https://t.me/MyLuckyStar8_Bot)
2. 点击 **Start** 开始使用
3. 将机器人添加为群组/频道管理员
4. 通过 Mini App 创建抽奖

### 方式二：私有部署
如需私有化部署，请联系我们获取商业授权。

---

## 💡 使用场景

| 场景 | 说明 |
|------|------|
| 📢 **频道推广** | 通过抽奖活动快速涨粉 |
| 👥 **社群活跃** | 激励群成员发言互动 |
| 🎮 **游戏奖励** | 发放游戏CDK、兑换码 |
| 🛒 **电商促销** | 优惠券、折扣码发放 |
| 🎉 **节日活动** | 节假日抽奖回馈用户 |

---

## 📊 技术架构

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

## 🛡️ 安全特性

- ✅ **Telegram InitData 验证** - 防止请求伪造
- ✅ **请求频率限制** - 防止API滥用
- ✅ **AES-256-GCM 加密** - 敏感数据加密存储
- ✅ **CORS 跨域保护** - 限制来源域名
- ✅ **SQL 注入防护** - 参数化查询

---

## 📞 联系我们

| 渠道 | 链接 |
|------|------|
| 📢 官方频道 | [@YourChannel](https://t.me/your_channel) |
| 💬 交流群组 | [@YourGroup](https://t.me/your_group) |
| 🤖 机器人 | [@MyLuckyStar8_Bot](https://t.me/MyLuckyStar8_Bot) |
| 📧 商务合作 | your-email@example.com |

---

## 📜 更新日志

### v2.5.0 (2026-01-03)
- ✨ 新增卡密使用地址功能
- ✨ 新增CSV批量导入奖品支持使用地址
- 🐛 修复编辑奖品时数据未预填充问题

### v2.4.0 (2026-01-01)
- ✨ 新增可验证公平抽奖系统
- ✨ 新增开奖凭证生成功能
- ✨ 集成TON区块链和drand信标作为随机源

[查看完整更新日志](CHANGELOG.md)

---

## ⚖️ 许可声明

本项目为**闭源商业软件**。

- 🚫 源代码不公开
- ✅ 可免费使用官方机器人
- 💼 私有化部署需商业授权

如需获取商业授权或私有部署，请通过上方联系方式与我们沟通。

---

<p align="center">
  <b>⭐ 如果觉得有用，欢迎 Star 本仓库 ⭐</b>
</p>

<p align="center">
  Made with ❤️ by Lucky Star Team
</p>
