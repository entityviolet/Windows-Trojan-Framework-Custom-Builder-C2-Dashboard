# 🧬 V-Entity Trojan Framework

> **Custom-compiled Windows agent framework with per-user C2 dashboard and intelligence analysis engine.**

V-Entity Trojan is a fully customizable Windows remote intelligence platform — compiled per-deployment with your chosen settings, icon, compiler, and target paths. Every build is cryptographically unique. Built, managed, and analyzed entirely from a private web dashboard.

**⚠️ Public overview repository.** The actual platform, agent source code, and builder infrastructure are hosted privately and compiled per-user at [v-entity.pro](https://v-entity.pro).

---

## 🖥️ Agent Capabilities

| Capability | Description |
|---|---|
| **Full Keystroke Capture** | Captures all keyboard input across the entire system — reconstructs readable text from every session |
| **Screen Capture** | Captures real-time desktop screenshots from the target machine |
| **Smart File Harvesting** | Monitors and exfiltrates files and folders from configurable target paths — automatically zips directories |
| **Credential Theft** | Extracts saved browser passwords, autofill profiles, cookies, and session data from Chrome, Edge, and Brave |
| **Remote Command Execution** | Execute shell commands on the target — no open ports, no reverse connection needed |
| **Self-Healing Persistence** | Deploys to multiple system locations — if one copy is removed, others restore it automatically |
| **Windows Service Installation** | Optionally runs as a hidden Windows service — survives reboots |
| **Binder / Host Stubbing** | Merges agent with any legitimate executable — host runs normally while agent extracts silently |

---

## 🕵️ Analysis Engine

| Capability | Description |
|---|---|
| **System Fingerprinting** | Identifies OS version, system identifier, and unique hardware-bound machine key |
| **Crypto Wallet Hunter** | Scans all captured data for 100+ wallet types — Phantom, MetaMask, Ledger, Trezor, Exodus, Trust Wallet, Electrum, Keplr, Coinbase Wallet, and more |
| **Seed Phrase & Private Key Finder** | Detects BIP39 seed phrases, mnemonic codes, private keys, keystore files, wallet.dat, and recovery seeds |
| **Secret & Credential Scanner** | Scans for credit/debit card numbers, bank accounts (IBAN, SWIFT), payment accounts (PayPal, Revolut, Wise, Stripe, Venmo), API keys, SSH keys, 2FA codes, and credential store entries |
| **Password Recovery** | Decrypts and displays saved browser passwords with one-click copy |
| **Browser Session Extraction** | Extracts cookies, saved sessions, autofill profiles, and encrypted card data |
| **Session Hijack Data** | Harvests browser session tokens and state data for potential session cloning |
| **Keyboard Log Decoder** | Reconstructs readable text from raw keystroke logs — handles special keys, backspace, shift states |
| **Directory Intelligence** | Rebuilds full Windows filesystem paths from raw directory dumps |
| **Email & Domain Discovery** | Extracts and categorizes email addresses by domain — reveals which services the target uses |
| **Clipboard Capture** | Captures clipboard content appended to keystroke data |
| **Live Camera Feed** | Remotely activates camera — real-time video stream via WebSocket |
| **Script Injection** | Executes arbitrary PowerShell scripts on the target with configurable delay |

---

## 📊 Dashboard

| Feature | Description |
|---|---|
| **Multi-System Overview** | Real-time status board — OS, last seen, active wallets, credential counts, file inventory |
| **Screenshot Gallery** | Date-organized album with fullscreen viewer, zoom, batch selection, and deletion |
| **Keystroke Viewer** | Readable reconstructed text from every keystroke session — organized by timestamp |
| **Wallet Dashboard** | Crypto matches tagged per-system with clickable forensic details |
| **Password Manager** | Searchable table of decrypted credentials — one-click copy |
| **Secret Trace Reports** | Terminal-style scan results with contextual hits |
| **Email Analyzer** | Redacted address view with domain ranking |
| **Remote Console** | Built-in shell for live command execution on any target |
| **System Controls** | Per-system toggle for screenshot capture, logging, and remote commands |
| **File Explorer** | Browse and download files harvested from any target |
| **Theme Selector** | 4 visual themes — dark, light, and terminal-inspired designs |
| **Admin Panel** | User and subscription management dashboard |

---

## 🧬 Custom Builder

| Feature | Description |
|---|---|
| **Per-Deployment Compilation** | Every agent build is unique — different PE signature each time |
| **Multiple Compilers** | Choose from different compiler backends for maximum evasion |
| **Custom Icon** | Upload your own icon for the executable |
| **Path Presets** | Pre-configured profiles: browsers, wallets, messaging, auth, databases, cloud, email |
| **Binder** | Stitch agent into any host executable |
| **Per-Target Tuning** | Independent intervals and toggles per infected machine |

---

## 💰 Pricing

```
3-Day Trial     $16
7-Day Trial     $27
Monthly         $47
3 Months        $99
6 Months        $169
Lifetime        $379
```

**Accepted Crypto:** BTC · ETH · XMR · SOL · LTC · ZEC · DASH · DOGE · NEAR · ATOM · SUI

---

## 🚀 How It Works

1. **Create your account** at [v-entity.pro](https://v-entity.pro)
2. **Configure your agent** — choose target paths, capture intervals, icon, and compiler
3. **Download** your custom-compiled executable
4. **Deploy** — the agent collects data and syncs to your dashboard
5. **Analyze** — screenshots, keystrokes, passwords, wallets, secrets, and files

All data is **isolated per user**.

---

## 🔗 Links

**Website:** [https://v-entity.pro](https://v-entity.pro)  
**Contact:** [support@v-entity.pro](mailto:support@v-entity.pro)  
**Telegram:** [https://t.me/violetentity](https://t.me/violetentity)

---

*This tool is intended exclusively for authorized security testing.*  
*This repository is a project overview. The platform, agent code, and builder are hosted privately.*
