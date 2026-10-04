---
layout: default
title: "PasteSpace vs Paste, Raycast, Maccy and Pastebot — Mac clipboard managers compared"
description: "How PasteSpace compares with Paste, Raycast, Maccy and Pastebot: price, privacy, password protection, search inside screenshots and documents, editing, transformations — and when another app may suit you better."
permalink: /compare/
---

# PasteSpace compared with other Mac clipboard managers

There are several good clipboard managers for the Mac, and the right one depends on what you need. This page compares **PasteSpace** with four popular alternatives — **Paste**, **Raycast**'s built-in clipboard history, **Maccy** and **Pastebot** — using only what each developer states on its own website, documentation or App Store page.

**A note on who's writing:** I'm the developer of PasteSpace, so this page isn't neutral. That's why every claim about another app comes from that app's own website, documentation or App Store page, linked at the bottom — and why the page also says when another app may suit you better.

*Checked on October 4, 2026, and re-checked with every PasteSpace release. Prices are in US dollars, vary by country and change over time. If something here is out of date, [write to me](mailto:mariuscpopescu@icloud.com) and I'll correct it.*

*"Not mentioned" means I found no mention of it on the developer's own website, documentation or App Store page. It doesn't prove the feature is missing — check with the developer if it matters to you.*

## Price and platforms

| | PasteSpace | Paste | Raycast | Maccy | Pastebot 3 |
|---|---|---|---|---|---|
| **Price** | Free; Pro is **$19.99 once** | Subscription, $29.99 a year; a lifetime plan is also offered | Free (history kept up to 3 months); Pro $96 a year for unlimited history | Free and open source; $9.99 on the Mac App Store | $39 with a year of updates, or $24.99 a year on the App Store |
| **Where your history is kept** | **Only on your Mac** — no sync, no cloud | Your devices and your private iCloud | Your Mac; cloud sync with Pro | Only on your Mac | Your Macs, with optional iCloud sync |
| **iPhone and iPad** | No | Yes | Not mentioned | No | Not mentioned |

## Privacy and security

| | PasteSpace | Paste | Raycast | Maccy | Pastebot 3 |
|---|---|---|---|---|---|
| **Recognises secrets in ordinary copies** | **Yes** — card numbers (checksum-verified), IBANs, API keys and tokens, passwords, personal ID numbers | Not mentioned | Not mentioned | Not mentioned | Not mentioned |
| **Keeps secrets encrypted one by one, behind Touch ID** | **Yes** — masked on screen and hidden from search | Not mentioned | The whole history is encrypted on disk | Not mentioned | Not mentioned |
| **Copies from password managers** | Go **straight into the encrypted Vault** — or are ignored, your choice | Rules to ignore passwords and sensitive apps | Ignored by default | Ignored, following the password manager | Blocklist for sensitive apps |
| **Erases the history every time the app quits** | **Yes** — Ephemeral Mode (Pro); the Vault is kept | Not mentioned; history kept from 1 day to forever | Not mentioned; history kept from 1 day to 3 months, longer with Pro | Not mentioned | Not mentioned |
| **How pasting works** | Puts the item on the clipboard and you press ⌘V — **no Accessibility permission needed** | Can paste into the app you're using, with the Accessibility permission | Pastes into the app you're using | Optional automatic paste, with the Accessibility permission | Pastes into the app you're using |

## Finding things

| | PasteSpace | Paste | Raycast | Maccy | Pastebot 3 |
|---|---|---|---|---|---|
| **Find a screenshot by the text in it** | Yes — up to 30 languages, detected automatically | Yes — matches highlighted in the results | Yes — Fast or Accurate mode | Not mentioned | Not mentioned |
| **Search inside copied PDFs and Word files** | **Yes** (Pro) — scanned PDFs, RTF, OpenDocument and web pages too | Not mentioned | Not mentioned | Not mentioned | Not mentioned |
| **Filter by kind of content** | **16 kinds** — including passwords, cards and IBANs, keys, code, documents, archives and folders — combined with date, state and source app in Pro | By content type, source app, date and device | 6 types: text, images, files, links, emails, colours | Not mentioned | Not mentioned |
| **Sort the history** | **9 orders**, including most used and recently used — or your own, by dragging | Not mentioned | Not mentioned | Not mentioned | Not mentioned |
| **Copy history of each item** | **Yes** — how many times it was copied, when, and in which app | Not mentioned | Not mentioned | Not mentioned | Not mentioned |
| **Recognises code** | **About 30 programming languages**, plus JSON, HTML, XML and YAML | Not mentioned | Not mentioned | Not mentioned | Not mentioned |

## Working with what you copied

| | PasteSpace | Paste | Raycast | Maccy | Pastebot 3 |
|---|---|---|---|---|---|
| **Edit an item** | **Full rich-text editor** — fonts, sizes, colours, highlights, lists, alignment, undo and redo, find | Edit text, with Apple Intelligence Writing Tools | Quick edits to text, links and colours | Not mentioned | Not mentioned |
| **The original, after an edit** | **Kept** — each save is a new version, and you can switch between Original and Edited | Updated in place | Not mentioned | Not mentioned | Not mentioned |
| **Edit the text read from an image or document** | **Yes** — correct it and save it as a version linked to the image or document | Extract text from an image in the preview | Copy the text from an image | Not mentioned | Not mentioned |
| **Transform what you copied** | **Data Magic** — 57 actions offered according to the content: format JSON, JSON → Swift or TypeScript, convert colours, remove link tracking, clean up code… | Paste as plain text | Paste in another format — plain text, RTF, HTML… | Paste with or without formatting | Filters you build by stacking base filters |
| **QR codes** | **Turns any text into a QR code** | Not mentioned | Reads QR codes in copied images | Not mentioned | Not mentioned |

