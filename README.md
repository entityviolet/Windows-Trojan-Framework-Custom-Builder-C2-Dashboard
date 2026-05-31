# 🧬 V-Entity Trojan Framework

> **Custom-compiled Windows agent framework with per-user C2 dashboard and intelligence analysis pipeline.**

V-Entity Trojan is a fully customizable Windows remote intelligence platform — compiled per-deployment with your chosen settings, icon, compiler, and target paths. Each build is cryptographically unique, keeping detection low. Built, managed, and analyzed entirely from a private web dashboard.

**⚠️ Public overview repository.** The actual platform, agent source code, and builder infrastructure are hosted privately and compiled per-user at [v-entity.pro](https://v-entity.pro).

---

## 🖥️ Agent Capabilities

| Capability | Description |
|---|---|
| **Global Keylogging** | Low-level `WH_KEYBOARD_LL` hook — captures all keystrokes across the system, reconstructs text from token streams, handles Shift/Caps/Numpad |
| **Screen Capture** | GDI+ multi-monitor screenshot (virtual screen dimensions), compressed JPEG upload |
| **File Harvesting** | Configurable path list — monitors directories and files, zips folders with recursion, uploads via R2 |
| **Login Data Processing** | Detects and processes Chromium `Login Data` SQLite databases, produces decrypted `.decoded.txt` credential dumps |
| **Remote Command Execution** | Polls `command.txt` from R2 cloud bucket, executes via `cmd.exe`, uploads `result.txt` output back — no open ports needed |
| **Watchdog Persistence** | Self-deploys to 3 locations (`%LOCALAPPDATA%\Enterprise`, `%LOCALAPPDATA%\Microsoft\Edge\Application`, `%LOCALAPPDATA%\Microsoft\Internet Explorer`) with mutex-based watchdog processes that relaunch each other |
| **Windows Service Mode** | Installs and runs as a Windows service (`TypingLogAssistantService`) with SCM control handler |
| **Registry Persistence** | Registers Run key entries (`MicrosoftEdgeUpdate`, `InternetExplorerUpdate`) for auto-start on boot |
| **Startup Shortcut** | Creates `.lnk` shortcut in Windows Startup folder via PowerShell |
| **Mutex Single-Instance** | Global mutex ensures only one worker runs; watchdogs take over on failure |
| **Remote Configuration** | Downloads per-system settings from cloud (`settings.json`, `startup.json`) — intervals, paths, screenshot/log toggles |
| **Binder Support** | Compiles agent stitched with a legitimate host EXE — host runs normally, agent extracts silently in background |

---

## 🕵️ Backend Analysis Pipeline

| Capability | Description |
|---|---|
| **System Identification** | Extracts OS version, entity software version, and unique hardware-bound System Key from log data |
| **Crypto Wallet Detection** | Scans all keystroke logs and directory paths for 100+ wallet keywords — Phantom, MetaMask, Ledger, Trezor, Exodus, Trust Wallet, Electrum, Keplr, Ronin, Coinbase Wallet, TronLink, and more |
| **Crypto Seed Hunter** | Detects BIP39 seed phrases, mnemonic codes, private keys, keystore files, wallet.dat, and recovery seeds across all harvested data |
| **Secret Trace Scanner** | Multi-pass heuristic engine for credit/debit cards (Visa, MC, Amex), bank accounts (IBAN, SWIFT, routing), payment platforms (PayPal, Revolut, Wise, Stripe, Venmo, Cash App), credential stores (1Password, Bitwarden, LastPass, KeePass, Dashlane) |
| **Password Decryption** | Parses Chromium `Login Data` and `decoded.txt` files — sorts by richness, displays decrypted URL/Username/Password triples with one-click copy |
| **Credential Extraction** | Chrome, Edge, Brave saved passwords with state indicator (DECRYPTED / ENCRYPTED / NONE) |
| **Browser Session Data** | Extracts browser session data, Local Extension Storage, Web Data — including saved autofill profiles and encrypted card numbers |
| **Full Browser Session Hijack** | Identifies and extracts browser session tokens, cookies, and state for potential session cloning |
| **Browser Cookie Extraction** | Detects cookie databases from Chrome/Brave/Edge — AES-GCM decrypted session data |
| **Auto-Fill & Card Data** | Parses Chrome Web Data for autofill profiles and encrypted credit card numbers |
| **Clipboard Monitoring** | Captures clipboard contents appended to keyboard logs in real-time |
| **Live Camera Streaming** | Remote camera activation with real-time feed via WebSocket viewer |
| **Script Injection** | Remote PowerShell execution with configurable delay — inline script editor, runs on target |
| **Keyboard Log Analysis** | Token stream parsing — reconstructs readable text from [Backspace], [Shift], [Enter], [Space] sequences |
| **Directory Reconstruction** | Full Windows filesystem path rebuilding from flat log dumps — infers root anchors, priority folders, env-var notation |
| **Email & Domain Extraction** | Redacted email display with domain frequency ranking — identifies which services the target uses |
| **File Browser** | Browse and download captured files per system with type icons, sizes, timestamps |

---

## 📊 Dashboard Features

| Feature | Description |
|---|---|
| **Multi-System Overview** | Real-time status of all targets — OS, last seen, system key, entity version, wallet flags, credential counts |
| **Screenshot Album** | Date-grouped gallery with week headers, fullscreen modal viewer, zoom, keyboard navigation, batch select/delete |
| **Keystroke Viewer** | Reconstructed readable text with symbolic rendering (⌫, ⌦, ⇧, ↵), session timestamps, raw token toggle |
| **Credential Tables** | Passwords with click-to-copy, URL links, decrypted values — 192+ entries on typical Chrome profiles |
| **Crypto Wallet Panel** | Keyword-hit badge on each system card, clickable match details, auto-generated path config snippets |
| **Secret Trace Report** | Terminal-style report with per-hit context, matched keyword tag, session timestamp |
| **Email & Domain Views** | Clean two-column tables — redacted addresses, domain frequency rankings |
| **Remote Console** | Bidirectional shell — enter commands, read live results, execute on any agent |
| **Settings Manager** | Per-system and global controls — screenshot/log toggles, auto-share intervals, remote command enable |
| **Startup Path Manager** | Edit download path configuration with env-var notation (%USERPROFILE%, %LOCALAPPDATA%) |
| **File Download Manager** | Browse, inspect, and download all exported files per system |
| **Multi-Theme UI** | 4 terminal themes: Green Hacker, Purple Terminal (default), Blue Dark, Light — all with CRT scanline effect |
| **Admin Panel** | User management — create, edit, delete, subscription control, R2 credential configuration |

---

## 🧬 Agent Builder

| Feature | Description |
|---|---|
| **Custom Compilation** | Build per-deployment agent with unique PE signature |
| **Compiler Options** | LLVM/Clang (different PE signature, less Defender detection), MinGW (standard GCC), UPX variants |
| **Icon Customization** | Upload custom .ico file for the compiled executable |
| **Target Path Groups** | Presets: browsers, crypto wallets, messaging apps, password managers, cloud storage, email clients, SSH keys, databases, auth apps |
| **Binder / Host Stubbing** | Merge agent with legitimate EXE — host runs visibly, agent extracts silently in background |
| **Per-System Tuning** | Independent capture intervals, screenshot/log toggles, and remote command settings per target |
| **Zip Download** | Build output includes compiled agent, bundled DLL runtime, uninstaller script, optional stitched host+agent |

---

## 💰 Pricing

```
3-Day Trial     $16    ($5.33/day)
7-Day Trial     $27    ($3.86/day)
Monthly         $47    ($1.57/day)
3 Months        $99    ($1.10/day)
6 Months        $169   ($0.94/day)
Lifetime        $379   (one-time)
```

**Accepted Crypto:** BTC · ETH · XMR · SOL · LTC · ZEC · DASH · DOGE · NEAR · ATOM · SUI

---

## 🚀 How It Works

1. **Create your account** at [v-entity.pro](https://v-entity.pro)
2. **Configure your agent** — choose target paths, capture intervals, icon, and compiler
3. **Download** your custom-compiled executable
4. **Deploy** — the agent collects data and syncs to your dashboard
5. **Analyze** — view screenshots, keystrokes, passwords, wallets, secrets, and files from your private dashboard

All settings, captures, and storage are **isolated per user**.

---

## 🔗 Links

**Website:** [https://v-entity.pro](https://v-entity.pro)  
**Contact:** [support@v-entity.pro](mailto:support@v-entity.pro)  
**Telegram:** [https://t.me/violetentity](https://t.me/violetentity)

---

*This tool is intended exclusively for authorized security testing, educational purposes, and legitimate research.*  
*This repository is a project overview. The actual platform, agent source code, and builder infrastructure are hosted privately and compiled per-user.*
