<h1 align="center">PasteSpace — Clipboard Manager</h1>

<p align="center">
  <strong>Secure clipboard history for macOS. Native. Private. Yours.</strong>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/platform-macOS%2014%2B-blue" alt="macOS 14+" />
  <img src="https://img.shields.io/badge/swift-5.9-orange" alt="Swift 5.9" />
  <img src="https://img.shields.io/badge/UI-SwiftUI-purple" alt="SwiftUI" />
  <img src="https://img.shields.io/badge/encryption-AES--256--GCM-green" alt="AES-256-GCM" />
  <img src="https://img.shields.io/badge/data%20collected-zero-brightgreen" alt="Zero Data Collection" />
  <img src="https://img.shields.io/badge/license-proprietary-lightgrey" alt="Proprietary" />
</p>

<p align="center">
  Free to use · Pro is <strong>$19.99 once, forever</strong> · No subscriptions · No tricks
</p>

---

## The Problem

You copy a phone number. Then a link. Then a paragraph from a document. Then an address. Now you need that phone number again — but it's gone. Your clipboard forgot it the moment you copied the link.

You dig through your browser history. You reopen the document. You scroll through your messages. Five minutes later, you've found it. Five minutes you'll never get back.

**PasteSpace remembers everything you copy** so you never have to.

---

## How It Works

PasteSpace lives in your **menu bar** — a small clipboard icon (📋) that's always there, never in the way. Every time you press `⌘C`, PasteSpace silently catches what you copied and adds it to your searchable history.

**Here's what using PasteSpace actually looks like:**

1. You're writing an email and need a client's address you copied an hour ago
2. Press **⌥⇧V** (or your custom shortcut) — PasteSpace opens instantly
3. Type "Bucharest" in the search bar — the address appears immediately
4. Press **Enter** — it's copied, ready to paste

That's it. No switching apps. No reopening documents. No digging through folders.

---

## Features

### 📋 Clipboard History

Every piece of text, every image, every file you copy — PasteSpace keeps it all in a searchable, scrollable list.

**Real-world example:**
> You're filling out a form that asks for your name, email, phone, address, and IBAN — all stored in different places. Without PasteSpace, you switch between apps six times. With PasteSpace, you copy all six pieces of information beforehand. They're all in your history, one click away.

- **Instant search** — type a word, find it across your entire history
- **Pin items** — your most-used snippets, templates, or credentials stay at the top
- **Source tracking** — every item shows where it came from (Safari, Xcode, Notes, etc.) so you never wonder "where did I copy this?"
- **Global shortcut** (`⌥⇧V`) — open PasteSpace from any app without touching the mouse

---

### 🔐 Vault Mode — Real Encryption, Not Theater

Most "secure" clipboard apps just hide your data behind a toggle. PasteSpace **encrypts** it — with **AES-256-GCM**, the same standard used by banks, via Apple's own CryptoKit framework. Your encryption key is stored in macOS **Keychain**, hardware-backed by the **Secure Enclave** on Apple Silicon.

**Real-world example:**
> You copy your credit card number to paste it into an online checkout. Without PasteSpace, that card number sits in your clipboard as plain text — any app with clipboard access can read it. With PasteSpace, the card number is **instantly detected** as sensitive data and **encrypted on the spot**. A few seconds later, your clipboard history shows `5418 •••• •••• 9593` instead of the full number. To see or use it again, you need your **fingerprint**.

**What gets auto-detected and encrypted:**
- Credit/debit card numbers
- IBANs and bank account numbers
- API keys and tokens (GitHub, Slack, Stripe, JWT)
- SSH keys and fingerprints
- Software license keys (Windows, JetBrains, etc.)
- Passwords from password managers
- OTP codes from authenticator apps
- High-entropy strings that look like secrets

**How Vault works in practice:**

| You copy... | What happens | What you see in history |
|---|---|---|
| `4532 7891 2345 6789` | Auto-detected as credit card → encrypted | `4532 •••• •••• 6789` 🔒 |
| `ghp_abc123def456ghi789` | Auto-detected as GitHub token → encrypted | `ghp_a••••••••••i789` 🔒 |
| `Hello world` | Normal text → stored normally | `Hello world` |
| Any text you choose | Manual vault (click 🔒) → encrypted | `Hello••••orld` 🔒 |

**To reveal a Vault item:** tap the 👁 button → Touch ID prompt → content revealed → auto-hides when you're done.

Vault items survive **Clear All** and **Ephemeral Mode** — they're yours until you explicitly remove them.

---

### 🔍 OCR — Text Extraction from Images

You copy a screenshot, a photo of a receipt, a slide from a presentation. With most apps, that image is just… an image. You can't search it. You can't copy the text from it. With PasteSpace, **the text is automatically extracted in the background** using Apple's Vision framework.

**Real-world example:**
> A colleague sends you a screenshot of an error log. You copy it. An hour later, you need to look up one of the error codes from that screenshot. You open PasteSpace, type the error code in the search bar, and the screenshot appears in your results — because PasteSpace already extracted all the text from it when you copied it.

