# PasteSpace Business — Terms of Use

**Last Updated: October 12, 2026**

### 1. Acceptance of Terms
By downloading, installing, or using PasteSpace Business — Clipboard Manager ("PasteSpace Business", "the App"), you agree to be bound by these Terms of Use. When an organization obtains the App for the people who use it, these terms apply both to the organization and to each of those people. If you do not agree to these terms, do not install or use the App.

### 2. Description of Service
PasteSpace Business is a macOS clipboard manager that runs in your menu bar. It monitors your system clipboard and maintains a searchable history of copied items, including text, links, images, and files, and the text inside copied documents. All data is processed and stored locally on your device.

PasteSpace Business is the edition of PasteSpace made for organizations. It includes every feature of PasteSpace for a one-time price, and it has no in-app purchases.

PasteSpace Business requires a Mac running macOS 14 Sonoma or later. Touch ID is optional: on a Mac without it, Vault items are protected by your Mac's login password. The languages available for text recognition depend on your version of macOS.

### 3. Licenses
PasteSpace Business is a paid app on the Mac App Store. Organizations can also buy licenses in volume through Apple Business Manager and Apple School Manager and assign them to people or Macs, for example through their device management system.

- Every purchase is made from Apple. Prices, payment, invoicing, and refunds are handled by Apple under its terms — those of the App Store, or of Apple Business Manager and Apple School Manager. To request a refund for a purchase you made yourself, visit reportaproblem.apple.com.
- Every license includes every feature. There are no in-app purchases, subscriptions, or recurring charges.

### 4. Vault & Encryption
The Vault provides local encryption for sensitive clipboard content using AES-256-GCM via Apple's CryptoKit framework, with no limit on the number of protected items. The encryption key is created on your Mac and stored in your macOS login Keychain, with a backup copy in the App's sandboxed container.

- PasteSpace Business does not have access to your encryption key outside of your device.
- If you lose access to your Mac, or the encryption key is lost (both the Keychain entry and its backup copy), encrypted Vault data cannot be recovered. PasteSpace Business and its developer are not responsible for data loss resulting from Keychain resets, device loss, or operating system reinstallation.
- Revealing, copying, or otherwise using protected content requires Touch ID or your Mac's password.
- Locking a file item protects PasteSpace Business's record of the file — its name and location. The file itself, on your disk, is not encrypted.

### 5. Biometric Authentication
PasteSpace Business uses Apple's LocalAuthentication framework to provide Touch ID or device password authentication for Vault features. Biometric data is handled entirely by macOS — PasteSpace Business never accesses, stores, or transmits your fingerprint or biometric information.

### 6. Text Recognition (OCR)
Text recognition uses Apple's Vision framework to read the text in every copied image. All text recognition is performed locally on your device, in a sandboxed helper process within the App. No images or recognised text are transmitted to any server. Recognised text may contain errors.

### 7. Text Extraction from Documents
Text extraction reads the text of documents you copy — such as PDFs, Word and Excel files, RTF and OpenDocument files, web pages, and text files — so that you can search your history by their contents. Scanned documents are read with text recognition, as described in Section 6. All reading is performed locally on your device. Only part of a very large document may be read, and extracted text may be incomplete or contain errors.

### 8. Data Magic
Data Magic detects the type of copied text (JSON, code, links, tables, color codes, dates, etc.) and offers one-click transformations for every text item. All processing occurs locally on your device.

### 9. Sensitive Data Detection
When the Vault and its automatic detection are enabled (both are on by default), PasteSpace Business may automatically detect and encrypt potentially sensitive content such as credit card numbers, IBANs, personal identification numbers, passwords, API keys, SSH keys, software license keys, tokens, and other credentials. This detection uses local pattern matching and is provided as a convenience — it is not guaranteed to identify all sensitive data.

You are solely responsible for the security of your clipboard content. PasteSpace Business is not liable for any sensitive data that is not automatically detected or for any data breach resulting from circumstances beyond the App's control.

### 10. Ephemeral Mode
Ephemeral Mode erases your clipboard history whenever PasteSpace Business quits, including when your Mac logs out, restarts, or shuts down. When you quit PasteSpace Business yourself, it asks you to confirm first; when your Mac logs out, restarts, or shuts down, the erasure proceeds without asking, because macOS does not let menu-bar apps pause or cancel it. Vault items are always kept, and pinned items are kept unless you choose otherwise. Erased items cannot be recovered.

### 11. App Blocklist
The App Blocklist allows you to prevent PasteSpace Business from recording clipboard content from any number of specific applications. Copies from known password managers are recorded only into the Vault, encrypted, while "Capture from password managers" is on (the default), and are ignored entirely when it is off.

### 12. Data Storage & Ownership
All clipboard history, Vault items, settings, and related data are stored exclusively on your Mac in the App's sandboxed container. PasteSpace Business does not operate any servers, cloud services, or remote databases, and it sends nothing to your organization either.

The data belongs to you or to your organization, as your organization's own policies determine. The developer does not access, collect, or have the ability to retrieve it. When you share an item through a macOS sharing service (for example Mail, Messages, or AirDrop), the content is handled by that service under its own terms.

### 13. Intellectual Property
PasteSpace Business, including its design, code, and documentation, is the intellectual property of Marius Constantin Popescu. You are granted a limited, non-exclusive, non-transferable license to use the App in accordance with these terms and the Apple Licensed Application End User License Agreement (EULA).

You may not reverse engineer, decompile, disassemble, or attempt to derive the source code of the App. You may not reproduce, distribute, sublicense, sell, or rent the App or any of its features to third parties.

### 14. Disclaimer of Warranties
PasteSpace Business is provided "as is" and "as available" without warranties of any kind, either express or implied. The developer does not warrant that the App will be uninterrupted, error-free, or free of harmful components.

The automatic detection of sensitive data is provided on a best-effort basis and should not be relied upon as the sole method of protecting sensitive information.

### 15. Limitation of Liability
To the maximum extent permitted by applicable law, the developer shall not be liable for any indirect, incidental, special, consequential, or punitive damages, or any loss of data, arising out of or related to your use of PasteSpace Business.

The developer's total liability shall not exceed the amount paid for the license under which the App is used.

### 16. Changes to Terms
We may update these Terms of Use from time to time. Continued use of the App after changes are posted constitutes your acceptance of the revised terms. Material changes will be communicated through the App or on our website.

### 17. Governing Law
These terms are governed by and construed in accordance with the laws of Romania, without regard to conflict of law principles.

### 18. Contact
If you have questions about these Terms of Use, you can contact us at:
mariuscpopescu@icloud.com
