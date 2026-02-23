<img alt="Hostura" src="https://raw.githubusercontent.com/Hostura/.github/main/assets/logo-light.png" width="400">

# Self-hosting made simple

**Hostura** is a 100% Docker-native self-hosting platform inspired by YunoHost. Deploy, manage, and secure your applications with a single CLI.

[![License: AGPL-3.0](https://img.shields.io/badge/License-AGPL%203.0-blue.svg)](https://opensource.org/licenses/AGPL-3.0)
[![Built with Rust](https://img.shields.io/badge/Built%20with-Rust-orange.svg)](https://www.rust-lang.org/)
[![Docker](https://img.shields.io/badge/Docker-Native-2496ED.svg)](https://www.docker.com/)

---

## ✨ Features

| Feature | Description |
|---------|-------------|
| 🐳 **Docker Native** | Every app runs in containers. No system pollution. |
| 🔐 **SSO Included** | Authentik-powered single sign-on for all your apps |
| 📦 **App Catalog** | One-command install from community-maintained catalog |
| 🌐 **Auto SSL** | Let's Encrypt certificates via Traefik |
| 💾 **Backups** | Per-app backups with Restic to any destination |
| 🏠 **Self-Hosted** | Your data stays on your server |

---

## 🚀 Quick Start

```bash
# Install Hostura
curl -fsSL https://get.hostura.dev | sh

# Initialize your server
hostura init --domain example.com

# Install your first app
hostura apps install vaultwarden

# Check status
hostura status
```

---

## 📦 Repositories

| Repository | Description |
|------------|-------------|
| [**hostura**](https://github.com/Hostura/hostura) | Core CLI & API (Rust) |
| [**stack**](https://github.com/Hostura/stack) | Infrastructure Docker configs |
| [**hostura-catalog**](https://github.com/Hostura/hostura-catalog) | Community app catalog |

---

## 🏗️ Architecture

```
Internet → Traefik (SSL) → Your Apps → Shared Services (DB, Redis, Backup)
                ↓
           Authentik (SSO)
```

---

## 🤝 Contributing

We welcome contributions! Check out:
- [Contributing Guide](https://github.com/Hostura/hostura/blob/main/CONTRIBUTING.md)
- [Roadmap](https://github.com/Hostura/stack/blob/main/docs/ROADMAP.md)
- [App Catalog Guidelines](https://github.com/Hostura/hostura-catalog/blob/main/CONTRIBUTING.md)

---

## 📄 License

Hostura is open source under the [AGPL-3.0 License](https://opensource.org/licenses/AGPL-3.0).

---

<p align="center">
  <sub>Built with 🦀 Rust and 🐳 Docker</sub>
</p>
