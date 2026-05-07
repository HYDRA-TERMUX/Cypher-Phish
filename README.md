<div align="center">

<img src="assets/logo.webp" width="500" alt="Cypher Phish Logo">

# Cypher Phish v3.4.0
### A beginners friendly, Automated phishing tool with 30+ templates.

<p align="center">
  <img src="https://img.shields.io/github/stars/HYDRA-TERMUX/cypher-phish?style=for-the-badge" alt="Stars">
  <img src="https://img.shields.io/github/forks/HYDRA-TERMUX/cypher-phish?style=for-the-badge" alt="Forks">
  <img src="https://img.shields.io/github/issues/HYDRA-TERMUX/cypher-phish?style=for-the-badge" alt="Issues">
  <img src="https://img.shields.io/github/license/HYDRA-TERMUX/cypher-phish?style=for-the-badge" alt="License">
</p>

<p align="center">
  <img src="https://img.shields.io/badge/version-3.4.0-blue?style=for-the-badge" alt="Version">
  <img src="https://img.shields.io/badge/platform-Linux%20%7C%20Termux%20%7C%20macOS%20%7C%20WSL-green?style=for-the-badge" alt="Platform">
  <img src="https://img.shields.io/badge/status-active-success?style=for-the-badge" alt="Status">
  <img src="https://img.shields.io/badge/security-awareness-orange?style=for-the-badge" alt="Security">
</p>

</div>

> A phishing simulation and security awareness framework designed for authorized security testing, employee training, and cybersecurity demonstrations.

---

## ⚠️ Important Notice
> [!CAUTION]
> All usage of **Cypher-Phish** is entirely at your own responsibility. Any **illegal** actions performed with this toolkit are strictly the fault of the end user. The creators, maintainers, and contributors of Cypher-Phish cannot be held accountable for any misuse, damages, or legal issues caused by improper use of this software.
> This project includes simulated phishing and social engineering concepts intended only for cybersecurity education, awareness training, and authorized security testing. Users must follow all applicable local, state, and international laws before downloading, accessing, or operating this toolkit.

> Cypher-Phish is created purely for learning and research purposes. It must never be used to steal credentials, bypass authorization, compromise accounts, or perform **malicious activities** against individuals, organizations, or online services.

> The purpose of this toolkit is to help users understand how phishing techniques function so they can improve security awareness and defensive practices. Any use of this software is done entirely at the user's own risk.
Unauthorized or unethical usage of this project is strongly discouraged. If you intend to use this toolkit for harmful or illegal activities, you should not use this software.

# 📌 Overview

Cypher Phish provides a controlled environment for demonstrating how phishing attacks work during:

* Security awareness workshops
* Red-team exercises
* Employee cybersecurity training
* Internal phishing simulations
* Capture-the-Flag (CTF) learning environments
* Academic cybersecurity research

The framework includes customizable web templates, local hosting support, notification integration, and simulation utilities that help organizations educate users about credential theft risks.

---

# ✨ Features

| Feature                     | Description                                                            |
| --------------------------- | ---------------------------------------------------------------------- |
| 🎭 Multiple Templates       | Includes realistic login simulation pages for awareness demonstrations |
| 🌐 Tunnel Support           | Secure tunneling support for controlled remote demonstrations          |
| 🤖 Notification Integration | Optional notification support for monitoring simulations               |
| 📍 Visitor Logging          | Optional logging for training analytics                                |
| 🔄 Redirect Support         | Redirect participants to official sites after simulations              |
| 💾 Persistent Settings      | Stores configuration preferences for future sessions                   |
| 📱 Termux Compatible        | Works on Android via Termux                                            |
| 🖥️ Cross Platform          | Linux, macOS, WSL, and Termux support                                  |

---

# 🖥️ Supported Platforms

* Linux
* Android (Termux)
---

# 📋 Requirements

### Required Dependencies

* PHP 7+
* cURL
* unzip
* Internet connection

Most missing dependencies are automatically detected during startup.

---

# 🚀 Installation

## Linux / macOS / WSL

```bash
git clone https://github.com/HYDRA-TERMUX/cypher-phish.git
cd cypher-phish
chmod +x setup.sh
./setup.sh
./cypher-phish.sh
```

## Termux (Android)

```bash
pkg update && pkg upgrade
pkg install git php curl

git clone https://github.com/HYDRA-TERMUX/cypher-phish.git
cd cypher-phish
chmod +x setup.sh
./setup.sh
./cypher-phish.sh
```

---

# 🎮 Basic Usage

After launching the framework:

1. Select a simulation template
2. Configure the local server
3. Enable optional integrations
4. Start the awareness simulation
5. Monitor training results in a controlled environment

---

# 📂 Project Structure

```text
cypher-phish/
├── setup.sh
├── cypher-phish
├── .sites/
│   ├── facebook/
│   ├── instagram/
│   ├── google/
│   └── ...
├── .server/
├── .credentials/
└── assets/
```

---

# 🛡️ Available Training Templates

The project includes awareness simulation templates inspired by commonly targeted services such as:

* Facebook
* Instagram
* Google
* Microsoft
* Netflix
* PayPal
* Steam
* Discord
* GitHub
* Roblox
* Spotify
* Reddit
* LinkedIn
* TikTok
* And more

These templates are designed for:

* Awareness demonstrations
* User training
* Red-team simulations
* Internal security assessments

---

# 📱 Telegram Integration

Cypher Phish supports optional Telegram notifications for awareness campaign monitoring.

## Setup Overview
> [!IMPORTANT]
> 1. Create a Telegram bot using BotFather
> 2. Obtain the bot token
> 3. Start a conversation with the bot
> 4. Add the token during setup

The framework stores configuration locally for future sessions.

---

# ⚙️ Configuration

Configuration data is stored inside:

```text
.credentials/config.cfg
```

Example:

```bash
TELEGRAM_BOT_TOKEN="YOUR_BOT_TOKEN"
TELEGRAM_CHAT_ID="YOUR_CHAT_ID" (Automatically adding)
```

---

# 🔧 Cleanup

## Manual Cleanup

```bash
rm -rf .server/
rm -rf .credentials/
pkill php
pkill cloudflared
```

---

# 🐛 Troubleshooting

## PHP Not Found

### Ubuntu / Debian

```bash
sudo apt install php
```

### Termux

```bash
pkg install php
```

### Arch Linux

```bash
sudo pacman -S php
```

---

## Permission Denied

```bash
chmod +x setup.sh
```

---

## Port Already In Use

```bash
lsof -i :8080
kill -9 PID
```

---

# 📝 Changelog

## v3.4.0

* Added additional awareness templates
* Improved notification stability
* Enhanced ARM compatibility
* Improved configuration persistence
* Added redirect support
* General bug fixes and performance improvements

---

# 👨‍💻 Author

### RIXON XAVIER (HYDRA-TERMUX)

GitHub:

```text
https://github.com/HYDRA-TERMUX
```

---

# 📄 License

This repository is provided for:

* Educational use
* Security research
* Awareness training
* Authorized testing

The author is not responsible for misuse or illegal activity.

---

## 🙏 Special Thanks

- **HTR-TECH** - For [ZPhisher](https://github.com/htr-tech/zphisher)


# ⭐ Support

If you found this project useful:

* ⭐ Star the repository
* 🐛 Report issues
* 🔔 Follow for updates
* 🤝 Contribute improvements

---

# ⚖️ Legal Reminder

Always ensure you have:

* Written authorization
* Organizational approval
* Legal permission
* Ethical justification

before conducting any phishing simulation or security assessment.

Unauthorized use may violate cybersecurity laws in your country.