- **Automatic** — copies an image → text extracted immediately, no buttons to press
- **Searchable** — find images by typing words that appear *inside* them
- **Copyable** — open Quick Look on an OCR image → select and copy any portion of the extracted text
- **Local** — all processing on your Mac's CPU/GPU, nothing uploaded anywhere

---

### 🪄 Data Magic — Instant Transformations

You copy data in one format and need it in another. Instead of opening a converter website, pasting, converting, and copying back — PasteSpace detects the type of data you copied and offers **one-tap transformations** right there in your clipboard history.

**Real-world examples:**

> **Developer:** You copy a minified JSON response from an API. Click 🪄 → "Pretty-print JSON" → perfectly formatted JSON is copied to your clipboard. No external tools.

> **Designer:** You copy a color value `#FF5733` from a design tool. Click 🪄 → "HEX to RGB" → `rgb(255, 87, 51)` is ready to paste into your CSS.

> **Writer:** You copy a paragraph in UPPER CASE from an old document. Click 🪄 → "To Title Case" → properly capitalized text, instantly.

> **Data analyst:** You copy a table from a spreadsheet. Click 🪄 → "Table to Markdown" → a perfectly formatted Markdown table for your documentation.

**All available transformations:**

| You copied | Available transformations |
|---|---|
| **JSON** | Pretty-print, Minify, → YAML, → XML |
| **URL with parameters** | Extract parameters, URL encode/decode |
| **Color** (`#FF5733`) | HEX ↔ RGB ↔ HSL ↔ SwiftUI Color |
| **Date** (`2026-04-11`) | → Unix timestamp, → ISO 8601, → readable |
| **Unix timestamp** | → Human-readable date |
| **Table** (tab/CSV) | → Markdown table, → JSON, → CSV |
| **HTML** | → Markdown, → plain text |
| **Markdown** | → HTML |
| **Base64** | Decode ↔ Encode |
| **Any text** | UPPER, lower, Title Case, camelCase, snake_case, kebab-case, URL slug, word count, JSON/HTML escape |
| **YAML** | → JSON |
| **XML** | → JSON |

**30+ transformations — all offline, all instant, all on your Mac.**

---

### 👁 Quick Look

Preview the full content of any item — text, images, PDFs, files — in a floating panel without leaving your current workflow. For images with extracted OCR text, you can view the full extracted text and **select specific portions** to copy.

**Real-world example:**
> You copied a long email draft two hours ago. Instead of opening Mail, you click the 👁 button in PasteSpace — the full email appears in a floating panel. You select the one paragraph you need, copy it, and paste it into your new document. All without leaving your current app.

---

### 🛡️ App Blocklist

Some apps handle sensitive data that should never enter your clipboard history — banking apps, password managers, medical software.

**Real-world example:**
> You use your banking app to check your balance. Without a blocklist, every account number and balance you copy is stored in your clipboard history. With PasteSpace, you add your banking app to the blocklist — anything copied from it is completely ignored.

---

### ⏳ Ephemeral Mode

When activated, your clipboard history is **automatically wiped when your Mac restarts or shuts down**. Vault items and pinned items are preserved.

**Real-world example:**
> You're working on a confidential project at a shared workstation. You activate Ephemeral Mode. When you shut down the Mac at the end of the day, all your clipboard history vanishes — except the items you explicitly pinned or vaulted. The next person to use the Mac finds a clean slate.

---

## Free vs. Pro

PasteSpace is **free to use** with generous limits. Every feature is available — Pro simply removes the limits.

| Feature | Free | Pro ($19.99 — lifetime) |
|---|---|---|
| Clipboard history | 10 items (rolling) | **Unlimited** |
| Pinned items | 3 | **Unlimited** |
| Vault Mode | 2 items | **Unlimited** + auto-detection |
| OCR | Latest image | **Every image** |
| Data Magic | Latest text | **Every text** |
| Quick Look | Latest text + image | **Everything** |
| App Blocklist | 1 app | **Unlimited** |
| Ephemeral Mode | — | ✅ |
| Search, copy, pin, delete, shortcut | ✅ | ✅ |
| Future updates | ✅ | ✅ |

**One purchase. No subscription. No renewal. No "premium tier." Yours for life.**

---

## Privacy

This is not a marketing line. PasteSpace **collects zero data**:

| | |
|---|---|
| ✅ No analytics | We don't track what you do |
| ✅ No crash reports | We don't know when something breaks |
| ✅ No cloud | Your data never leaves your Mac |
| ✅ No account | We don't know your name |
| ✅ No third-party SDKs | No code watching you |
| ✅ No network calls | Except Apple's StoreKit for purchases |

Everything is stored **locally** in the macOS **App Sandbox**. Your encryption key lives in the **Keychain**, hardware-backed by the **Secure Enclave**. There is no server. There is no database with your name in it. There is nothing to hack, nothing to leak, nothing to sell.

**Fully compliant with GDPR and CCPA** — not because we followed a checklist, but because there's genuinely nothing to comply about.

---

## Security Architecture

