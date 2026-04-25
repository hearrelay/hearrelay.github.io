---
title: Privacy Policy — HearRelay
lang: en
---

# Privacy Policy

**Effective date: 2026-04-24**
**Last updated: 2026-04-24**

HearRelay ("the App") is designed to be private by default. This policy explains what data is, and is not, processed when you use HearRelay.

If you have any questions, please contact us at **hearrelay-privacy@conex-cp.com**.

---

## 1. Who we are

HearRelay is developed by **CONEX Corporation** (株式会社CONEX), a company incorporated in Japan ("the Developer", "we", "us"). Because HearRelay processes no personal data on our servers, we do not act as a "data controller" in any meaningful sense — we are the app's publisher. For correspondence, please use the email addresses at the bottom of this page.

---

## 2. Data we do not collect

We do **not** collect, store, transmit to our servers, or share any of the following:

- Audio picked up by your device's microphone
- Audio recordings you create with the App
- Contact information, location, photos, camera data, or device identifiers
- Advertising identifiers (IDFA, IDFV used for tracking)
- Analytics, crash telemetry routed to third-party services, or behavioural profiles

HearRelay does not contain any third-party SDKs for analytics, advertising, or tracking.

---

## 3. Data processed locally on your device

The App processes the following on your device, and **only on your device**:

| Data | Purpose | Retention |
|---|---|---|
| Microphone audio (live) | Real-time monitoring to headphones or to a paired device on the same Wi-Fi | Not stored |
| Audio recordings (optional) | You can record sessions manually | Deleted automatically after 24 hours by default; you may extend or delete earlier |
| Connection history (peer name, last connected time) | Convenience feature to reconnect quickly | Stored locally; cleared when you uninstall the App |
| App preferences | Remember your settings | Stored locally |

When you uninstall the App, all of the above data is removed with it.

---

## 4. Data briefly handled by Apple's infrastructure

To let your own Apple devices find each other on the same Wi-Fi, HearRelay uses **iCloud Key-Value Storage**, provided by Apple, to publish:

- A cryptographic **public key** generated on your device
- A **fingerprint** (SHA-256) of that key
- Your device's **name**, **platform**, **model**, and the **app version**

This data is stored within your own Apple ID scope, inside Apple's iCloud service, and is not visible to other Apple ID holders or to us. The Developer operates no servers and has no access to this data. Apple's handling is governed by Apple's own privacy policy.

---

## 5. Network communication

HearRelay communicates **only** with other Apple devices that are:

1. Signed in to the same Apple ID, **and**
2. Connected to the same Wi-Fi / local network

Communication is encrypted with **TLS 1.3**. HearRelay does **not** send any data over the internet to remote servers, nor does it support remote monitoring across networks. Remote use is deliberately prohibited to prevent covert surveillance.

---

## 6. Audio recordings you create

If you enable the recording feature:

- Recordings are saved **only on the device that created them**
- Recordings are stored inside the App's sandbox with **file-level encryption** (`NSFileProtectionComplete`)
- Recordings are **automatically deleted 24 hours** after creation, unless you explicitly choose to preserve them
- You can share or export recordings through iOS's share sheet, under your control
- Recordings are never uploaded to us or to any third party by the App

---

## 7. Third parties

- We do **not** share data with any third party.
- We do **not** use advertising, analytics, or profiling SDKs.
- We do **not** sell or rent data of any kind.

Distribution and payment are handled by Apple through the App Store under Apple's own terms. When Apple processes your purchase or delivers updates, Apple's privacy policy applies to that activity.

---

## 8. International users

Because HearRelay does not transfer data out of your devices, there is no international transfer of personal data performed by us.

---

## 9. Children's privacy

HearRelay is a utility intended for adults, typically parents or caregivers. It is **not directed at children under 13**, and we do not knowingly collect personal data from children. The App's processing is local to your device, so no personal data of children is collected, stored, or transmitted.

---

## 10. Your rights

Because we hold no personal data about you, there is typically nothing for us to access, correct, delete, export, or restrict. Nevertheless, depending on your location (EEA, UK, California, Brazil, Japan, etc.), you may have statutory rights, including:

- Right of access
- Right to rectification
- Right to erasure
- Right to object or restrict processing
- Right to data portability
- Right to lodge a complaint with your local supervisory authority

To exercise any right, contact us at **hearrelay-privacy@conex-cp.com**. Please note that to delete all data the App has stored locally, you only need to uninstall the App from your device.

---

## 11. Security

We use industry-standard protections:

- **TLS 1.3** for all device-to-device communication
- **Curve25519 / P-256** keys generated and stored in the **Secure Enclave** where supported
- **Public-key pinning** to prevent impostor devices from connecting
- **File protection** (`NSFileProtectionComplete`) for local recordings

No method of transmission or storage is perfectly secure. To report a vulnerability, please see our [Security page](/en/security/) and email **hearrelay-security@conex-cp.com**.

---

## 12. Changes to this policy

We may revise this Privacy Policy. The revision date will be updated at the top of this page, and material changes will be announced in the App's release notes. Continuing to use the App after changes take effect constitutes acceptance.

---

## 13. Contact

- Privacy: **hearrelay-privacy@conex-cp.com**
- Support: **hearrelay-support@conex-cp.com**
- Security: **hearrelay-security@conex-cp.com**
- Web: <https://hearrelay.app/>

---

**日本語版は** [こちら](/ja/privacy/) **をご覧ください。**
