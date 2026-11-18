# Account & Data Deletion Guide

**Effective Date:** November 18, 2026  
**Support Contact:** [nitiphoom.dev@gmail.com](mailto:nitiphoom.dev@gmail.com)

In accordance with Apple App Store Review Guideline **5.1.1(v)**, you can permanently delete your Brightcraft account directly inside the app at any time.

---

## Delete Your Account in the App

1. Open **Brightcraft** on your iPhone or iPad.
2. Open **Settings** (from the sidebar bottom row on iPad, or the top-leading account menu on iPhone).
3. Tap **Apple Account** at the top of the Settings screen.
4. Scroll to the bottom and tap **Delete Account**.
5. Confirm by tapping **Delete** in the confirmation alert.

### What Deletion Removes Immediately

- **CloudKit Profile Record:** Deletes your synced account profile record from your private iCloud container.
- **Linked Cloud Memory Namespace (if applicable):** Queues and executes deletion of any associated Mem0 namespace (automatically retried if offline when requested).
- **On-Device Account Traces:** Clears your saved Sign in with Apple name, email, user identifier, preferences, shared-link history, and Keychain tokens, and signs you out immediately.
- **Local Workspaces:** As noted in the confirmation alert, local workspace rows remain on your device so you do not lose local notes if you reinstall or sign back in — and they are automatically purged if a **different** Apple Account signs in on the device.

---

## Revoke Sign in with Apple Access (iOS System Setting)

To revoke Brightcraft's Sign in with Apple token at the OS level:

1. Open **iPhone Settings → [Your Name] → Sign-In & Security → Sign in with Apple**.
2. Select **Brightcraft**.
3. Tap **Stop Using Apple ID**.

---

## Removing Local & iCloud Data Completely

- **Delete Local App Data:** Uninstall **Brightcraft** from your iPhone or iPad Home Screen.
- **Delete iCloud Data:** Open **iPhone Settings → [Your Name] → iCloud → Saved to iCloud → Brightcraft** (or **Manage Account Storage**) to remove synced container data.

For assistance, email **[nitiphoom.dev@gmail.com](mailto:nitiphoom.dev@gmail.com)**.
