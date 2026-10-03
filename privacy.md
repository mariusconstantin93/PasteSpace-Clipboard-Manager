# Privacy Policy

**Last Updated: October 3, 2026**

PasteSpace — Clipboard Manager ("PasteSpace", "the App") is developed by Marius Constantin Popescu. This Privacy Policy explains how the App handles your data.

### 1. Our Core Principle: Your Data Stays on Your Device
PasteSpace is designed with a local-first architecture. All clipboard history, Vault items, settings, text recognised in images, text extracted from documents, and related data are stored exclusively on your Mac. We do not operate any servers, cloud services, analytics platforms, or remote databases.

No data ever leaves your device through PasteSpace. The only network communication is handled by Apple's App Store framework, as described in Section 11.

### 2. Data We Collect
We do not collect any personal data. Specifically:

- No analytics or telemetry — we do not track how you use the App.
- No crash reports are sent to us — macOS handles crash reporting through Apple's own systems, subject to your macOS privacy settings.
- No advertising or ad networks.
- No third-party SDKs that collect data.
- No account creation required — the App has no user accounts or login.

Because PasteSpace collects zero personal data, it is inherently compliant with major data privacy regulations worldwide, including the European Union's General Data Protection Regulation (GDPR), the California Consumer Privacy Act (CCPA), and similar frameworks. There is no personal data to collect, process, share, or delete — your privacy is protected by design.

### 3. Data Stored Locally on Your Device
PasteSpace stores the following data locally within its macOS App Sandbox container:

- Clipboard History: text (with its formatting), links, images, and references to files copied to your system clipboard, together with the name of the app each item was copied from and the date and time. Stored in a local SQLite database.
- Copy History and Usage: a record of each time an item is copied — when, and whether in another app or from PasteSpace — and how often you use each item from PasteSpace. It powers the item details and the "Most used" and "Recently used" sort orders, and is deleted together with the item.
- Vault Items: clipboard content encrypted using AES-256-GCM, together with its formatting and any text read from it. The ciphertext, nonce, and authentication tag are stored in the same local database, alongside a masked preview and a keyed fingerprint (see Section 6).
- Recognised and Extracted Text: text recognised in copied images (Section 8) and, in the Pro tier, text extracted from copied documents (Section 9), stored alongside the corresponding item so that it can be searched.
- Edited Versions: texts you edit and save in Quick Look, stored as new items linked to the original.
- Settings & Preferences: your configuration choices (toggle states, blocklist, hotkey) and the counters used to decide when to show the App Store rating request (Section 11), stored in UserDefaults within the App Sandbox.
- Encryption Key: stored in your macOS login Keychain on this Mac, with a file backup in the sandboxed Application Support directory. The key never leaves your device.
- Purchase Status: StoreKit transaction data managed by Apple's frameworks, verified on-device via JWS (JSON Web Signature). PasteSpace sends no purchase data to any server.

### 4. Clipboard Monitoring
PasteSpace monitors your macOS system clipboard (NSPasteboard) at regular intervals to detect new copied content. This is the App's core functionality.

- Monitoring runs only while PasteSpace is running; quitting the App stops it.
- You can exclude specific apps with the App Blocklist in Settings — 1 app in the Free tier, any number in Pro. Nothing copied in a blocked app is recorded.
- Content that an app marks as private ("concealed" or "transient", as is common for passwords and one-time codes) is not recorded, nor is content arriving from another device through Universal Clipboard.
- Copies from known password managers are recorded only into the Vault, encrypted, while "Capture from password managers" is on — the default, in both tiers. A copy that cannot be locked (for example because the free Vault is full or the Vault is turned off) is not recorded at all. With the option off, password managers are ignored entirely.
- PasteSpace never simulates keystrokes or pastes into other apps on your behalf.

### 5. Sensitive Data Detection
When the Vault and its automatic detection are enabled (both are on by default, in both tiers), PasteSpace checks each copied text locally against patterns for potentially sensitive content, including:

- Credit/debit card numbers (validated with the Luhn checksum)
- IBANs (validated with their check digits)
- Personal identification numbers (US Social Security numbers, Romanian CNPs)
- API keys and tokens (GitHub, GitLab, Slack, OpenAI, Google, AWS, Stripe, JWT, etc.)
- SSH and PEM private keys, SSH fingerprints
- Database connection strings and secret environment variables
- Software license keys
- Passwords, username and password pairs, and cryptocurrency seed phrases
- One-time codes copied from authenticator apps
- High-entropy strings that may be secrets

Detected content is encrypted in the Vault automatically. The same local checks also label items by kind (for example "Passwords") so that you can filter your history; the label is stored only on your Mac. All detection is performed locally. No data is sent anywhere for analysis.

### 6. Encryption & Security
The Vault uses industry-standard encryption:

- Algorithm: AES-256-GCM (Authenticated Encryption with Associated Data)
- Implementation: Apple's CryptoKit framework (not a custom or third-party implementation)
- What is encrypted: the item's content, its formatted copies, and any text recognised in it or extracted from it
- Key Storage: a single 256-bit key, created on your Mac and stored in your macOS login Keychain. It is never synced to iCloud or transferred to another device.
- File Backup: a synchronized copy of the key is kept in the sandboxed Application Support directory with POSIX 0600 permissions (readable only by your user account) as a safety net
- Search: locked items are removed from the search index, so their contents cannot be found, or confirmed, by searching
- Previews and Fingerprints: a locked item shows only a masked preview, and its duplicate-detection fingerprint is computed with a key derived from the Vault key (HMAC-SHA256), so it reveals nothing without that key