```text
┌─────────────────────────────────────────────────────┐
│                    PasteSpace App                   │
│                  (macOS App Sandbox)                │
│                                                     │
│  ┌─────────────┐  ┌────────────────────────────┐    │
│  │  Clipboard  │  │   Local SQLite Database    │    │
│  │  Monitoring │──│ • Plain items (text/files) │    │
│  │(NSPasteboard│  │ • Encrypted vault items    │    │
│  │  polling)   │  │   (AES-256-GCM ciphertext) │    │
│  └─────────────┘  │ • OCR extracted text       │    │
│                   │ • Settings (UserDefaults)  │    │
│  ┌─────────────┐  └────────────────────────────┘    │
│  │ Sensitivity │                                    │
│  │  Detector   │  ┌────────────────────────────┐    │
│  │(regex-based │  │  macOS Keychain / Secure   │    │
│  │ local-only) │  │        Enclave             │    │
│  └─────────────┘  │ • AES-256 encryption key   │    │
│                   │ • Hardware-backed (M1/M2/  │    │
│  ┌─────────────┐  │   M3/M4/T2)                │    │
│  │ OCR Engine  │  │ • Never leaves device      │    │
│  │(Apple Vision│  └────────────────────────────┘    │
│  │ framework)  │                                    │
│  └─────────────┘  ┌────────────────────────────┐    │
│                   │ Touch ID / Device Password │    │
│  ┌─────────────┐  │   (LocalAuthentication)    │    │
│  │ StoreKit 2  │  │ • Vault reveal             │    │
│  │ (Apple IAP) │  │ • On-device only           │    │
│  └─────────────┘  └────────────────────────────┘    │
│                                                     │
│        ✗ No servers  ✗ No cloud  ✗ No analytics     │
└─────────────────────────────────────────────────────┘
```

| Component | Technology |
|---|---|
| Encryption | AES-256-GCM via Apple CryptoKit |
| Key storage | macOS Keychain (Secure Enclave on Apple Silicon) |
| Authentication | Touch ID / device password via LocalAuthentication |
| OCR | Apple Vision framework (VNRecognizeTextRequest) |
| Database | SQLite via GRDB.swift |
| In-app purchase | StoreKit 2 (on-device JWS verification) |
| UI framework | SwiftUI (native macOS) |
| Export compliance | ITSAppUsesNonExemptEncryption = false (CryptoKit exempt) |

---

## System Requirements

- **macOS 14.0** (Sonoma) or later
- Any Mac (Intel or Apple Silicon)
- Touch ID recommended for Vault Mode (device password works on all Macs)
- Secure Enclave available on Apple Silicon (M1/M2/M3/M4) and T2 Macs for hardware-backed key storage

---

## Installation

**From the Mac App Store** (recommended):

1. Search for **"PasteSpace"** on the Mac App Store
2. Download (free)
3. PasteSpace appears as a 📋 icon in your menu bar
4. Click the icon to open — your clipboard history starts building immediately

**First launch:**
- A small indicator appears pointing to the 📋 icon in your menu bar
- Click it to open PasteSpace
- Everything works out of the box — no configuration needed
- Press **⌥⇧V** from any app to open PasteSpace instantly

---

## Quick Start

### Copy something → It's in PasteSpace
```text
You: ⌘C (copy anything — text, image, file)
PasteSpace: ✓ Captured silently. Searchable. Ready to paste.
```

### Find something you copied earlier
```text
You: ⌥⇧V (open PasteSpace)
You: Type "invoice" in search
PasteSpace: Here's the invoice number from 3 hours ago,
            and the screenshot of the invoice that contains the word "invoice".
```

### Pin something you use often
```text
You: Hover over your email signature → click 📌
PasteSpace: Pinned. Always at the top. One click to copy.
```

### Protect sensitive data
```text
You: Copy a credit card number
PasteSpace: Detected as sensitive → auto-encrypted → 4532 •••• •••• 6789 🔒
You: Need it later? Tap 👁 → Touch ID → revealed for a moment → auto-hidden
```

### Transform data
```text
You: Copy `{"name":"John","age":30}`
You: Click 🪄 → "Pretty-print JSON"
PasteSpace: Copied to clipboard:
            {
              "name": "John",
              "age": 30
            }
```

---

## Keyboard Shortcuts

| Shortcut | Action |
|---|---|
| **⌥⇧V** | Open/close PasteSpace (customizable) |
| **↑ ↓** | Navigate clipboard history |
| **↵ Enter** | Copy selected item |
| **⌘V** | Paste (standard macOS) |
| **Esc** | Close PasteSpace |

---

## Built for People Who Care About Their Mac

PasteSpace is **not** an Electron wrapper. It's **not** a cross-platform app ported to macOS as an afterthought. It's a **native macOS application** built with **SwiftUI** — it respects your system appearance, integrates with Touch ID, and sits quietly in your menu bar using virtually no resources when idle.

If you care about what runs on your Mac, PasteSpace was built for you.

---

## Legal

- [Terms of Use](https://pastespace.app/terms) · [Privacy Policy](https://pastespace.app/privacy)
- **© 2026 Marius Constantin Popescu. All rights reserved.**

---

## Contact

Questions, feedback, or feature requests?

📧 **mariuscpopescu@icloud.com** — I read every email.
