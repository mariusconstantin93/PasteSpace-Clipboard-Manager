# Terms of Use

**Last Updated: October 3, 2026**

### 1. Acceptance of Terms
By downloading, installing, or using PasteSpace — Clipboard Manager ("PasteSpace", "the App"), you agree to be bound by these Terms of Use. If you do not agree to these terms, do not install or use the App.

### 2. Description of Service
PasteSpace is a macOS clipboard manager that runs in your menu bar. It monitors your system clipboard and maintains a searchable history of copied items, including text, links, images, and files, and — in the Pro tier — the text inside copied documents. All data is processed and stored locally on your device.

PasteSpace requires a Mac running macOS 14 Sonoma or later. Touch ID is optional: on a Mac without it, Vault items are protected by your Mac's login password. The languages available for text recognition depend on your version of macOS.

### 3. Free and Pro Tiers
PasteSpace is available in two tiers:

- Free Tier: a clipboard history of up to 10 items, up to 3 pinned items, a Vault of up to 2 items, and an App Blocklist of 1 app; Quick Look, text recognition, Data Magic, and QR codes for your most recent text and image; search, filtering by kind, sorting, sharing, drag and drop, and multiple selection.
- Pro Tier: a one-time, non-consumable in-app purchase that unlocks unlimited history, pinned items, Vault items, and blocked apps; Quick Look, text recognition, Data Magic, and QR codes for every item; search inside documents; filtering by date, state, and source app; and Ephemeral Mode.

The Pro upgrade is a lifetime purchase — there are no subscriptions or recurring charges.

### 4. In-App Purchases
The Pro upgrade is processed through the Apple App Store using StoreKit, whether you buy it inside the App or from PasteSpace's page on the Mac App Store. All purchases are subject to Apple's terms and conditions. Prices are displayed in your local currency at the time of purchase.

- Payment is charged to your Apple ID account at confirmation of purchase.
- The purchase is non-consumable and can be restored on any Mac signed in with the same Apple ID.
- Refunds are handled exclusively by Apple in accordance with their refund policy. To request a refund, visit reportaproblem.apple.com.

### 5. Vault & Encryption
The Vault provides local encryption for sensitive clipboard content using AES-256-GCM via Apple's CryptoKit framework. It is available in both tiers (up to 2 items in the Free tier). The encryption key is created on your Mac and stored in your macOS login Keychain, with a backup copy in the App's sandboxed container.

- PasteSpace does not have access to your encryption key outside of your device.
- If you lose access to your Mac, or the encryption key is lost (both the Keychain entry and its backup copy), encrypted Vault data cannot be recovered. PasteSpace and its developer are not responsible for data loss resulting from Keychain resets, device loss, or operating system reinstallation.
- Revealing, copying, or otherwise using protected content requires Touch ID or your Mac's password.
- Locking a file item protects PasteSpace's record of the file — its name and location. The file itself, on your disk, is not encrypted.

### 6. Biometric Authentication
PasteSpace uses Apple's LocalAuthentication framework to provide Touch ID or device password authentication for Vault features. Biometric data is handled entirely by macOS — PasteSpace never accesses, stores, or transmits your fingerprint or biometric information.

### 7. Text Recognition (OCR)
Text recognition uses Apple's Vision framework to read the text in copied images — your most recent image in the Free tier, every image in Pro. All text recognition is performed locally on your device, in a sandboxed helper process within the App. No images or recognised text are transmitted to any server. Recognised text may contain errors.

### 8. Text Extraction from Documents
Text extraction (Pro feature) reads the text of documents you copy — such as PDFs, Word, RTF, and OpenDocument files, web pages, and text files — so that you can search your history by their contents. Scanned documents are read with text recognition, as described in Section 7. All reading is performed locally on your device. Only part of a very large document may be read, and extracted text may be incomplete or contain errors.

### 9. Data Magic
Data Magic detects the type of copied text (JSON, code, links, tables, color codes, dates, etc.) and offers one-click transformations — for your most recent text item in the Free tier, for every text item in Pro. All processing occurs locally on your device.

### 10. Sensitive Data Detection
When the Vault and its automatic detection are enabled (both are on by default), PasteSpace may automatically detect and encrypt potentially sensitive content such as credit card numbers, IBANs, personal identification numbers, passwords, API keys, SSH keys, software license keys, tokens, and other credentials. This detection uses local pattern matching and is provided as a convenience — it is not guaranteed to identify all sensitive data.

You are solely responsible for the security of your clipboard content. PasteSpace is not liable for any sensitive data that is not automatically detected or for any data breach resulting from circumstances beyond the App's control.

### 11. Ephemeral Mode
Ephemeral Mode (Pro feature) erases your clipboard history whenever PasteSpace quits, including when your Mac logs out, restarts, or shuts down. PasteSpace asks you to confirm before quitting; when macOS is logging out, restarting, or shutting down and no answer is given within 20 seconds, the erasure proceeds. Vault items are always kept, and pinned items are kept unless you choose otherwise. Erased items cannot be recovered.

### 12. App Blocklist
The App Blocklist allows you to prevent PasteSpace from recording clipboard content from specific applications — 1 application in the Free tier, any number in Pro. Copies from known password managers are recorded only into the Vault, encrypted, while "Capture from password managers" is on (the default), and are ignored entirely when it is off.

### 13. Data Storage & Ownership
All clipboard history, Vault items, settings, and related data are stored exclusively on your Mac in the App's sandboxed container. PasteSpace does not operate any servers, cloud services, or remote databases.

You retain full ownership of all data stored by PasteSpace. The developer does not access, collect, or have the ability to retrieve your data. When you share an item through a macOS sharing service (for example Mail, Messages, or AirDrop), the content is handled by that service under its own terms.

### 14. Intellectual Property
PasteSpace, including its design, code, and documentation, is the intellectual property of Marius Constantin Popescu. You are granted a limited, non-exclusive, non-transferable license to use the App in accordance with these terms and the Apple Licensed Application End User License Agreement (EULA).

You may not reverse engineer, decompile, disassemble, or attempt to derive the source code of the App. You may not reproduce, distribute, sublicense, sell, or rent the App or any of its features to third parties.

### 15. Disclaimer of Warranties
PasteSpace is provided "as is" and "as available" without warranties of any kind, either express or implied. The developer does not warrant that the App will be uninterrupted, error-free, or free of harmful components.

The automatic detection of sensitive data is provided on a best-effort basis and should not be relied upon as the sole method of protecting sensitive information.

### 16. Limitation of Liability
To the maximum extent permitted by applicable law, the developer shall not be liable for any indirect, incidental, special, consequential, or punitive damages, or any loss of data, arising out of or related to your use of PasteSpace.

The developer's total liability shall not exceed the amount you paid for the Pro upgrade.

### 17. Changes to Terms
We may update these Terms of Use from time to time. Continued use of the App after changes are posted constitutes your acceptance of the revised terms. Material changes will be communicated through the App or on our website.

### 18. Governing Law
These terms are governed by and construed in accordance with the laws of Romania, without regard to conflict of law principles.

### 19. Contact
If you have questions about these Terms of Use, you can contact us at:
mariuscpopescu@icloud.com
