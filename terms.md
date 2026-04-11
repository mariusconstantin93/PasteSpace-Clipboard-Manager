# Terms of Use

**Last Updated: April 8, 2026**

### 1. Acceptance of Terms
By downloading, installing, or using PasteSpace — Clipboard Manager ("PasteSpace", "the App"), you agree to be bound by these Terms of Use. If you do not agree to these terms, do not install or use the App.

### 2. Description of Service
PasteSpace is a macOS clipboard manager that runs in your menu bar. It monitors your system clipboard and maintains a searchable history of copied items, including text, images, and files. All data is processed and stored locally on your device.

PasteSpace requires a compatible Mac running a supported version of macOS. Certain features, such as Vault Mode, rely on Apple hardware capabilities (Secure Enclave, Touch ID) and may not be fully available on all devices.

### 3. Free and Pro Tiers
PasteSpace is available in two tiers:

• Free Tier: Includes clipboard history (limited to 20 items), pinned items (limited to 5), and basic clipboard management features.

• Pro Tier: A one-time, non-consumable in-app purchase that unlocks unlimited history, unlimited pins, Vault Mode (encrypted storage with biometric protection), Quick Look previews, OCR text extraction from images, Data Magic transformations, App Blocklist, and Ephemeral Mode.

The Pro upgrade is a lifetime purchase — there are no subscriptions or recurring charges.

### 4. In-App Purchases
The Pro upgrade is processed through the Apple App Store using StoreKit. All purchases are subject to Apple's terms and conditions. Prices are displayed in your local currency at the time of purchase.

• Payment is charged to your Apple ID account at confirmation of purchase.
• The purchase is non-consumable and can be restored on any Mac signed in with the same Apple ID.
• Refunds are handled exclusively by Apple in accordance with their refund policy. To request a refund, visit reportaproblem.apple.com.

### 5. Vault Mode & Encryption
Vault Mode (Pro feature) provides local encryption for sensitive clipboard content using AES-256-GCM via Apple's CryptoKit framework. The encryption key is stored in your device's Keychain, backed by the Secure Enclave on Apple Silicon Macs.

• PasteSpace does not have access to your encryption key outside of your device.
• If you lose access to your device or reset your Keychain, encrypted Vault data cannot be recovered. PasteSpace and its developer are not responsible for data loss resulting from Keychain resets, device loss, or operating system reinstallation.
• Vault Mode requires biometric authentication (Touch ID) or your device password to reveal protected content.

### 6. Biometric Authentication
PasteSpace uses Apple's LocalAuthentication framework to provide Touch ID or device password authentication for Vault features. Biometric data is handled entirely by macOS — PasteSpace never accesses, stores, or transmits your fingerprint or biometric information.

### 7. OCR (Optical Character Recognition)
The OCR feature (Pro) uses Apple's Vision framework to extract text from copied images. All text recognition is performed locally on your device. No images or extracted text are transmitted to any server.

### 8. Data Magic
Data Magic (Pro feature) detects the type of copied text (JSON, URLs, tables, color codes, dates, etc.) and offers one-tap transformations. All processing occurs locally on your device.

### 9. Sensitive Data Detection
When Vault Mode is enabled, PasteSpace may automatically detect and encrypt potentially sensitive content such as credit card numbers, IBANs, API keys, SSH keys, software license keys, tokens, and other credentials. This detection uses local pattern matching and is provided as a convenience — it is not guaranteed to identify all sensitive data.

You are solely responsible for the security of your clipboard content. PasteSpace is not liable for any sensitive data that is not automatically detected or for any data breach resulting from circumstances beyond the App's control.

### 10. Ephemeral Mode
Ephemeral Mode (Pro feature) automatically deletes your clipboard history when your Mac is restarted or shut down. Vault-protected items are excluded from automatic deletion.

### 11. App Blocklist
The App Blocklist feature (Pro) allows you to prevent PasteSpace from capturing clipboard content from specific applications. In the Free tier, content from known password managers is automatically blocked. In the Pro tier, password manager content can optionally be captured and protected by Vault Mode.

### 12. Data Storage & Ownership
All clipboard history, Vault items, settings, and related data are stored exclusively on your Mac in the App's sandboxed container. PasteSpace does not operate any servers, cloud services, or remote databases.

You retain full ownership of all data stored by PasteSpace. The developer does not access, collect, or have the ability to retrieve your data.

### 13. Intellectual Property
PasteSpace, including its design, code, and documentation, is the intellectual property of Marius Constantin Popescu. You are granted a limited, non-exclusive, non-transferable license to use the App in accordance with these terms and the Apple Licensed Application End User License Agreement (EULA).

You may not reverse engineer, decompile, disassemble, or attempt to derive the source code of the App. You may not reproduce, distribute, sublicense, sell, or rent the App or any of its features to third parties.

### 14. Disclaimer of Warranties
PasteSpace is provided "as is" and "as available" without warranties of any kind, either express or implied. The developer does not warrant that the App will be uninterrupted, error-free, or free of harmful components.

The automatic detection of sensitive data is provided on a best-effort basis and should not be relied upon as the sole method of protecting sensitive information.

### 15. Limitation of Liability
To the maximum extent permitted by applicable law, the developer shall not be liable for any indirect, incidental, special, consequential, or punitive damages, or any loss of data, arising out of or related to your use of PasteSpace.

The developer's total liability shall not exceed the amount you paid for the Pro upgrade.

### 16. Changes to Terms
We may update these Terms of Use from time to time. Continued use of the App after changes are posted constitutes your acceptance of the revised terms. Material changes will be communicated through the App or on our website.

### 17. Governing Law
These terms are governed by and construed in accordance with the laws of Romania, without regard to conflict of law principles.

### 18. Contact
If you have questions about these Terms of Use, you can contact us at: mariuscpopescu@icloud.com