Locking a file item protects PasteSpace's record of the file — its name and location. The file itself, on your disk, is not encrypted.

PasteSpace uses encryption only to protect data stored on your device (ITSAppUsesNonExemptEncryption = false).

### 7. Biometric Data (Touch ID)
PasteSpace uses Apple's LocalAuthentication framework to authenticate users via Touch ID — or, on a Mac without Touch ID, the device password — when accessing Vault items.

- PasteSpace never accesses your fingerprint or biometric data directly.
- All biometric processing is handled by macOS and the Secure Enclave.
- The App only receives a success or failure result from the system.
- No biometric data is stored, transmitted, or logged by PasteSpace.

### 8. Text Recognition in Images (OCR)
Text recognition uses Apple's Vision framework to read the text in copied images.

- All processing happens locally on your Mac.
- Recognition runs in a separate helper process within the App. The helper is sandboxed, with no network access and no access to your files of its own: it receives only the image being read, and quits when it has nothing to do.
- No images are uploaded to any server.
- Recognised text is stored in the local database alongside the original image and is searchable within the App, unless the image is locked in the Vault.
- You can turn text recognition off in Settings.

### 9. Text Extraction from Documents
In the Pro tier, PasteSpace reads the text of documents you copy — PDFs, Word, RTF, and OpenDocument files, web pages and web archives, and text and code files — so that you can find them by their contents. Scanned documents are read with text recognition, as described in Section 8.

- All reading happens locally on your Mac, using Apple's PDFKit and AppKit document readers. Web pages are read by PasteSpace's own reader, which never downloads anything a page refers to — images, style sheets, scripts, or links.
- The extracted text is stored alongside the file reference in the local database. Locked documents are not read, and text read before locking is encrypted with the item.
- You can turn text extraction off in Settings. Text already extracted stays until the item is deleted.

### 10. In-App Purchases
PasteSpace uses Apple's StoreKit 2 framework for the Pro upgrade, whether you buy it inside the App or from PasteSpace's page on the Mac App Store:

- Transaction verification is performed on-device using JWS (JSON Web Signature).
- PasteSpace sends no purchase data to any external server.
- Purchase history is stored locally by Apple's StoreKit framework.
- We do not have access to your Apple ID, payment method, or billing information.

### 11. Third-Party Services
PasteSpace does not integrate with any third-party services, analytics platforms, crash reporting tools, advertising networks, or cloud storage providers.

The only external communication is between Apple's StoreKit framework and Apple's App Store servers, for purchase verification and for the App Store rating request. Both are handled entirely by Apple's frameworks and are subject to Apple's Privacy Policy.

PasteSpace decides when to show the rating request using counts kept on this Mac alone: how many times you pasted, on how many days you opened it, and which features you used. It sends none of that anywhere, and it is never told whether you left a review. The "Rate PasteSpace on the App Store" button in Settings simply opens PasteSpace's page in the App Store app.

When you share an item, it is handed to the macOS sharing service you choose (for example Mail, Messages, or AirDrop), which sends it under its own terms; PasteSpace itself makes no network connection. Links in your history are shown with a title derived from the address itself — PasteSpace never visits the page — and open in your default browser only when you choose to open them.

### 12. Data Retention & Deletion
- Clipboard history can be cleared at any time with the Clear History button; pinned and Vault items are kept. Individual items, or a selection of items, can be deleted at any time.
- Pinned items can be removed with "Clear Pinned", and Vault items with "Clear Vault" (after authentication), in Settings.
- When the history limit is reached, the oldest unpinned items are removed automatically, and — if you set "Keep history for" to 1, 7, or 30 days — so are items older than that. Pinned and Vault items are never removed automatically.
- Ephemeral Mode (Pro) erases your clipboard history whenever PasteSpace quits, including when your Mac logs out, restarts, or shuts down; the erasure is completed the next time PasteSpace starts. Vault items are always kept, and pinned items are kept unless you choose otherwise.
- Deleting an item also deletes its copy history and any text read from it. Deleted items cannot be recovered.
- macOS keeps an app's data after the app itself is deleted. To remove all of PasteSpace's data, quit the App, delete the folders "com.pastespace.clipboard-manager" and "com.pastespace.clipboard-manager.ocr-helper" in ~/Library/Containers, and delete the "com.pastespace.clipboard-manager.vault" item from your login keychain in Keychain Access.

### 13. Children's Privacy
PasteSpace is not directed at children under the age of 13. We do not knowingly collect personal information from children. Since no data is collected from any user, this policy applies equally to all age groups.

### 14. macOS Permissions
PasteSpace uses the following macOS capabilities to function:

- Clipboard Access (NSPasteboard): to monitor and record clipboard content.
- Touch ID / Device Password (LocalAuthentication): to authenticate access to Vault items.
- App Sandbox: the App and its text-recognition helper run within Apple's App Sandbox, which restricts access to the file system and other apps' data.
- File Access (security-scoped bookmarks): to access files you copy in Finder — for preview, document reading, and dragging them back out.
- Network (outgoing connections): used only by Apple's StoreKit framework, for purchases and the rating request.

PasteSpace does not request the Accessibility permission, does not monitor your keystrokes (it receives only its own global shortcut), and never simulates keystrokes.

### 15. Changes to This Policy
We may update this Privacy Policy from time to time. Changes will be reflected in the "Last Updated" date at the top of this document. Continued use of the App after changes constitutes your acceptance of the updated policy.

### 16. Contact
If you have questions or concerns about this Privacy Policy, you can contact us at:
mariuscpopescu@icloud.com
