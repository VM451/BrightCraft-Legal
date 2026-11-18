# Privacy Policy for Brightcraft

**Effective Date:** November 18, 2026  
**Last Updated:** November 18, 2026  
**Developer:** Nitiphoom Phothichai (`nitiptc`)  
**Contact:** [nitiphoom.dev@gmail.com](mailto:nitiphoom.dev@gmail.com)

Brightcraft is a privacy-first, on-device business workspace for iOS and iPadOS. We built Brightcraft so your business ideas, product plans, research notes, and AI conversations stay under your control on your device by default.

## Summary

- **On-device by default:** Workspaces, notes, playbooks, metrics, chat history, and settings are stored locally on your device.
- **On-device AI inference:** Free tier (`Apple Foundation Model` on supported hardware and LiquidAI `LFM2.5-VL 450M` via `llama.cpp`) and Pro tier (LiquidAI `LFM3-VL 2B` via `llama.cpp`) run locally on your device. Your prompts and attached images never leave your device for AI model inference.
- **No private backend servers for your content:** Nothing syncs off your device unless you turn on private **iCloud Sync**.
- **No ads and no tracking:** We display no third-party advertisements, use no cross-app tracking SDKs (`NSPrivacyTracking = false`), and never sell your personal information.
- **You control deletion:** You can delete your account and linked cloud records directly inside the app (`Settings → Apple Account → Delete Account`).

---

## 1. Data Stored on Your Device

By default, everything you create in Brightcraft lives only on your iPhone or iPad:

- **Workspace Content:** Projects, business ideas, competitor notes, playbooks, metrics, tasks, and Markdown documents (stored via local SwiftData).
- **On-Device AI Activity:** Prompts, chat history, and images attached for vision analysis are processed locally by the selected on-device model (`Apple Foundation Model`, `LFM2.5-VL 450M`, or `LFM3-VL 2B`) and are not transmitted to external AI APIs.
- **Model Artifact Downloads:** When you download an optional LiquidAI GGUF model and multimodal projector (`LFM2.5-VL 450M` or `LFM3-VL 2B`), your device downloads the static model weights over HTTPS/TLS from **Hugging Face** (`huggingface.co`). No chat prompts, workspace content, or personal identifiers are sent during this download.
- **Sign in with Apple Identity:** When you sign in with Apple, the name and email address you choose to share (including Apple Private Email Relay addresses) and your stable Apple user identifier are stored locally in the app's preferences/Keychain to keep you signed in and display your account profile.
- **Service Credentials:** Any optional user-configured credentials or keys are stored locally in the iOS Keychain with hardware-backed protection.

---

## 2. Optional Private iCloud Sync

If **iCloud Sync** is enabled (`Settings → iCloud Sync`), Brightcraft syncs your workspaces, workspace items, and synced profile details across devices signed in to your same Apple Account using Apple's **CloudKit Private Database**:

- Synced records live inside **your own private iCloud storage quota**; we cannot browse or access your private iCloud container.
- Apple processes iCloud data in accordance with the [Apple Privacy Policy](https://www.apple.com/legal/privacy/).
- Turning iCloud Sync off stops future network synchronization immediately and never deletes local data on your device.

---

## 3. User-Initiated Online Features & Third-Party Requests

Brightcraft includes optional features that access the public internet only when you trigger or configure them. Each request is sent over encrypted HTTPS/TLS directly from your device:

- **Web Search & Competitor Research:** Search queries you run may be sent to **DuckDuckGo** or, if you configure one in `Settings → Capabilities → SearXNG`, your own HTTPS **SearXNG** instance.
- **Brand Icons & Cover Photos:** Public domain company/source logos (`SourceLogoService` via Eulerpool) and optional stock workspace covers (**Unsplash**) fetch public static imagery without user workspace content.
- **Optional Workspace Tools (if configured):** If an external memory namespace (`Mem0`) or sandboxed runner (`E2B`) is configured, only requests needed for those actions are sent under a one-way hashed namespace ID rather than your name, email, or Apple ID.

We never send your Keychain secrets, Contacts, Photos library, precise location, microphone audio, or device advertising identifiers (`IDFA`) to third parties.

---

## 4. Subscriptions & Billing

Pro subscriptions (**Brightcraft Pro Monthly** and **Brightcraft Pro Annual**) are processed exclusively by **Apple** through the App Store using StoreKit 2:

- We never receive, process, or store your credit card, banking, or billing details.
- Apple provides the app with anonymous/signed transaction verification records (product identifier, expiration/renewal date, subscription standing) solely to unlock Pro features on your Apple Account.
- Manage, cancel, or request refunds through your Apple Account subscription settings (`iPhone Settings → [Your Name] → Subscriptions`).

---

## 5. Permissions

Brightcraft operates with minimal platform access:

- **Sign in with Apple / iCloud:** Used solely for authentication and user-enabled Private CloudKit sync.
- **Photo Library (Picker):** When you select a photo to analyze with a local multimodal model or attach to a workspace item, iOS grants temporary read access solely to the specific photo(s) you select via the system picker.
- **No Tracking:** Brightcraft does not request App Tracking Transparency (`NSUserTrackingUsageDescription`) permission because it performs zero tracking.

---

## 6. Data Retention & Account Deletion

- **On-Device Content:** Retained locally until you delete items, clear workspace data, delete your account, or uninstall Brightcraft.
- **Private iCloud Data:** Retained in your private CloudKit database until deleted by you in the app or removed via iOS iCloud storage settings.
- **In-App Account Deletion:** Open **Settings → Apple Account → Delete Account** to permanently remove your CloudKit profile record, clear linked cloud namespaces (retried automatically if offline), wipe local account preferences/identity/secrets, and sign out. You can also revoke Sign in with Apple authorization in `iOS Settings → Apple Account → Sign in with Apple`. Full instructions: [ACCOUNT-DELETION.md](https://github.com/VM451/BrightCraft-Legal/blob/main/ACCOUNT-DELETION.md).

---

## 7. Children's Privacy

Brightcraft is intended for users aged **13 and older** (or the minimum digital consent age in your jurisdiction). We do not knowingly collect personal information from children under 13. If you believe a child has provided personal data, please contact us so we can assist with removal.

---

## 8. International Privacy Rights (GDPR, UK GDPR, PDPA, CCPA/CPRA)

Because we do not operate developer servers holding your workspace content, you exercise direct control over access, correction, export, and deletion inside Brightcraft on your device. For any privacy inquiry, data access question, or legal request under Thailand's Personal Data Protection Act (PDPA), GDPR, or US state privacy laws, contact us at **[nitiphoom.dev@gmail.com](mailto:nitiphoom.dev@gmail.com)**.

---

## 9. Changes to This Policy

We host the authoritative Privacy Policy in this repository so updates take effect without requiring an app binary update. When we update this policy, we revise the **Last Updated** date above and note material changes in [CHANGELOG.md](https://github.com/VM451/BrightCraft-Legal/blob/main/CHANGELOG.md).
