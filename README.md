# 🧬 V-Entity Trojan Framework

> **Custom-compiled Windows agent framework with per-user C2 dashboard and intelligence analysis engine.**

V-Entity Trojan is a fully customizable Windows remote intelligence platform — compiled per-deployment with your chosen settings, icon, compiler, and target paths. Every build is cryptographically unique. Built, managed, and analyzed entirely from a private web dashboard.

**⚠️ Public overview repository.** The actual platform, agent source code, and builder infrastructure are hosted privately and compiled per-user at [v-entity.pro](https://v-entity.pro).

---

## 🖥️ Agent Capabilities

| Capability | Description |
|---|---|
| **Full Keystroke Capture** | Captures all keyboard input across the entire system — reconstructs readable text from every session, handles special keys and shift states |
| **Screen Capture** | Captures real-time desktop screenshots from the target machine |
| **Live Camera Streaming** | Remotely activates camera devices — real-time video feed via WebSocket or HTTP frames |
| **Clipboard Monitoring** | Intercepts all clipboard changes — captures password manager copies, seed phrase pastes, sensitive field fill-ins |
| **File Harvesting** | Monitors and exfiltrates files and folders from configurable target paths — automatically zips directories |
| **Credential Theft** | Extracts saved passwords, autofill profiles, cookies, and session data from Chrome, Edge, and Brave |
| **Browser Session Hijack** | Captures live browser state — open tabs, navigation history, active authenticated sessions |
| **Auto-Fill & Card Extraction** | Extracts Chrome Web Data — autofill profiles, encrypted credit card numbers |
| **Browser Cookie Decryption** | Decrypts and extracts all cookies from Chromium browsers — AES-GCM decrypted session tokens |
| **Crypto Seed Hunter** | Searches for wallet files, BIP39 seed phrases, keystores, and private keys across user directories |
| **Script Injection** | Write and execute multi-line PowerShell scripts on any target with configurable delay |
| **Remote Command Execution** | Execute shell commands on the target — no open ports, no reverse connection needed |
| **Live Reverse Shell** | One-click interactive PowerShell terminal — browse filesystem, run commands, download files in real time |
| **Self-Healing Persistence** | Deploys to multiple system locations — if one copy is removed, others restore it automatically |
| **Windows Service Mode** | Optionally runs as a hidden Windows service — survives reboots |
| **Binder / Host Stubbing** | Merges agent with any legitimate executable — host runs normally while agent extracts silently |

---

## 🕵️ Analysis Engine

| Capability | Description |
|---|---|
| **System Fingerprinting** | Identifies OS version, system ID, and unique hardware-bound machine key |
| **Crypto Wallet Hunter** | Scans all data for 100+ wallet types — Phantom, MetaMask, Ledger, Trezor, Exodus, Trust Wallet, Electrum, Keplr, Coinbase Wallet, and more |
| **Seed Phrase & Private Key Finder** | Detects BIP39 mnemonic seeds, private keys, keystore files, wallet.dat, and recovery seeds |
| **Secret & Credential Scanner** | Scans for credit/debit cards, bank accounts (IBAN, SWIFT), payment platforms (PayPal, Revolut, Wise, Stripe, Venmo), API keys, SSH keys, 2FA codes |
| **Password Recovery** | Decrypts and displays saved browser passwords with one-click copy |
| **Session Extraction** | Harvests session tokens, cookies, and browser state for potential cloning |
| **Keyboard Log Decoder** | Reconstructs readable text from raw keystroke logs — handles backspace, shift states, numpad |
| **Directory Intelligence** | Rebuilds full Windows filesystem paths from raw directory dumps |
| **Email & Domain Discovery** | Extracts and categorizes email addresses by domain — reveals which services the target uses |

---

## 📊 Dashboard

| Feature | Description |
|---|---|
| **Multi-System Overview** | Real-time status board — OS, last seen, active wallets, credential counts, file inventory |
| **Live Reverse Shell** | Interactive PowerShell terminal — real-time relay, file download, multi-session support |
| **Screenshot Gallery** | Date-organized album with fullscreen viewer, zoom, batch selection, and deletion |
| **Camera Live Viewer** | Real-time camera feed with frame counter and connection status |
| **Script Injection Panel** | Multi-line PowerShell editor with syntax styling, delay configuration, one-click inject |
| **Keystroke Viewer** | Readable reconstructed text from every keystroke session — organized by timestamp |
| **Wallet Dashboard** | Crypto matches tagged per-system with clickable forensic details |
| **Password Manager** | Searchable table of decrypted credentials with one-click copy |
| **Secret Trace Reports** | Terminal-style scan results with contextual hits |
| **Email Analyzer** | Redacted address view with domain frequency ranking |
| **Remote Console** | Built-in shell for command execution on any target |
| **System Controls** | Per-system toggles for screenshot capture, logging, remote commands, clipboard, camera, cookies |
| **File Explorer** | Browse and download files harvested from any target |
| **Theme Selector** | 4 visual themes — dark, light, and terminal-inspired designs |

---

## 🧬 Custom Builder

| Feature | Description |
|---|---|
| **Per-Deployment Compilation** | Every agent build is unique — different PE signature each time |
| **Multiple Compiler Backends** | Choose from different compilers for maximum evasion |
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
5. **Analyze** — screenshots, keystrokes, passwords, wallets, camera, secrets, files, and live shell

All data is **isolated per user**.

---

## 🔗 Links

**Website:** [https://v-entity.pro](https://v-entity.pro)  
**Contact:** [support@v-entity.pro](mailto:support@v-entity.pro)  
**Telegram:** [https://t.me/violetentity](https://t.me/violetentity)

---

*This tool is intended exclusively for authorized security testing.*  
*This repository is a project overview. The platform, agent code, and builder are hosted privately.*
