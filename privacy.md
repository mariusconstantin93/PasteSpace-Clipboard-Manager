# Privacy Policy

**Last Updated: April 8, 2026**

PasteSpace — Clipboard Manager ("PasteSpace", "the App") is developed by Marius Constantin Popescu. This Privacy Policy explains how the App handles your data.

### 1. Our Core Principle: Your Data Stays on Your Device
PasteSpace is designed with a local-first architecture. All clipboard history, Vault items, settings, OCR results, and related data are stored exclusively on your Mac. We do not operate any servers, cloud services, analytics platforms, or remote databases.

No data ever leaves your device through PasteSpace.

### 2. Data We Collect
We do not collect any personal data. Specifically:

• No analytics or telemetry — we do not track how you use the App.
• No crash reports are sent to us — macOS handles crash reporting through Apple's own systems, subject to your macOS privacy settings.
• No advertising or ad networks.
• No third-party SDKs that collect data.
• No account creation required — the App has no user accounts or login.

Because PasteSpace collects zero personal data, it is inherently compliant with major data privacy regulations worldwide, including the European Union's General Data Protection Regulation (GDPR), the California Consumer Privacy Act (CCPA), and similar frameworks. There is no personal data to collect, process, share, or delete — your privacy is protected by design.

### 3. Data Stored Locally on Your Device
PasteSpace stores the following data locally within its macOS App Sandbox container:

• Clipboard History: Text, images, and file references copied to your system clipboard. Stored in a local SQLite database.
• Vault Items: Clipboard content that has been encrypted using AES-256-GCM. The ciphertext, nonce, and authentication tag are stored in the same local database.
• OCR Text: Text extracted from copied images using Apple's Vision framework, stored alongside the corresponding image in the local database.
• Settings & Preferences: Your configuration choices (toggle states, blocklist, hotkey), stored in UserDefaults within the App Sandbox.
• Encryption Key: Stored in macOS Keychain (hardware-backed on Apple Silicon) with a file backup in the sandboxed Application Support directory. The key never leaves your device.
• Purchase Status: StoreKit transaction data managed by Apple's frameworks, verified on-device via JWS (JSON Web Signature). No purchase data is sent to any server.

### 4. Clipboard Monitoring
PasteSpace monitors your macOS system clipboard (NSPasteboard) at regular intervals to detect new copied content. This is the App's core functionality.

• Monitoring runs only while PasteSpace is active.
• You can pause or stop monitoring at any time by quitting the App.
• You can exclude specific apps from being monitored using the App Blocklist (Pro feature) or by adding them to the blocklist in Settings.
• In the Free tier, content from known password managers is automatically blocked.
• In the Pro tier with Vault Mode, password manager content can optionally be captured and encrypted.

### 5. Sensitive Data Detection
When Vault Mode is enabled (Pro), PasteSpace performs local pattern matching to automatically detect potentially sensitive content, including:

• Credit/debit card numbers
• IBANs and bank account numbers
• API keys, tokens (GitHub, Slack, Stripe, JWT, etc.)
• SSH keys and fingerprints
• Software license keys
• Passwords copied from password managers
• OTP codes from authenticator apps
• High-entropy strings that may be secrets

All detection is performed locally using regular expressions. No data is sent anywhere for analysis.

### 6. Encryption & Security
Vault Mode uses industry-standard encryption:

• Algorithm: AES-256-GCM (Authenticated Encryption with Associated Data)
• Implementation: Apple's CryptoKit framework (not a custom or third-party implementation)
• Key Storage: macOS Keychain with kSecAttrAccessibleWhenUnlockedThisDeviceOnly — the key is accessible only when your Mac is unlocked and never backed up to iCloud or transferred to another device
• Hardware Backing: On Macs with Apple Silicon (M1/M2/M3/M4) or T2 chip, the Keychain is anchored to the Secure Enclave
• File Backup: A synchronized copy of the key is kept in the sandboxed Application Support directory with POSIX 0600 permissions as a safety net

PasteSpace uses Apple's CryptoKit, which is exempt from U.S. export encryption regulations (ITSAppUsesNonExemptEncryption = false).

### 7. Biometric Data (Touch ID)
PasteSpace uses Apple's LocalAuthentication framework to authenticate users via Touch ID or device password when accessing Vault items.

• PasteSpace never accesses your fingerprint or biometric data directly.
• All biometric processing is handled by macOS and the Secure Enclave.
• The App only receives a success or failure result from the system.
• No biometric data is stored, transmitted, or logged by PasteSpace.

### 8. OCR (Image Text Extraction)
The OCR feature uses Apple's Vision framework (VNRecognizeTextRequest) to extract text from copied images.

• All processing happens locally on your device's CPU/GPU.
• No images are uploaded to any server.
• Extracted text is stored in the local database alongside the original image and is searchable within the App.

### 9. In-App Purchases
PasteSpace uses Apple's StoreKit 2 framework for the Pro upgrade:

• Transaction verification is performed on-device using JWS (JSON Web Signature).
• No purchase data is sent to any external server.
• Purchase history is stored locally by Apple's StoreKit framework.
• We do not have access to your Apple ID, payment method, or billing information.

### 10. Third-Party Services
PasteSpace does not integrate with any third-party services, analytics platforms, crash reporting tools, advertising networks, or cloud storage providers.

The only external communication is between StoreKit and Apple's App Store servers for purchase verification — this is handled entirely by Apple's frameworks and is subject to Apple's Privacy Policy.

### 11. Data Retention & Deletion
• Clipboard history can be cleared at any time using the Clear button. Pinned and Vault items are excluded from clearing.
• Vault items can be deleted using "Clear Vault" in Settings.
• Ephemeral Mode (Pro) automatically deletes non-Vault clipboard history when your Mac restarts.
• Uninstalling PasteSpace removes all data stored in the App Sandbox, including the database, settings, and encryption key backup file. Keychain entries may persist until manually deleted or the Keychain is reset.

### 12. Children's Privacy
PasteSpace is not directed at children under the age of 13. We do not knowingly collect personal information from children. Since no data is collected from any user, this policy applies equally to all age groups.

### 13. macOS Permissions
PasteSpace requires the following macOS permissions to function:

• Clipboard Access (NSPasteboard): To monitor and record clipboard content.
• Touch ID / Device Password (LocalAuthentication): To authenticate access to Vault items.
• App Sandbox: The App runs within Apple's App Sandbox, which restricts access to the file system and other apps' data.
• File Access (security-scoped bookmarks): To access files copied from Finder for preview and storage purposes.

### 14. Changes to This Policy
We may update this Privacy Policy from time to time. Changes will be reflected in the "Last Updated" date at the top of this document. Continued use of the App after changes constitutes your acceptance of the updated policy.

### 15. Contact
If you have questions or concerns about this Privacy Policy, you can contact us at: mariuscpopescu@icloud.com
