---
title: Privacy Policy — HearRelay
lang: en
---

# Privacy Policy

**Effective date: 2026-04-25**
**Last updated: 2026-04-25**

HearRelay ("the App") is designed to be private by default. This policy explains what data is, and is not, processed when you use HearRelay.

If you have any questions, please contact us at **hearrelay-privacy@conex-cp.com**.

---

## 1. Who we are

HearRelay is developed by **CONEX Corporation** (株式会社CONEX), a company incorporated in Japan ("the Developer", "we", "us", "CONEX"). The App is designed so that audio, recordings, payment information, advertising identifiers, analytics, and tracking data are not transmitted to CONEX servers. CONEX does not operate any backend server for the App.

To the extent any limited device-discovery information is processed by Apple within your Apple ID account (see §4), CONEX does not access or operate that processing. Where applicable law nonetheless treats such information as "personal data," CONEX cooperates in good faith with information requests under §10.

For correspondence, please use the email addresses at the bottom of this page.

---

## 2. Data we do not collect

CONEX does **not** collect or receive on its own servers, store, or share any of the following:

- Audio picked up by your device's microphone
- Audio recordings you create with the App
- Contact information, location, photos, camera data, or device identifiers
- Advertising identifiers (IDFA, IDFV used for tracking)
- Analytics, crash telemetry routed to third-party services, or behavioural profiles
- Payment card or billing details (Apple processes purchases — see §7)

HearRelay does not contain any third-party SDKs for analytics, advertising, or tracking.

---

## 3. Data processed locally on your device

The App processes the following on your device, and **only on your device**:

| Data | Purpose | Retention |
|---|---|---|
| Microphone audio (live) | Real-time monitoring to headphones or to a paired device on the same Wi-Fi | Not stored |
| Audio recordings (optional) | You can record sessions manually | Deleted automatically after 24 hours by default; you may extend or delete earlier |
| Connection history (peer name, last connected time) | Convenience feature to reconnect quickly | Stored locally; cleared when you uninstall the App |
| App preferences (including trial start date for purchase gating) | Remember your settings | Stored locally |

When you uninstall the App, all of the above data is removed with it.

---

## 4. Limited information processed by Apple iCloud (Apple ID scope)

To let your own Apple devices find each other on the same Wi-Fi, the App causes the following limited device-discovery information to be stored in **Apple iCloud Key-Value Storage** within your Apple ID account:

- A cryptographic **public key** generated on your device
- A **SHA-256 fingerprint** of that public key
- Your device's **name** (as set in iOS Settings → General → About → Name)
- Your device's **platform**, **model**, and the installed **app version**
- The **creation date** and **last-rotation date** of the key

This information is stored within your own Apple ID scope, inside Apple's iCloud service, and is not visible to other Apple ID holders or to CONEX. CONEX does not operate Apple iCloud and does not access this information on its own servers. Apple's handling is governed by Apple's own privacy policy and the iCloud terms.

**Depending on applicable law and your device-name settings, some of this information may be considered personal data** — for example, if your device name contains your full name. We describe it here for transparency. You can change your device name at any time in iOS Settings, and you can purge the App's identity (rotating its key and clearing the entry) from **Settings → Security → Reset all device security** in the App.

---

## 5. Network communication

HearRelay communicates **only** with other Apple devices that are:

1. Signed in to the same Apple ID, **and**
2. Connected to the same Wi-Fi / local network

Communication is encrypted with the **HearRelay Secure Channel** (X25519 ECDH key agreement + ChaCha20-Poly1305 AEAD with replay protection). HearRelay does **not** send any data over the internet to remote servers, nor does it support remote monitoring across networks. Remote use is deliberately prohibited to prevent covert surveillance.

---

## 6. Audio recordings you create

If you enable the recording feature:

- Recordings are saved **only on the device that created them**
- Recordings are stored inside the App's sandbox with **file-level encryption** (`NSFileProtectionComplete`)
- Recordings are **automatically deleted 24 hours** after creation, unless you explicitly choose to preserve them
- You can share or export recordings through iOS's share sheet, under your control
- Recordings are never uploaded to CONEX or to any third party by the App

You are responsible for confirming that any recording or live monitoring you perform complies with all applicable laws — including consent requirements that may apply where you are. See our [Terms of Use](/en/terms/) and [Support](/en/support/) for more.

---

## 7. Third parties, payments, and the App Store

- CONEX does **not** share data with any third party.
- The App does **not** use advertising, analytics, or profiling SDKs.
- CONEX does **not** sell or rent data of any kind.

Distribution and payments are handled by Apple through the App Store and In-App Purchase. **HearRelay Full Access is a Non-Consumable, one-time purchase, not an auto-renewing subscription.** Prices, taxes, refunds, and billing are processed by Apple under the App Store and Apple Media Services Terms. CONEX does not receive payment card numbers or billing details. You can restore a previous purchase using the **Restore Purchases** option in the App.

When Apple processes your purchase or delivers updates, Apple's own privacy policy applies to that activity. Any diagnostic information Apple collects from your device (e.g. crash logs sent through "Share With App Developers") is governed by your iOS Settings and Apple's developer terms.

