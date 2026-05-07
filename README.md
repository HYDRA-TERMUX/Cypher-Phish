<div align="center">

<img src="assets/logo.webp" width="500" alt="Cypher Phish Logo">

# Cypher Phish v3.4.0

### Security Awareness & Phishing Simulation Framework

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

Cypher Phish is intended **strictly for educational purposes, internal security awareness programs, and authorized penetration testing environments**.

Unauthorized credential collection, impersonation, or phishing against real users without explicit permission may violate laws and organizational policies.

By using this project, you agree that:

* You own the target systems **or**
* You have written authorization to perform security testing
* You will use the project responsibly and ethically

---

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
* macOS
* Windows (WSL)
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
chmod +x smfdemo.sh
./smfdemo.sh
```

## Termux (Android)

```bash
pkg update && pkg upgrade
pkg install git php curl

git clone https://github.com/HYDRA-TERMUX/cypher-phish.git
cd cypher-phish
chmod +x smfdemo.sh
./smfdemo.sh
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
├── smfdemo.sh
├── logo.sh
├── minilogo.sh
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

1. Create a Telegram bot using BotFather
2. Obtain the bot token
3. Start a conversation with the bot
4. Add the token during setup

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
TELEGRAM_CHAT_ID="YOUR_CHAT_ID"
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
chmod +x smfdemo.sh
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
