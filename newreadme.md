---
layout: default
title: "PasteSpace — Clipboard Manager"
description: "PasteSpace is a private clipboard history app for macOS 14+. Encrypted Vault with Touch ID, search inside images and documents, filters and sorting, Data Magic, a Quick Look text editor with versions, QR codes, Share, drag and drop, rich-text fidelity, plain-text controls — fully offline, zero data collected."
keywords: "PasteSpace, clipboard manager, macOS clipboard history, macOS 27, secure clipboard manager, encrypted clipboard, Vault, Touch ID, OCR, search inside PDF, document text search, clipboard filters, Data Magic, Quick Look text editor, QR code generator, drag and drop clipboard, multi-file clipboard, rich text clipboard, copy as plain text, paste as plain text, menu bar app, privacy-focused, offline, macOS app"
permalink: /
---

<h1 align="center">PasteSpace — Clipboard Manager</h1>

<p align="center">
  <strong>Secure clipboard history for macOS. Native. Private. Yours.</strong> · <a href="https://apps.apple.com/ro/app/pastespace-clipboard-manager/id6762815491?mt=12" rel="noopener noreferrer">Open in the Mac App Store</a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/platform-macOS%2014%2B-blue" alt="macOS 14+" />
  <img src="https://img.shields.io/badge/tested-macOS%2027%20beta-informational" alt="Tested on macOS 27 beta" />
  <img src="https://img.shields.io/badge/swift-6.0-orange" alt="Swift 6.0" />
  <img src="https://img.shields.io/badge/UI-SwiftUI-purple" alt="SwiftUI" />
  <img src="https://img.shields.io/badge/encryption-AES--256--GCM-green" alt="AES-256-GCM" />
  <img src="https://img.shields.io/badge/data%20collected-zero-brightgreen" alt="Zero Data Collection" />
  <img src="https://img.shields.io/badge/license-proprietary-lightgrey" alt="Proprietary" />
</p>

<p align="center">
  Free to use · Pro is <strong>$19.99 once, forever</strong> · No subscriptions · Works completely offline
</p>

<p align="center">
  <strong>New in 3.0:</strong> text recognition in 30 languages, search inside documents, filters and sorting, a stronger Vault and a redesigned window. <a href="#whats-new">See everything new →</a>
</p>

---

## Contents