---

## 8. Our website

The HearRelay website at <https://hearrelay.app/> is a static informational site hosted on GitHub Pages. We do **not** use advertising cookies, analytics cookies, tracking pixels, or third-party marketing tags. If this changes, we will update this Policy and provide any notices or choices required by applicable law.

---

## 9. International users

Because HearRelay does not transfer data out of your devices to CONEX servers, there is no international transfer of personal data performed by CONEX.

### 9.1 Users in the European Economic Area (EEA), United Kingdom, Switzerland

The App is designed so that CONEX does not collect or receive audio, recordings, payment information, analytics data, advertising identifiers, or tracking data on its own servers.

Limited device-discovery information may be stored in Apple iCloud within your Apple ID account (§4). CONEX does not operate Apple iCloud and does not access this information on its own servers. Where applicable law treats this information as personal data, the **purposes** of any such processing are limited to enabling device discovery, mutual authentication, security, and local peer-to-peer communication between your own devices; the **legal basis** is your consent to use the App for that purpose, and your legitimate interest in connecting your own devices privately.

CONEX has assessed the requirement under GDPR Article 27 to designate an EU representative and concluded that the limited, occasional, and low-risk nature of any processing falls within the exemption in Article 27(2)(a). This determination is documented internally and is reviewed when material facts change. If you are a supervisory authority or a data subject in the EEA who needs to reach us, please use **hearrelay-privacy@conex-cp.com** — we commit to responding within statutory timeframes.

### 9.2 Users in Brazil

The App's processing posture under LGPD mirrors §9.1. CONEX is not aware of any personal data processed on its own servers. CONEX has not appointed a local Encarregado (DPO) on the basis that no large-scale or high-risk personal-data processing occurs through CONEX. The contact above serves as the point of contact for LGPD requests.

### 9.3 Users in Japan

CONEX does not include third-party advertising, analytics, or tracking SDKs in the App, and does not transmit user-related information to its own servers. Apple iCloud Key-Value Storage is used solely to synchronize the limited device-discovery information described in §4 within your own Apple ID account; CONEX does not receive this information on its own servers. We refer to this configuration in good faith when assessing Japan's external-transmission notification regime under the Telecommunications Business Act.

### 9.4 Users in Hong Kong / Taiwan

The same processing posture applies. CONEX is mindful that PDPO (Hong Kong) and the Personal Information Protection Act (Taiwan) define personal data and personal information broadly; please refer to §4 and §10 for our position and the rights you may exercise.

---

## 10. Children's privacy

HearRelay is a utility intended for adults, typically parents or caregivers. It is **not directed at children under 13**, and CONEX does not knowingly collect personal data from children. The App's processing is local to your device, so no personal data of children is collected, stored, or transmitted to CONEX.

---

## 11. Your rights

Because CONEX holds no personal data about you on its servers, there is typically nothing for us to access, correct, delete, export, or restrict. Nevertheless, depending on your location (EEA, UK, California, Brazil, Japan, Hong Kong, Taiwan, etc.), you may have statutory rights, including:

- Right of access
- Right to rectification
- Right to erasure
- Right to object or restrict processing
- Right to data portability
- Right to opt out of "sale" or "sharing" — CONEX does not sell or share personal data
- Right to lodge a complaint with your local supervisory authority

To exercise any right, contact **hearrelay-privacy@conex-cp.com**. Please note that to delete all data the App has stored locally, you only need to uninstall the App from your device. To purge the App's per-device identity from Apple iCloud (§4), use **Settings → Security → Reset all device security** in the App.

---

## 12. Security

We use industry-standard protections:

- **HearRelay Secure Channel** (X25519 ECDH + ChaCha20-Poly1305 AEAD) for all device-to-device communication
- **P-256** identity keys generated and stored in the **Secure Enclave** where supported, with a Keychain fallback
- **Public-key pinning** through an iCloud-scoped trust list to prevent impostor devices from connecting
- **File protection** (`NSFileProtectionComplete`) for local recordings

No method of transmission or storage is perfectly secure. To report a vulnerability, please see our [Security page](/en/security/) and email **hearrelay-security@conex-cp.com**.

---

## 13. Changes to this policy

We may revise this Privacy Policy. The revision date will be updated at the top of this page, and material changes will be announced in the App's release notes. Where applicable law requires, we will obtain your consent or provide you with reasonable advance notice and a meaningful opportunity to stop using the App before the change takes effect.

---

## 14. Contact

- Privacy: **hearrelay-privacy@conex-cp.com**
- Support: **hearrelay-support@conex-cp.com**
- Security: **hearrelay-security@conex-cp.com**
- Web: <https://hearrelay.app/>

---

**Translations are available in:** [日本語](/ja/privacy/) · [Français](/fr/privacy/) · [Español](/es/privacy/) · [Português (Brasil)](/pt-BR/privacy/) · [简体中文](/zh-Hans/privacy/)

Where this Policy is provided in any language other than English, the **English version controls** to the extent permitted by applicable law. This precedence rule does not limit any rights granted to you by mandatory consumer-protection, privacy, or data-protection laws of your country or region.