## Where PasteSpace is different

- **It locks your secrets away by itself.** Passwords, card numbers, IBANs, API keys and other secrets are recognised the moment you copy them — card numbers must pass the checksum every real card number passes, so random numbers aren't mistaken for cards — and encrypted one by one with AES-256 in the Vault. They're shown masked, unlocked only with Touch ID or your Mac's password, and invisible to search. The other apps compared here describe protecting passwords mainly by *not recording them*; PasteSpace keeps them — safely. [How the Vault works](https://mariusconstantin93.github.io/PasteSpace-Clipboard-Manager/#vault)
- **It reads inside your documents.** None of the other apps compared here mention it: PasteSpace reads the text of the documents you copy in Finder — PDFs, scanned PDFs, Word, RTF, OpenDocument, web pages, text files — so a search finds the file that contains the words. [Text inside documents](https://mariusconstantin93.github.io/PasteSpace-Clipboard-Manager/#documents)
- **Edits never overwrite.** PasteSpace's Quick Look editor is a full rich-text editor, and saving always creates a new version: the original stays exactly as you copied it, one click away. That includes the text read out of a screenshot or a scanned document — correct what was misread, and the corrected text stays linked to the image. [Quick Look and the editor](https://mariusconstantin93.github.io/PasteSpace-Clipboard-Manager/#quick-look)
- **It understands what you copied.** It recognises code in about 30 programming languages, sorts your history into 16 kinds of content — passwords and cards included — and Data Magic offers only the transformations that make sense for each item: a colour gets colour conversions, a JSON response gets formatting and a Swift struct, a link with tracking gets it removed. Every item also keeps its own copy history. [Data Magic](https://mariusconstantin93.github.io/PasteSpace-Clipboard-Manager/#data-magic)
- **Nothing ever leaves your Mac.** There is no sync, no account and no cloud — not even an optional one. The only connections PasteSpace makes are through Apple's App Store framework, for purchases and the occasional rating request. With Ephemeral Mode, the history itself is erased every time PasteSpace quits. [Privacy](https://mariusconstantin93.github.io/PasteSpace-Clipboard-Manager/#privacy)
- **It never asks to control your Mac.** Paste and Maccy can paste into the app you're using for you, which requires the macOS Accessibility permission — the one that lets an app watch and control everything you do. PasteSpace doesn't ask for it: it puts your item on the clipboard and brings back your app, and you press ⌘V.
- **One payment.** PasteSpace is free to use, and Pro is a single $19.99 payment, for life.

## When another app may suit you better

- **You want your clipboard on your iPhone and iPad too** → **Paste** syncs your history across your devices through your private iCloud. PasteSpace keeps everything on one Mac by design.
- **You want to share clips with your team** → **Paste** offers shared pinboards and a plan for teams.
- **You want AI assistants to work with your clipboard** → **Paste** connects to Claude, Cursor, Codex and other AI tools, and suggests items with Apple Intelligence; **Raycast** can send an entry to its AI chat. PasteSpace deliberately connects to nothing but the App Store.
- **You already use Raycast as your launcher** → its built-in clipboard history may be all you need.
- **You want something free, minimal and open source** → **Maccy**.
- **You want the app to paste for you**, without pressing ⌘V → **Paste** or **Maccy**, once you've granted them the Accessibility permission.
- **You want paste stacks and filters you build yourself** → **Pastebot** pastes a series of items one after another and lets you combine its base filters into your own.

## Sources

- Paste: [pasteapp.io](https://pasteapp.io/), [pricing](https://pasteapp.io/pricing), [help centre](https://pasteapp.io/help), [Paste on Mac](https://pasteapp.io/help/paste-on-mac), [search and filters](https://pasteapp.io/help/search-and-filters), [editing items](https://pasteapp.io/help/edit-items-before-pasting), [history retention](https://pasteapp.io/help/control-history-retention), [Intelligent Clipboard](https://pasteapp.io/help/intelligent-clipboard), [App Store](https://apps.apple.com/us/app/paste-limitless-clipboard/id967805235)
- Raycast: [Clipboard History](https://www.raycast.com/core-features/clipboard-history), [manual](https://manual.raycast.com/clipboard-history), [pricing](https://www.raycast.com/pricing)
- Maccy: [maccy.app](https://maccy.app/), [GitHub](https://github.com/p0deje/Maccy), [App Store](https://apps.apple.com/us/app/maccy/id1527619437)
- Pastebot: [tapbots.com/pastebot](https://tapbots.com/pastebot/)
- PasteSpace: [website](https://mariusconstantin93.github.io/PasteSpace-Clipboard-Manager/), [Mac App Store](https://apps.apple.com/app/id6762815491)

---

[← Back to PasteSpace](https://mariusconstantin93.github.io/PasteSpace-Clipboard-Manager/)