- [The problem](#problem)
- [How PasteSpace works](#how-it-works)
- [Privacy](#privacy)
- [Your clipboard history](#history)
- [Search, filters and sorting](#search)
- [The Vault — how protection really works](#vault)
- [Security architecture](#security)
- [Text in images (OCR)](#ocr)
- [Text inside documents](#documents)
- [Quick Look and the text editor](#quick-look)
- [Data Magic](#data-magic)
- [Drag and drop](#drag-and-drop)
- [Share](#share)
- [QR codes](#qr)
- [Formatting and plain text](#plain-text)
- [App Blocklist](#blocklist)
- [Ephemeral Mode](#ephemeral)
- [Deleting and clearing](#deleting)
- [Rating PasteSpace](#rating)
- [Free vs. Pro](#free-vs-pro)
- [Every setting, explained](#settings)
- [Keyboard shortcuts](#shortcuts)
- [Questions people ask](#faq)
- [System requirements](#requirements)
- [What's new in PasteSpace 3.0](#whats-new)
- [Contact](#contact)

---

<a id="problem"></a>
## The problem

You copy a phone number, then a link, then a paragraph from a document. When you need the phone number again, it's gone — replaced by the last thing you copied. So you dig through browser history, reopen documents and scroll through messages to find it again.

**PasteSpace remembers what you copy**, so you don't have to — and it keeps the sensitive parts locked away while it does.

---

<a id="how-it-works"></a>
## How PasteSpace works

**Copy the way you always do. PasteSpace remembers it all — and hands any of it back in seconds.**

It lives in your menu bar: no window to keep open, no Dock icon, nothing to set up. Every time you copy — text, a link, an image, a file — PasteSpace adds it to a history you can search in an instant.

> **An hour ago, a client emailed you their address. Now you need it.**
> Press **⌥⇧V** — PasteSpace opens right under your pointer. Type `Bucharest`. Press **Return**, then **⌘V**. Done, without leaving the email you're writing.

**Why it's different:**

- **It finds things by what's inside them.** Search reads the words in your screenshots and — in Pro — inside your PDFs and documents, scanned ones included. You don't have to remember where something came from, only a word that was in it.
- **It locks your secrets away by itself.** Card numbers, IBANs, passwords and API keys are recognised the moment you copy them and encrypted in the Vault, behind Touch ID. Not even PasteSpace's own search can see inside them.
- **Nothing ever leaves your Mac.** No account, no cloud, no analytics, no tracking — every feature works offline. [Privacy →](#privacy)
- **It never asks to control your Mac.** PasteSpace doesn't use the Accessibility permission, which would let it watch and control everything you do. It puts your item on the clipboard, brings back the app you were in, and steps aside — the ⌘V stays yours.
- **It does more than paste.** Tidy a JSON response, convert a colour, strip the tracking from a link, edit a text before you paste it, turn it into a QR code, or drag it straight into another app.
- **It stays out of your way.** It opens under your pointer, with the pointer already on your newest copy, and closes the moment you've picked something — or stays on top while you work.

**Where it saves you time every day:**

- **Filling in forms** — your IBAN, address, ID number or email, pinned once and a shortcut away every time after. Card numbers and IBANs stay locked, and are pasted after a quick Touch ID.
- **Research and writing** — copy quotes, links and figures as you read, then paste them one by one, or select several and paste them all at once.
- **Writing code** — API tokens are locked the moment you copy them; a minified API response becomes readable JSON, or a Swift struct, in a couple of clicks.
- **Answering the same questions** — pin your standard replies and your signature, adjust them in Quick Look, and paste them formatted or as plain text.

**Opening PasteSpace:**

- **The global shortcut** — `⌥⇧V` by default, changeable in Settings. Press it again to close.
- **The menu-bar icon** — click to open or close; right-click for *Quit PasteSpace*.
- **Open at mouse cursor** (on by default) — the window appears where your pointer is, positioned so the pointer lands on your newest item, ready to click. Turn it off and the window opens under the menu-bar icon instead. Near a screen edge, the window moves just enough to stay fully visible.
- **Always on top** — keeps the window open above other apps until you close it with its ✕ or the menu-bar icon. Copying an item no longer closes it; PasteSpace simply hands focus back to your app so `⌘V` works. While it's pinned like this, the shortcut moves the window to your pointer (if *Open at mouse cursor* is on) rather than hiding it.

---

<a id="privacy"></a>
## Privacy

PasteSpace **collects no data at all**.

| | |
|---|---|
| ✅ No analytics | Nothing about how you use PasteSpace is recorded or sent. |
| ✅ No crash reports | No automatic error reports leave your Mac. |
| ✅ No cloud | Your history never leaves your Mac. There's no sync and no server. |
| ✅ No account | Nothing to sign up for. |
| ✅ No third-party code | No external SDKs, trackers or advertising. |
| ✅ No network for features | Search, OCR, document reading, Data Magic, QR codes and the Vault all work offline. |

The only connections are made by **Apple's own App Store framework**, for two things:

- **Purchasing and restoring Pro.** Verification happens on your Mac.
- **The occasional "Rate PasteSpace" request.** PasteSpace decides when to show it on your Mac alone, and macOS shows the request. Nothing about how you use PasteSpace is sent anywhere, and PasteSpace is never told whether you left a review.

Everything else is stored **locally**, inside PasteSpace's private **App Sandbox** folder. Because no personal data is collected or processed, PasteSpace is compatible with GDPR and CCPA by design.

---

<a id="history"></a>
## Your clipboard history

### What PasteSpace keeps

Whatever you copy as text, an image or a file, PasteSpace keeps:

| You copy | PasteSpace keeps |
|---|---|
| **Text** — a phone number, an address, a paragraph, a snippet of code | The text, exactly as copied. Code is recognised as code, in around 30 programming languages. |
| **Formatted text** — from a web page, Pages, Word, Notes, Mail… | The text **and** its formatting — fonts, sizes, colours, bold, italic, highlights, lists. |
| **Links** | The link, shown with a readable title derived from the address itself — PasteSpace never visits the page. |
| **Images and screenshots** — from any app, or as image files in Finder | The image, at any size, plus the text in it ([OCR](#ocr)). |
| **Documents** — PDFs (scanned ones too), Word, Pages, spreadsheets, presentations, web pages, text and code files | A reference to the file — and, in Pro, the text inside PDFs, Word, RTF and OpenDocument files, web pages and text files, so a search can find it ([more](#documents)). |
| **Any other file or folder** — archives, audio, video, apps | A reference to it, with its name, kind and size. The file itself stays where it is. |
| **Several files at once** | One item that keeps them together, so they can be copied or dragged back as a group. |
| **Passwords, card numbers, keys and other secrets** | Kept — but **encrypted in the Vault** and shown masked, whether PasteSpace recognised them or you locked them yourself ([Vault](#vault)). |

Each item records **which app it came from** and **the date and time** you copied it.

**A long history costs nothing.** PasteSpace draws only the items on screen and reads an image only when you use it, so the window opens instantly and scrolls smoothly however many screenshots and documents you keep.

### Copies that are handled differently

A few kinds of copies get special treatment, on purpose:

- **Copies from password managers** (1Password, Bitwarden, LastPass, Dashlane, KeePassXC, Enpass, NordPass, Proton Pass, RoboForm, Apple Passwords, Keychain Access) **go straight into the Vault**, encrypted — that's the default. If one can't be locked, because the free Vault is full or the Vault is switched off, it isn't stored at all rather than kept readable. If you'd rather PasteSpace left them out entirely, turn off *Capture from password managers*. [More](#vault-sources)
- **Copies an app marks as private.** Apps often tag a password or a one-time code as "concealed" or "transient" when they put it on the clipboard — a request to clipboard managers not to keep it. PasteSpace honours that request. (Password managers are the exception above: their copies go only into the Vault.)
- **Copies made in apps on your [App Blocklist](#blocklist)** aren't recorded — that's what the list is for.
- **A single copy of more than 10 MB of text** — several thousand pages in one go — isn't recorded. Images and files have no size limit.
- **Content arriving from your iPhone, iPad or another Mac through Universal Clipboard** isn't recorded.
- **Copying an item out of PasteSpace** doesn't add it a second time; the copy is noted in that item's [copy history](#history) instead.

### Copying the same thing twice

Copying something in another app that is already in your history doesn't create a duplicate. The existing item takes the new copy time and source app, and **moves back to the top**, where a fresh copy belongs — even if you had [dragged it somewhere else](#arranging) before. Only **pinned** items keep their place, so your pins don't reshuffle.

This applies to locked items too: copying a password that's already in your Vault refreshes the locked item and brings it to the top, instead of adding a second copy. And if you had **removed the protection** from that password and then copy it again from your password manager — or copy a secret PasteSpace recognises — the item **is locked again** and keeps its whole copy history, rather than staying readable next to a new locked copy.

Copying an item **from** PasteSpace — clicking it, pressing Return — **doesn't move it**: your list stays the way it was, so the item is still where your hand expects it next time. The copy is still noted in the item's [copy history](#history).

### Reading a row

Each item's text runs the full width of the window. Beneath it, a slim bar holds the item's buttons on the left and where and when it was copied on the right — so the content gets the space, and the controls stay out of the way until you need them.

Every row shows what it is at a glance:

- **An icon for the kind of content** — text, formatted text, link, image, PDF, archive, folder, app, audio, video, a group of files…
- **A small text badge on the icon** when PasteSpace has read text out of the item — words recognised in an image, or the text of a document. It's a marker, not a button: the text itself is read in Quick Look.
- **The source app and the exact date and time** at the bottom right. (Dates show the year only when it isn't the current one.)
- **An ⓘ** next to the source. Hover over it for a moment, or click it, to see what the row can't show: the kind of content and its size in characters, words and lines, the programming language of a code snippet, the full link, a file's location, kind and size, a folder's total size, an image's dimensions, whether the item is an edited version, and — if *Keep history for* is set — when it will be removed automatically. For a locked Vault item, the ⓘ says only **Protected**.
- **The item's copy history**, at the bottom of the ⓘ details: how many times it has been copied, then each copy on its own line, newest first — the date and time, and where it happened:

  ```text
  Copied: 4 times
  Oct 2, 18:20 · from PasteSpace
  Oct 2, 18:11 · in Passwords
  Oct 1, 09:02 · from PasteSpace, as plain text
  Sep 30, 14:10 · its text, from PasteSpace
  ```

  "In Safari" means you copied it in Safari; "from PasteSpace" means you copied it out of your history. The 20 most recent copies are listed, with a count of the earlier ones. Items that were already in your history before this feature existed show the last copies PasteSpace knew about, followed by *Earlier copies weren't recorded*. A locked item's copy history appears once you reveal it. Dragging an item into another app and sharing it aren't counted as copies.
- **Action buttons** along the bottom — faint until you point at the row, so the list stays calm. When you select two or more items, the rows hide their buttons and show the order you picked them in; the actions move to the selection bar.

<a id="buttons"></a>
### Buttons you don't use disappear

Every feature with a button on the rows — **Quick Look, Data Magic, QR Code and Share** — has its own switch in [Settings](#settings). Turn one off and its button disappears from **every item**, so your history shows only the tools you actually use. Turn it back on and the buttons return.

Two buttons behave differently, on purpose:

- **A locked item keeps its 👁** even when Quick Look is off, because it's the only way to reveal what's inside. It then simply shows and hides the content in the row, without opening Quick Look.
- **With the Vault switched off**, the 🔒 button stays, dimmed, and points you to the setting that turns the Vault back on.

Some buttons appear only where they make sense: Data Magic and QR codes on text, the plain-text button on formatted text, a copy-text button on images with recognised text.

### Using an item

- **Click a row, or select it with ↑ ↓ and press Return** (hold an arrow key to move quickly — the list follows as you go) — the item goes on the clipboard, the row flashes **✓ Copied**, PasteSpace closes, and your previous app comes back to the front. Press `⌘V`. (With *Always on top*, the window stays open and only hands the focus back.)
- **⌥Return** copies the selected item **as plain text**, without its formatting.
- **Formatted items also have a plain-text button**, for the same thing with the mouse.

### Pinned items

Pin the things you paste often — your email signature, an address, a template — and they stay in a **Pinned** section above the rest of your history.

- Pinned items **never expire** and **don't count** toward your history limit.
- The **PINNED (4) ▸** header folds the section away with one click when the pinned list gets long — your recent copies then start right at the top. PasteSpace remembers the choice. When you search, pinned matches are always shown, folded or not.
- Both headers show their counts — *PINNED (4)*, *RECENT (103)* — while the footer shows the total.
- Free: up to 3 pinned items. Pro: as many as you like.

<a id="arranging"></a>
### Arranging your history

Drag an item up or down the list to put it where you want it. A blue line shows where it will land. Hold it near the top or bottom edge of the list and the history scrolls to follow — slowly at first, faster the closer you get to the edge — so you can move an item anywhere, not only among the ones on screen. Your arrangement is kept — until you copy that item again in another app, which brings it back to the top as its newest copy. Copying it *from* PasteSpace leaves it where it is.

Reordering is switched off while a search or a filter is active, or when the list is sorted by something other than your own order: dropping an item between two of the visible rows would put it in an unpredictable spot among the hidden ones.

### Working with many items at once

- **⌘-click** a row, or press **⌘Return** on the focused row, to add it to a selection. Each selected row shows its number in the order you picked it.
- **⇧-click** selects every row between the last one you picked and this one.
- A bar appears with actions for the whole selection: **Copy**, **Copy all as plain text**, **Reveal all in Finder**, **Pin all**, **Protect all with Vault**, **Delete all**, and **Clear selection** (or **Esc**). You can also drag the whole selection into another app.
- When you copy several items together, they're joined with a separator you choose in Settings — a new line by default, or a tab, a comma, anything you like.
- If a search hides some of the selected items, the bar tells you how many — they're still part of the selection.
- Tools that only make sense for one item at a time — Quick Look, Data Magic, QR codes — stay on the individual rows.

### How long items are kept

Two settings work together:

- **History limit** — how many items to keep. When it's reached, the oldest items make room for new ones. Pinned and Vault items don't count toward the limit and are never removed by it. Free: 10 items. Pro: any number, or unlimited.
- **Keep history for** — *Forever* (the default), *1 day*, *7 days* or *30 days*. Items older than that are removed automatically. Copying an item again restarts its time; unpinning an item gives it a fresh period. Pinned and Vault items never expire.

PasteSpace also keeps, privately on your Mac, a record of every time each item is copied — the copy history in its ⓘ details — and counts how often you use each item from PasteSpace, which powers the *Most used* and *Recently used* sort orders. When an item is deleted, its records go with it. None of this is ever shared or leaves your Mac.

---

<a id="search"></a>
## Search, filters and sorting

### Search

Type in the field at the top and the list narrows as you type. PasteSpace searches:

- the **text** of every item,
- **file names**,
- the **name of the app** each item was copied from,
- **text recognised in images** ([OCR](#ocr)),
- **text inside documents** ([Pro](#documents)).

How matching works:

- Words match **from their beginning**: `inv` finds *invoice*, but `voice` doesn't find *invoice*.
- Several words narrow the search: `invoice march` finds items containing both.
- **Accents don't matter**: `cafe` finds *café*, `sosea` finds *Șosea*.
- **Locked Vault items never appear in search results** — not even when you type words that are inside them. [Here's why](#vault-search).

### Filters

The filter button inside the search field opens the filters. **Every filter in use is shown as a chip under the search field**, with an ✕ to remove it, plus *Clear all* — so a forgotten filter can never make it look as if part of your history has vanished. Filters reset every time PasteSpace starts.

**Kind** (free) — what the item is. Choose several and you'll see all of them:

| Text | Media | Files |
|---|---|---|
| Plain text | Images | Documents (PDF, Word, Pages, spreadsheets, presentations, e-books, text files) |
| Formatted text | Audio | Archives (ZIP, RAR, 7-Zip, disk images, installers…) |
| Links | Video | Folders |
| Code (snippets *and* source files, JSON, YAML, XML, HTML) | | Multiple files |
| Passwords | | Other files — anything none of the kinds above describe |
| Keys & tokens | | |
| Cards & IBANs | | |
| Personal IDs | | |

PasteSpace works out the kind from **what the item actually contains**, not just from how it arrived: a link copied as text is a *Link*; a screenshot copied as a file in Finder is an *Image*; a snippet of Swift code is *Code*; a `.rar` or `.mkv` is recognised even on a Mac with no app that opens it.

**Advanced** (Pro) — combine any of these with kinds and with search:

- **When** — Today, Last 7 days, Last 30 days.
- **State** — Pinned, Protected (in the Vault), Edited (versions saved from Quick Look), Has extracted text.
- **Source app** — the apps that actually appear in your history, most frequent first.

In the free version the advanced part of the filter panel is visible but dimmed.

### Sorting

The sort menu next to the filter button changes the order of the list:

*Custom order* (yours — the default) · *Newest first* · *Oldest first* · *Largest first* · *Smallest first* · *Source app* · *Kind* · *Most used* · *Recently used*

Any order other than *Custom* is a temporary view: your own arrangement is kept untouched underneath, and choosing *Custom order* again brings it back exactly. The sort you choose is remembered between launches (unlike filters), and while it's active it appears as a chip too, so you always know why the list looks the way it does. Sorting is free.

---

<a id="vault"></a>
## The Vault — how protection really works

The Vault is where PasteSpace keeps things that shouldn't be readable by anyone glancing at your screen, searching your history, or opening PasteSpace's files: passwords, card numbers, bank details, API keys, private notes.

Unlike apps that merely *hide* such items behind dots, PasteSpace **encrypts** them. This section explains exactly what happens, so you can see for yourself that it works.

<a id="vault-sources"></a>
### How items get into the Vault

**1. Automatically, when PasteSpace recognises a secret.** As each copy arrives, PasteSpace checks it — on your Mac, never anywhere else — against patterns for:

| Recognised | Checked how |
|---|---|
| Card numbers | The number must pass the Luhn checksum every real card number passes, so random 16-digit numbers aren't mistaken for cards. |
| IBANs | The country code, the length for that country and the check digits must all be valid. |
| Personal ID numbers — US Social Security numbers, Romanian CNPs | The CNP's control digit is verified. |
| API keys and tokens — GitHub, GitLab, Slack, OpenAI, Anthropic, Google, AWS, Stripe, Shopify, DigitalOcean, Hugging Face, PyPI, Telegram bots, JWTs, bearer tokens | Each provider's own recognisable format. |
| SSH private keys, PEM keys, SSH fingerprints | Their standard headers and formats. |
| Database connection strings and secret environment variables | `postgres://user:password@…`, `API_SECRET=…` and similar. |
| Software licence keys | Typical licence-key formats. |
| Passwords | A single word of 8–64 characters containing **an uppercase letter, a lowercase letter, a digit and a symbol**. |
| Username + password pairs, crypto seed phrases | Their typical shapes. |
| One-time codes | Only when copied from an authenticator app — a 6-digit number from anywhere else is just a number. |
| Long random-looking strings | Must also contain at least one digit. |

The rules are strict on purpose: it is better to occasionally miss a secret than to lock away ordinary text you then have to unlock every time. Two examples: `iPhone15Pro2024` has no symbol, so it is *not* treated as a password; a symbol name copied from a debugger, such as `_NSDetectedLayoutRecursion`, has no digit, so it is *not* treated as a key. **If something sensitive isn't recognised, lock it yourself** with one click on its 🔒 button.

**2. By hand.** Click 🔒 on any item — text, a link, an image, a file, a group of files — or select several and choose *Protect all with Vault*.

**3. From password managers.** Copies from the password managers listed [above](#history) are normally never recorded at all. With *Capture from password managers* on (the default), they're recorded **straight into the Vault**, encrypted. A password-manager copy is **never stored unlocked**: if it can't go into the Vault — because the free Vault is full, or the Vault is switched off — it isn't recorded at all, exactly as if the option were off. Turn the option off and PasteSpace goes back to ignoring them completely.

You can switch automatic detection off in Settings and keep only manual locking, or turn the Vault off entirely.

### What happens the moment an item is locked

1. **The item is encrypted with AES-256-GCM**, using Apple's CryptoKit. Encrypted together with it: its **formatting** (the formatted copies of the text), any **text recognised in it** (if it's an image), and any **text extracted from it** (if it's a document). Each of those would otherwise spell out the same words in readable form.
2. **It disappears from the search index.** From now on, no search can find it by its contents. [Why](#vault-search).
3. **A masked preview** is made, so you can still tell your items apart (see below).
4. **Its duplicate-detection fingerprint is replaced** by one that is useless without your key. [Why](#vault-fingerprint).
5. **It stops expiring** and stops counting toward your history limit. It survives *Clear history* and *Ephemeral Mode*.
6. If it was an **edited version** from Quick Look, its link to the original — which is stored as readable text — is removed.

Encryption uses a key that is unique to your Mac (see [Where the key lives](#vault-key)). Without that key, a locked item is just unreadable data.

### What a locked item shows

| You copy | Locked as | You see |
|---|---|---|
| `Hunt3r2!xQ` | Password | `••••••••` 🔒 |
| `4242 4242 4242 4242` | Card number | `•••• 4242` 🔒 |
| `RO49 AAAA 1B31 0075 9384 0000` | IBAN | `RO•• •••• 0000` 🔒 |
| `123-45-6789` | Social Security number | `••••••••` 🔒 |
| `ghp_1234…wxyzAB` (a 40-character GitHub token) | Key / token | `ghp_••••••••yzAB` 🔒 |
| A private note you lock yourself | — | at most a quarter of its first line, e.g. `Meet••••••••lock` |
| `iPhone15Pro2024` | Not recognised | `iPhone15Pro2024` — lock it yourself if it's secret |

The rules behind the previews:

- **Passwords and personal ID numbers show only dots.** No part of them is harmless.
- **Cards show the last four digits**, the way a bank statement does — enough to tell your cards apart.
- **IBANs show the country code and the last four characters.**
- **Everything else shows at most a quarter of the first line**, split between its beginning and end, and nothing at all if it's shorter than 12 characters.
- **There are always eight dots**, whatever the length — the preview doesn't even tell you how long the secret is.
- **Locked links** show a masked page title; **locked files** show a masked file name.

### Using a locked item

Every action that needs the real content asks for **Touch ID — or your Mac's password** on a Mac without Touch ID — first. Nothing is decrypted until you've authenticated.

| You want to… | What happens |
|---|---|
| **See it** | Click 👁 → authenticate → the content appears in the row. Click 👁 again to open it in Quick Look. |
| **Copy it** | Click it (or press Return) → authenticate → it's copied, and stays locked. |
| **Copy several** | Select them and copy → **one** authentication covers all of them. |
| **Open it in Quick Look** | Opens only after authentication, and locks again when you close the panel. |
| **Use Data Magic or make a QR code** | Authenticate first; the item locks again when you're done. |
| **Share it** | Authenticate first; it locks again afterwards. |
| **Open a locked link or file** | Authenticate first. |
| **Drag it into another app** | The authentication prompt appears **when you drop**, not before — and the content is decrypted only after you've authenticated. Dragging several locked items asks **once**. |
| **Delete it** | Authenticate first, so nobody can quietly erase what you've protected. |
| **Remove its protection** | Authenticate; the item is decrypted back into a normal item, and becomes searchable again. |

**Why some items can be copied without Touch ID and others can't.** Once you've **revealed** an item (with 👁), you've already proved it's you. Until it locks again, it behaves like a normal item: click to copy, drag it as text or as the real file — no further prompts. A locked item that hasn't been revealed always asks.

**When revealed items lock again:** when you close the PasteSpace window, when you close the item's Quick Look panel, and — if *Always on top* keeps the window open — right after you copy. Revealing is meant to last moments, not hours.

<a id="vault-search"></a>
### Why locked items don't appear in search

Searching works by looking words up in an index. If a locked item's words stayed in that index, anyone at your Mac could **confirm what's inside it without authenticating** — type a guessed password, a name or an account number, and watch whether a locked item appears. The search would leak the secret one guess at a time.

So when an item is locked, its words are removed from the index entirely — including the text recognised in a locked image and the text of a locked document, and the full path of a locked file (its masked name is all the row shows). A locked item is findable only by what it shows, which is nothing. Every time PasteSpace starts, it also re-checks that no locked item has anything left in the index.

You can still find locked items by **filtering**: the *Protected* state shows every locked item, and kinds such as *Passwords* or *Cards & IBANs* include locked ones. Those filters tell you an item *is* a password — never what the password is.

### Why some things stop working while an item is locked

Each of these follows from the same principle: **PasteSpace never decrypts your content unless you've just authenticated.**

| While locked | Why |
|---|---|
| Not found by search | See above — search would leak the contents. |
| No new text recognition or document reading | Reading the content would mean decrypting it without you. Text already read before locking is kept — encrypted — and comes back when you remove the protection. |
| No "text found" badge, and skipped by the *Has extracted text* filter | Both would reveal something about what's inside. |
| No *Original ⇄ Edited* versions | The original version is stored as readable text; keeping the link would undo the protection. |
| Quick Look, Data Magic, QR codes, Share, copy, drag, open, delete — all ask first | Each needs the real content. |
| No row details beyond "Protected" | The details (size in words, file location, image dimensions…) describe the content. |

<a id="vault-fingerprint"></a>
### Copying a locked secret again

To avoid duplicates, PasteSpace gives each item a fingerprint of its contents. For ordinary items that's a standard fingerprint. For locked items, a standard fingerprint would be dangerous: anyone holding PasteSpace's database file could compute fingerprints of guesses — every possible PIN, every card number ending in the four digits a preview shows — and compare. So a locked item's fingerprint is computed **with your secret key**; without the key it reveals nothing.

What this means in practice:

- **Copying a locked secret again refreshes the locked item** instead of adding a readable copy beside it.
- **Copying again a secret you had unlocked locks it again.** If you removed the protection from a password and later copy that same password from your password manager — or copy a secret PasteSpace recognises — the existing item is locked again and the new copy merges into it, with its full copy history. It never stays readable beside a new locked duplicate.
- **A new copy that gets locked automatically** is never merged into an older, unlocked item — that would leave the secret readable.

<a id="vault-key"></a>
### Where the key lives

- PasteSpace creates one **256-bit key** for your Vault, on your Mac.
- It's stored in **your macOS Keychain**, marked **available only while your Mac is unlocked** and **only on this Mac** — it is never synced to iCloud or to other devices.
- A backup copy sits in PasteSpace's own **private, sandboxed folder** (readable only by your user account), so the Vault keeps working even if the Keychain entry is lost.
- The key never leaves your Mac, and PasteSpace has no server that could receive it.

*A note on the Secure Enclave:* earlier versions of this page said the key was protected by the Secure Enclave. That isn't accurate — the Secure Enclave can't hold this kind of encryption key — and the description above is how PasteSpace actually works.

### What the Vault protects you from — and what it doesn't

It's important to be honest about this.

**The Vault protects your secrets from:**

- **Anyone looking at your screen**, or using your Mac while you're away — they see masks, and every action asks for Touch ID or your password.
- **Search** — nobody can probe your locked items by typing guesses.
- **Someone who gets hold of PasteSpace's database file** on its own — it contains only encrypted data, previews that give nothing away, and fingerprints that are useless without the key.

**It can't protect against:**

- **Someone who knows your Mac's password** — they can authenticate, just as you can.
- **Malicious software running under your account** with full access to your files and Keychain.
- **The files themselves.** Locking a *file* item protects PasteSpace's record of it — its name and location, behind Touch ID. The file on your disk stays exactly where and as it is; PasteSpace doesn't encrypt files.

### Dragging locked documents into some apps

When you drag a locked item, PasteSpace promises the destination a file and writes it only after you authenticate. Finder, Mail, Notes and most Mac apps wait for that. Some apps built on web technology — **WhatsApp**, for example — read the file the instant you drop it, before you've had a chance to authenticate, and end up with an empty file. That's how those apps handle drops; writing the file earlier would mean decrypting it before you've proved it's you. **Reveal the item first (👁), then drag it** — a revealed item is dragged as the real thing.

### Limits

- **Free:** the Vault holds **2 items**, whether locked automatically or by hand. Once it's full, secrets you copy in ordinary apps are no longer locked automatically — they're stored like any other item. Copies from password managers are the exception: they are **not recorded at all** until there's room in the Vault again. Pro removes the limit.
- **Clear Vault** in Settings deletes every locked item at once, after authentication.
- Turning the Vault off doesn't delete what's already in it.

---

<a id="security"></a>
## Security architecture

How the pieces fit together — everything inside one sandboxed app, on your Mac:

```text
┌──────────────────────────────────────────────────────────────┐
│                 PasteSpace  (macOS App Sandbox)              │
│                                                              │
│  ┌──────────────┐   ┌──────────────────────────────────────┐ │
│  │  Clipboard   │   │        Local SQLite database         │ │
│  │  monitoring  │──▶│ • Ordinary items (text, files…)      │ │
│  └──────┬───────┘   │ • Vault items: content, formatting,  │ │
│         │           │   extracted & recognised text —      │ │
│  ┌──────▼───────┐   │   all AES-256-GCM ciphertext         │ │
│  │ Sensitivity  │   │ • Masked previews, keyed fingerprints│ │
│  │  detector    │   │ • Search index — never Vault content │ │
│  │ (on-device)  │   └──────────────────────────────────────┘ │
│  └──────────────┘                                            │
│  ┌──────────────┐   ┌──────────────────────────────────────┐ │
│  │ Vision OCR   │   │  Vault key (256-bit)                 │ │
│  │ (sandboxed   │   │ • macOS Keychain: this Mac only,     │ │
│  │ helper),     │   │   available only while unlocked      │ │
│  │ PDFKit       │   │ • Backup in the private app folder   │ │
│  └──────────────┘   │ • Never leaves the Mac               │ │
│  ┌──────────────┐   └──────────────────────────────────────┘ │
│  │ StoreKit 2   │   ┌──────────────────────────────────────┐ │
│  │ (purchases,  │   │ Touch ID / Mac password              │ │
│  │ rating ask)  │   │ (LocalAuthentication, on-device)     │ │
│  └──────────────┘   └──────────────────────────────────────┘ │
│                                                              │
│     ✗ No servers   ✗ No cloud   ✗ No analytics   ✗ No SDKs   │
└──────────────────────────────────────────────────────────────┘
```

---

<a id="ocr"></a>
## Text in images (OCR)

When you copy an image — a screenshot, a photo, a scan — PasteSpace **reads the text in it**, in the background, using Apple's Vision framework, entirely on your Mac.

> **Example:** You take a screenshot of an error dialog. Days later you remember only the error code. You type the code into PasteSpace's search, and the screenshot appears.

- **30 languages**, and the language of each image is **detected automatically** — you don't choose it:

  - **Latin script** — English (US), French, Italian, German, Spanish, Portuguese (Brazil), Dutch, Danish, Norwegian, Norwegian Bokmål, Norwegian Nynorsk, Swedish, Polish, Czech, Romanian, Turkish, Indonesian, Malay, Vietnamese
  - **Cyrillic** — Russian, Ukrainian
  - **East and Southeast Asian scripts** — Chinese (Simplified and Traditional), Cantonese (Simplified and Traditional), Japanese, Korean, Thai
  - **Arabic script** — Arabic, Najdi Arabic

  The languages come from macOS itself: all 30 are available on macOS 26, earlier versions of macOS recognise fewer, and PasteSpace always uses every one your Mac offers. The languages you've set for your Mac are tried first, so a page in your own language is read by its own model.
- Images copied as **files** in Finder are read too — **of any size**.
- Large images are scaled down for reading only; the image you copied is never changed.
- Reading runs in a **separate, sandboxed helper** inside PasteSpace, with no network access and no access to your files. Recognition needs about 100 MB, and the helper quits after 30 seconds without work, so that memory goes back to your Mac instead of staying with PasteSpace all day.
- Open the image in **Quick Look** and switch between **Preview** and **Extracted text**. The text can be selected and copied — and **edited**: correct a word the recognition misread, save, and the corrected text becomes a new item, linked to the image as its edited version ([Versions](#quick-look)).
- Images with recognised text carry a small **text badge** on their icon.
- Recognised text is plain text: image recognition reports words, not fonts or colours.
- **Locked images** aren't read; text read before locking is kept, encrypted.
- Turn it off in Settings with *Text recognition in images (OCR)*.
- **Free:** you can open and copy the text of your latest image. **Pro:** every image.

---

<a id="documents"></a>
## Text inside documents *(Pro)*

PasteSpace reads the text of the documents you copy in Finder, so searching for a word finds the file that contains it — not only files with that word in their name.

> **Example:** You copied a dozen contracts last month. You need the one mentioning "termination fee". Search for it, and PasteSpace shows the PDF.

**What it reads:**

| Document | How |
|---|---|
| PDFs with a text layer | Page by page, with their original fonts, sizes and colours. |
| Scanned PDFs (no text layer) | Every page is recognised like an image, one after another in the background — a long scan takes a few minutes. |
| Word (`.doc`, `.docx`), RTF, OpenDocument text | With their formatting. |
| HTML pages and web archives | With their formatting — fonts, sizes, weights, colours, highlights, links, lists — read from the page's own style sheets, including those saved inside a web archive. Nothing the page refers to is ever downloaded. |
| Plain text and source-code files | As they are, in whatever encoding they were saved — UTF-8 and UTF-16, and the older national ones such as Windows-1250, Windows-1251, Shift-JIS, GB18030, Big5 or KOI8-R, recognised automatically. |

**What you can do with it:**

- **Search** — the document's words are added to the search index.
- **Quick Look** opens the document with two tabs: **Preview** (the document itself) and **Extracted text**.
- When the document had formatting, the extracted text keeps it, and you get **Copy formatted** *and* **Copy as plain text** — for the whole text or for what you've selected. A plain `.txt` file or a single-font PDF just gets **Copy**.
- The text can be **edited** — fix what a scan misread, keep just the paragraph you need — and saved as a new item, linked to the document as its edited version.
- The ⓘ details report how much text was read, and whether it's formatted.

**Limits and behaviour:**

- **No document is skipped for being big.** PasteSpace keeps up to **200,000 characters** of text from every document, whatever its size — from up to the first **100 pages** of a PDF's text, and from every page of a scanned PDF. A 4,000-page manual would take seconds to read in full; the first hundred pages take a fraction of a second. Reading happens in the background, so even a very large file never slows the window down.
- Documents copied before you upgraded, or before this feature existed, are read gradually — up to 50 each time PasteSpace starts. Scanned PDFs that were read when only their first five pages were recognised are read again once, the same way, so their whole text becomes searchable.
- **Locked documents aren't read** — PasteSpace would have to decrypt them without you. Text read before locking is kept, encrypted, and returns when you remove the protection.
- Turn it off with *Text extraction from documents*. Text already read stays searchable.

---

<a id="quick-look"></a>
## Quick Look and the text editor

Quick Look opens any item in a floating panel, with room to read it — and, for text, to edit it.

### Reading

- **Text** — the whole text, with its formatting adjusted so it's readable in both Light and Dark mode. (Only the display is adjusted: copying, pasting and dragging always use the formatting exactly as captured.)
- **Images** — the full image, and a separate *Extracted text* tab when it contains text.
- **Documents** — a *Preview* tab with the document itself, and an *Extracted text* tab ([Pro](#documents)). Web pages and web archives open straight on their text, formatted from the page's own style sheets: macOS can't draw a web page inside a sandboxed app's preview, and drawing it with a web engine of our own would fetch whatever the page links to.
- **Other files** — the standard macOS preview.
- **Selecting text** shows a small floating button to copy just the selection — **Copy formatted** and **Copy as plain text** when the text has formatting, **Copy selection** when it doesn't.

### Finding

Press **⌘F**, or click the **🔍** at the right of the title bar, and a find bar opens above the text — while reading and while editing alike. Every match is highlighted, the current one more strongly, and the count reads **3 of 12**.

- **Return** or **⌘G** goes to the next match, **⇧Return** or **⇧⌘G** to the previous one. If you've clicked somewhere in the text in the meantime, the search carries on from there.
- Upper and lower case don't matter, and neither do accents.
- Select a word before pressing **⌘F** and the search starts with it.
- In the editor the matches follow your typing, so you can keep the bar open while you correct each one.
- **Esc** or **Done** closes the bar and leaves the match you were on selected — in the editor, the cursor is right there.
- On a document or image, **⌘F** switches to the *Extracted text* tab for you; the file's own preview can't be searched.

The highlights are only drawn on screen: they never become part of the text you save or copy. What you search for stays inside PasteSpace — it isn't shared with the find field of other apps.

### Editing

Click **Edit** for a full rich-text editor:

- **undo and redo** — the ↶ ↷ buttons at the start of the toolbar, or **⌘Z** and **⇧⌘Z**. They take back formatting as well as typing, and a whole typed run goes back in one step;
- font family and size, **bold**, *italic*, underline, ~~strikethrough~~;
- text colour and highlight colour, each from a 27-colour palette;
- clear the formatting of selected characters;
- alignment — left, centre, right, justified;
- bulleted and numbered lists.

**If the original was plain text**, the characters you didn't touch are pasted using the destination app's own font and colour — white on a dark page in Pages, the body font in Word — and only what you actually formatted carries your styling.

### Versions — saving never overwrites

**Save** creates a **new item** in your history; the original stays exactly as it was. Editing an edit adds another version of the same family. In view mode Quick Look shows a version strip — **Original | Edited · 2 of 3** — so you can step between them, and **Show in History** jumps to the version you're looking at in the list.

This works for text recognised in images and documents too: correct a word in the text of a scanned receipt, save, and the corrected text becomes a new version linked to that image.

### Copying

**Copy Edited** puts the edited text on the clipboard right away. For formatted text, you choose **Copy formatted** or **Copy as plain text**. There's deliberately no "copy everything" button for the extracted text of images and documents — select what you need.

**Free:** Quick Look opens your latest text and latest image. **Pro:** everything.

**Locked items** open in Quick Look only after authentication and lock again when you close the panel.

---

<a id="data-magic"></a>
## Data Magic

Click 🪄 on a text item and PasteSpace offers **transformations that fit what you copied** — it looks at the content first, and shows only the actions that make sense for it. A colour gets colour conversions, a table gets table conversions, a link with tracking parameters gets *Remove Tracking from Link* (and a link without them doesn't). General-purpose text tools are tucked under **Text tools**, and only the ones worth using on that content are offered — case changes are offered for prose but not for a table or a colour.

Pick an action and the result is copied, ready to paste. The original item stays unchanged.

> **Developer:** Copy a minified API response → 🪄 → *Pretty Print JSON*, or *JSON → Swift struct*.
> **Designer:** Copy `#FF5733` → 🪄 → *Hex → RGB* → `rgb(255, 87, 51)`.
> **Analyst:** Copy cells from a spreadsheet → 🪄 → *To Markdown Table*.
> **Everyone:** Copy a long link from a newsletter → 🪄 → *Remove Tracking from Link*.

**All 57 transformations:**

| Content | Transformations |
|---|---|
| **Code** | Remove Indentation · Tabs → Spaces · Spaces → Tabs · Strip Line Numbers · Remove Comments · Join into One Line · Escape as String Literal · Wrap as Markdown Code Block · Format SQL |
| **JSON, YAML, XML** | Pretty Print JSON · Minify JSON · Sort JSON Keys · JSON → YAML · JSON → XML · JSON → Swift struct · JSON → TypeScript interface · YAML → JSON · Pretty Print XML |
| **Tables** (tab- or comma-separated) | To Markdown Table · To JSON Array · To CSV |
| **Links** | Extract URL Parameters · Remove Tracking from Link · URL Encode · URL Decode · Generate URL Slug |
| **Colours** | Hex → RGB · Hex → HSL · Hex → SwiftUI Color · RGB → Hex |
| **Dates and timestamps** | To ISO 8601 · To Unix Timestamp · To Readable Date |
| **Encoding** | Decode Base64 · Encode to Base64 · Escape for JSON · Escape for HTML |
| **HTML and Markdown** | HTML → Markdown · Markdown → HTML |
| **Letter case** | To camelCase · To snake_case · To kebab-case · To UPPERCASE · To lowercase · To Title Case · To Sentence case |
| **Everyday text** | Clean Up Text · Extract Links · Extract Email Addresses · Extract Phone Numbers · Sort Lines A → Z · Remove Duplicate Lines · Number the Lines · Add Up Numbers · Calculate Result · Normalize Phone Number · Remove Diacritics |

Everything runs offline, on your Mac. Code detection recognises around 30 programming languages plus JSON, HTML, XML and YAML.

**Free:** your latest text item. **Pro:** every text item. Locked items ask for authentication first.

---

<a id="drag-and-drop"></a>
## Drag and drop

Drag items **out of** PasteSpace straight into other apps:

- **Text** into a text field, a document or a message — it's inserted where you drop it.
- **Links** into a browser, a note or an email.
- **Images** into a document or a chat.
- **Files and groups of files** into Finder, Mail, Slack and other apps — as the real files, not shortcuts.
- **A whole selection at once** — text items are joined with your separator, files arrive as files, locked items as promised files.
- **Locked items** — the authentication prompt appears when you drop, the content is decrypted only after you've authenticated, and several locked items need only **one** authentication. Some web-based apps such as WhatsApp can't receive locked documents this way — [reveal them first](#vault).
- **Revealed items** (unlocked with 👁) are dragged as what they really are — text as text, a file as the file — alone or in a selection, with no further prompt.

Every kind of item has been tested this way — text, links, images, single files, groups of files, locked and revealed Vault items, and mixed selections — both into Finder and Apple's apps and into third-party apps, including those built on web technology, such as Slack and WhatsApp, which are the fussiest about what they accept:

- files arrive as real files under their own names, never as unnamed data;
- a multi-selection arrives whole — no item is dropped on the way;
- the picture under your pointer matches the item, whatever its kind;
- with *Always on top*, a drag starts on the very first click, even while another app is in front.

Dragging an item **within** the list rearranges your history ([see above](#history)). Nothing is ever added to your history by dropping onto PasteSpace.

---

<a id="share"></a>
## Share

The Share button sends any item — text, link, image, file or group of files — through the services on your Mac: **Messages, Mail, AirDrop, Notes**, and any other app that offers sharing.

- Files stay accessible to the service you chose until it has finished with them.
- **Locked items** ask for authentication first, and lock again afterwards. For locked text, the plain text is shared.
- PasteSpace makes no network connection of its own — the service you pick does the sending.
- Free in both versions. Hide the button in Settings if you don't use it.

---

<a id="qr"></a>
## QR codes

Click the QR button on a text item to turn it into a **scannable QR code**, shown in a floating panel that stays on screen while you work.

> **Wi-Fi for a guest:** copy the network password → QR → they scan it with their phone.
> **A link to your phone:** copy a URL → QR → scan it to open the page on mobile.
> **Contact details:** copy a phone number or email → QR → nobody has to type it.

Generated entirely on your Mac with Apple's Core Image — nothing is sent anywhere. **Free:** your latest text item. **Pro:** every text item. Locked items ask first.

---

<a id="plain-text"></a>
## Formatting and plain text

PasteSpace keeps formatted text exactly as you copied it. When you'd rather have plain text, you decide when:

| You want | Use |
|---|---|
| Never to keep formatting at all | **Always copy as plain text** — formatted text is recorded as plain text from then on. |
| To keep formatting in history but always paste plain | **Always paste as plain text** — your history keeps the formatting; everything you paste is plain. |
| Plain text just this once | **⌥Return**, the plain-text button on the row, or **Copy as plain text** in Quick Look. |
| Part of a formatted text | Select it in Quick Look → **Copy formatted** or **Copy as plain text**. |

> **Example:** you're writing in a note-taking app and want every paste to match your document — no headings, colours or size jumps from the web page you copied from. Turn on *Always paste as plain text*, and your history still keeps the original formatting for the day you need it.

---

<a id="blocklist"></a>
## App Blocklist

Tell PasteSpace to ignore certain apps completely. Anything copied in a blocked app is never recorded — not even briefly.

> **Example:** add your banking app, or the software you use for medical records, and nothing you copy there ever reaches your history.

**Free:** 1 app. **Pro:** unlimited.

---

<a id="ephemeral"></a>
## Ephemeral Mode *(Pro)*

For when you want a clean slate every day. With Ephemeral Mode on, your history is erased whenever PasteSpace quits — including when your Mac restarts or shuts down.

- **When you quit, PasteSpace asks first.** A window shows exactly what will happen — what will be erased and what will be kept — with **Confirm and Quit** and **Cancel**. Cancel (or Esc) keeps PasteSpace running with your history untouched.
- **The same question appears when your Mac is about to log out, restart or shut down.** There, Cancel also stops the log out, restart or shut down. If nobody answers within **20 seconds**, PasteSpace goes ahead and erases your history as promised — an unattended Mac is never kept from shutting down.
- **Vault items are always kept.**
- **Pinned items are kept** too, unless you turn off *Keep Pinned items*.
- The erasing is completed the next time PasteSpace starts, before any history is shown. Doing it at startup means it still happens even if your Mac shut down before PasteSpace could finish quitting.
- Erased items can't be recovered.

---

<a id="deleting"></a>
## Deleting and clearing

| Action | What it removes | Confirmation |
|---|---|---|
| Delete an item | That item | Asks you to confirm |
| Delete a locked item | That item | Touch ID or your password |
| Delete a selection | Every selected item | Asks you to confirm — and authentication if any are locked |
| Clear history (🗑 in the footer) | Everything **except** pinned and Vault items | Asks you to confirm |
| Clear Pinned (Settings) | All pinned items | Asks you to confirm |
| Clear Vault (Settings) | All Vault items | Touch ID or your password |

Deleted items can't be recovered.

---

<a id="rating"></a>
## Rating PasteSpace

**If PasteSpace saves you time, a rating on the App Store is the most helpful thing you can do in return.**

- **It's how other people find PasteSpace.** The App Store leans heavily on ratings and reviews when it decides which apps to show. A few honest words from someone who uses PasteSpace every day count for more than anything written on this page.
- **It's the only feedback PasteSpace gets.** PasteSpace collects no analytics and no usage data — that's a promise, not a setting. There is no dashboard showing which features you rely on or what gets in your way. Your review is how I find out, and it shapes what comes next.
- **It keeps PasteSpace independent.** Every person who discovers PasteSpace through your review helps keep it what it is: no ads, no subscription, no data collection.
- **It takes less than a minute.** Open Settings and click **Rate PasteSpace on the App Store** at the bottom — it takes you straight to the review page. The stars alone help; a sentence about what you use PasteSpace for helps even more.

Now and then, macOS may also show its own rating request — three times at most, always at a quiet moment, and never again once you've used the Rate button in Settings. PasteSpace never sees your rating, and nothing about how you use it leaves your Mac.

Something not working the way you'd expect? Write to me as well — I read every email, and a review that describes a problem helps get it fixed for everyone.

---

<a id="free-vs-pro"></a>
## Free vs. Pro

PasteSpace is **free to use**. Pro removes the limits and adds the power tools — for a **single payment**, yours for life.

| | Free | Pro ($19.99, lifetime) |
|---|---|---|
| Clipboard history | 10 items (rolling) | **Unlimited** |
| Pinned items | 3 | **Unlimited** |
| Vault | 2 items | **Unlimited** |
| Text in images (OCR) | Latest image | **Every image** |
| Text inside documents | — | ✅ |
| Quick Look + editor | Latest text and image | **Everything** |
| Data Magic | Latest text | **Every text** |
| QR codes | Latest text | **Every text** |
| Search and filter by kind | ✅ | ✅ |
| Sorting (all nine orders) | ✅ | ✅ |
| Filter by date, state and source app | — | ✅ |
| App Blocklist | 1 app | **Unlimited** |
| Ephemeral Mode | — | ✅ |
| Share, drag and drop, multi-selection | ✅ | ✅ |
| Formatted text, plain-text controls | ✅ | ✅ |
| Keep history for, item details, reordering | ✅ | ✅ |
| Future updates | ✅ | ✅ |

Buy Pro inside the app (Settings, or any **PRO** badge), or directly from PasteSpace's page on the Mac App Store.

**One purchase. No subscription. No account.**

---

<a id="settings"></a>
## Every setting, explained

| Setting | Default | What it does |
|---|---|---|
| Launch at login | Off | Starts PasteSpace when you log in. |
| Open at mouse cursor | On | Opens the window at your pointer, with the pointer on your newest item. |
| Always on top | Off | Keeps the window open above other apps until you close it. |
| Global shortcut | ⌥⇧V | The keys that open and close PasteSpace from any app. |
| Sound on copy | On | A short sound when you pick an item. |
| Always paste as plain text | Off | Everything you paste from PasteSpace is plain text. |
| Always copy as plain text | Off | Formatted text is recorded as plain text. |
| Join multiple items with | New line | The separator placed between items copied together (`\n` new line, `\t` tab, or any text). |
| History limit | 10 (free) | How many items to keep. Pro: any number, or ∞. |
| Keep history for | Forever | Removes unpinned items older than 1, 7 or 30 days. |
| Pinned limit | 3 (free) | How many items can be pinned. Pro: any number, or ∞. |
| Ephemeral Mode *(Pro)* | Off | Erases your history when PasteSpace quits. With *Keep Pinned items* (on). |
| App Blocklist | Empty | Apps whose copies are never recorded. |
| Vault | On | Encrypted storage for sensitive items. Off: nothing new is locked, and the 🔒 buttons dim. Items already locked stay locked. |
| ↳ Auto-detect sensitive content | On | Locks recognised secrets automatically. |
| ↳ Capture from password managers | On | Records password-manager copies straight into the Vault instead of ignoring them. |
| Text recognition in images (OCR) | On | Reads the text in images you copy. |
| Text extraction from documents *(Pro)* | On | Reads the text of documents you copy. |
| Quick Look · Data Magic · QR Code · Share | On | One switch each. A feature you turn off disappears from every item — its button is removed from the rows ([more](#buttons)). |

At the end of Settings, **Rate PasteSpace on the App Store** opens PasteSpace's review page — see [Rating PasteSpace](#rating).

---

<a id="shortcuts"></a>
## Keyboard shortcuts

| Keys | Action |
|---|---|
| **⌥⇧V** | Open or close PasteSpace (change it in Settings) |
| **↑ ↓** | Move through the list |
| **Return** | Copy the focused item — or the whole selection |
| **⌥Return** | Copy as plain text |
| **⌘Return** | Add the focused item to the selection, or remove it |
| **⌘-click** | Add an item to the selection, or remove it |
| **⇧-click** | Select a range |
| **Esc** | Clear the selection — or close PasteSpace if nothing is selected |
| **⌘V** | Paste, in your app |

**In Quick Look**

| Keys | Action |
|---|---|
| **⌘F** | Find in the text |
| **Return** · **⌘G** | Next match |
| **⇧Return** · **⇧⌘G** | Previous match |
| **Esc** | Close the find bar |
| **⌘Z** | Undo, in the editor |
| **⇧⌘Z** | Redo, in the editor |

---

<a id="faq"></a>
## Questions people ask

**Why do I have to press ⌘V myself?**
Pasting for you would require the macOS Accessibility permission, which lets an app observe and control everything on your Mac. PasteSpace is built never to need it: choosing an item puts it on the clipboard and brings back the app you were in, so all that's left is ⌘V — and the paste stays yours.

**I copied a password and it wasn't locked.**
It probably didn't meet the password rule — one word of 8–64 characters with an uppercase letter, a lowercase letter, a digit and a symbol. Lock it with 🔒. In the free version, also check whether your Vault already holds 2 items. (A password copied from a password manager is never stored unlocked — when the Vault is full, it isn't recorded at all.)

**Why doesn't my password show up when I search for it?**
Because it's locked. A search that could find locked items would let anyone confirm your secrets by guessing. Use the *Protected* or *Passwords* filter to find locked items. [More](#vault-search).

**Why does a locked item ask for Touch ID every time I copy it, but another one doesn't?**
The one that doesn't is currently revealed — you already authenticated. It locks again when you close PasteSpace. [More](#vault).

**I locked a file. Is the file encrypted now?**
No. PasteSpace protects its record of the file — name and location, behind Touch ID — but the file on your disk is unchanged. [More](#vault).

**Why did a locked document arrive empty in WhatsApp?**
Some web-based apps read a dropped file before you've had time to authenticate. Reveal the item first, then drag it. [More](#vault).

**A button is missing from my items.**
Check Settings: Quick Look, Data Magic, QR Code and Share each have a switch, and turning one off removes its button from every item. Data Magic and QR codes also appear only on text. [More](#buttons).

**Something I copied wasn't saved.**
It may have come from a blocked app or a password manager, been marked private by the app you copied from, been more than 10 MB of text (images and files of any size are always recorded), or arrived from another device through Universal Clipboard. [More](#history).

**Will updating PasteSpace delete my history?**
No. Your history, pinned items and Vault are kept across updates.

**Does PasteSpace upload anything?**
No. The only connection is Apple's App Store framework, for purchases and the occasional rating request. [More](#privacy).

**What happens to my history if I stop using Ephemeral Mode?**
Nothing — it simply stops being erased when PasteSpace quits.

---

<a id="requirements"></a>
## System requirements

- **macOS 14 Sonoma** or later, including macOS 27 beta.
- Any Mac — Apple silicon or Intel.
- Touch ID recommended for the Vault; your Mac's login password works on every Mac.

### Under the hood

| Component | Technology |
|---|---|
| Encryption | AES-256-GCM via Apple CryptoKit |
| Key storage | macOS Keychain (this device only, available when unlocked), with a backup in the sandboxed app folder |
| Vault fingerprints | HMAC-SHA256 under a key derived from the Vault key |
| Authentication | Touch ID or device password via LocalAuthentication |
| Text recognition | Apple Vision, in a separate sandboxed helper with no network or file access, which quits when idle |
| Document reading | Apple PDFKit and AppKit's document readers; web pages by PasteSpace's own reader, which never loads anything a page links to |
| Database | SQLite via GRDB.swift, with a full-text search index |
| In-app purchase | StoreKit 2 with on-device verification |
| Interface | SwiftUI and AppKit, native macOS |
| Paste | Clipboard only — no simulated keystrokes, no Accessibility permission |
| Export compliance | `ITSAppUsesNonExemptEncryption = false` (local data protection only) |

---

<a id="whats-new"></a>
## What's new in PasteSpace 3.0

### A new design

- **More room for what you copied.** Each item's text now spans the full width of the window. Its buttons sit in a slim bar underneath — faint until you point at the item — with the source app and the exact date and time of the copy on the right. A cleaner header, item counts on both sections, a discreet *✓ Copied* confirmation, and formatted text that stays readable in both Light and Dark mode.
- **Open at mouse cursor** — the window opens right under your pointer, with the pointer already resting on your newest item.
- **Always on top** — the window stays open above your other apps while you work, and copying an item no longer closes it.
- **A switch for every feature.** Quick Look, Data Magic, QR codes, Share and reading text from documents can each be turned off in Settings — and a feature you turn off takes its button off every item, so your history shows only what you use. Also new in Settings: *Always copy as plain text*, and *Keep history for* 1, 7 or 30 days, or forever.
- **Fold away Pinned** — one click on the *PINNED* header collapses the section, so your recent copies start right at the top.
- **Arrange your history** by dragging items; the list scrolls by itself when you hold an item near its edge.
- **Work with many items at once** — ⌘-click or ⌘Return to build a selection, ⇧-click for a range, then copy, pin, protect, reveal in Finder, delete or drag them all together.
- **Faster and lighter** — PasteSpace opens instantly and scrolls smoothly even with large images and long web pages in your history, and text recognition gives back its memory as soon as it's done.

### Finding things

- **Filters and sorting** — narrow your history by 15 kinds of content (links, code, passwords, images, PDFs and other documents, archives, folders…), and in Pro by date, state and source app. Nine sort orders, including *Most used* and *Recently used*. Every active filter is shown as a removable chip, so nothing ever silently hides part of your history.
- **Search inside documents** *(Pro)* — the PDFs, Word, RTF and OpenDocument files, web pages, and text and code files you copy are read, so searching for a word finds the file that contains it. Scanned PDFs are recognised page by page, and no document is too large to be read.
- **Find in Quick Look** — press **⌘F** (or the 🔍 in the title bar) to search the text you're reading or editing, including the text of images and documents. Accents don't matter: *sarbatoare* finds *sărbătoare*.
- **Item details** — an ⓘ next to each item shows what the row can't: the code language, the full link, a file's size and location, image dimensions, when it will be removed — and every time the item was copied.

### Text in images and documents

- **Text recognition in 30 languages**, detected automatically: English (US), French, Italian, German, Spanish, Portuguese (Brazil), Chinese (Simplified and Traditional), Cantonese (Simplified and Traditional), Korean, Japanese, Russian, Ukrainian, Thai, Vietnamese, Arabic, Najdi Arabic, Turkish, Indonesian, Czech, Danish, Dutch, Norwegian, Norwegian Bokmål, Norwegian Nynorsk, Malay, Polish, Romanian and Swedish. *(All 30 on macOS 26; earlier versions of macOS recognise fewer.)*
- **Edit the text PasteSpace reads** — the text recognised in an image or extracted from a document can now be edited: correct it, and save it as a new item linked to the original. Images and documents open in Quick Look with *Preview* and *Extracted text* tabs.
- **No size limits** — images and files of any size are recorded and read, and scanned PDFs are recognised in full, every page.
- **Web pages keep their look** — fonts, colours and highlights come from the page's own style sheets, and nothing the page links to is ever downloaded.
- **Text files in any encoding** — older national encodings such as Windows-1250, Windows-1251, Shift-JIS or Big5 are recognised automatically.

### Quick Look and editing

- **Undo and redo** in the text editor — toolbar buttons, or **⌘Z** and **⇧⌘Z**, for typing and formatting alike.
- **Edits never overwrite** — saving creates a new version; *Original ⇄ Edited* lets you switch between them.
- **Copy formatted / Copy as plain text** — wherever text is shown with formatting, for all of it or just the part you've selected.

### Vault

- **A stronger Vault** — locked items now hide completely from search; their formatting and any text read out of them are encrypted along with the content; previews reveal far less (a password shows only dots); copying a locked secret again no longer creates a readable copy; and a copy from a password manager is never stored unlocked. More kinds of secrets are recognised, with fewer false alarms. [How it works →](#vault)

### Data Magic

- **57 actions, 20 of them new** — code clean-up, *JSON → Swift struct* and *→ TypeScript interface*, *Remove Tracking from Link*, extracting the links, email addresses and phone numbers from a text, *Calculate Result*, *Add Up Numbers* and more. Data Magic now offers only the actions that fit what you copied, recognises code in about 30 programming languages, and its preview and 👁 button now work as they should.

### Drag and drop

- **Fixed throughout, and tested with every kind of item** — text, links, images, single files, groups of files, Vault items and multiple selections — into Finder, Apple's apps and third-party apps alike, including web-based ones such as Slack and WhatsApp. Files arrive as real files under their own names, a selection arrives whole, and several locked items need just one Touch ID.

### Also new

- **Share** any item through Messages, Mail, AirDrop, Notes and other services.
- **Ephemeral Mode asks before quitting** — it shows what will be erased and what will be kept, and asks too when your Mac is about to log out, restart or shut down.
- **Rate PasteSpace from inside the app** — from a card at the end of Settings, plus an occasional reminder at a quiet moment, which stops for good once you've used that card. [Why it matters →](#rating)
- **Buy Pro straight from PasteSpace's App Store page**, as well as inside the app.
- **A new app icon**, redrawn for current macOS.

---

## Legal

- [Terms of Use](https://mariusconstantin93.github.io/PasteSpace-Clipboard-Manager/terms) · [Privacy Policy](https://mariusconstantin93.github.io/PasteSpace-Clipboard-Manager/privacy)
- **© 2026 Marius Constantin Popescu. All rights reserved.**

<a id="contact"></a>
## Contact

Questions, feedback or feature requests?

📧 **mariuscpopescu@icloud.com** — I read every email.
