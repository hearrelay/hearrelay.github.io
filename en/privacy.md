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

To the extent any limited device-discovery information is processed by Apple within your Apple ID account (see §5), CONEX does not access or operate that processing. Where applicable law nonetheless treats such information as "personal data," CONEX cooperates in good faith with information requests under §12.

If you choose to contact us by email — for support, privacy, security, or other inquiries — CONEX will receive the contents of those emails (see §4).

For correspondence, please use the email addresses at the bottom of this page.

---

## 2. Data we do not collect through the App

Except for information you choose to send to us directly (see §4), CONEX does **not** collect or receive on its own servers, store, or share any of the following through the App:

- Audio picked up by your device's microphone
- Audio recordings you create with the App
- Contact information, location, photos, camera data, or device identifiers
- Advertising identifiers (IDFA, IDFV used for tracking)
- Analytics, crash telemetry routed to third-party services, or behavioural profiles
- Payment card or billing details (Apple processes purchases — see §8)

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

## 4. Communications you send to us

The App is designed so that CONEX does not collect or receive personal data through the App on its own servers.

However, if you choose to contact CONEX by email for support, privacy requests, security reports, refund-related questions, or other inquiries, **we will receive the information you choose to send**. This may include:

- Your email address
- Your name, if included in your message
- The contents of your message
- Device model, iOS / iPadOS version, app version
- Screenshots, logs, reproduction steps
- Vulnerability details (in security reports)

**Purpose.** CONEX uses this information only to respond to your inquiry, provide support, investigate security issues, comply with legal obligations, and protect the App and our users. We do **not** use support, privacy, or security correspondence for advertising, tracking, or profiling.

**Service providers.** These communications may be processed by our email, hosting, or security-reporting service providers. Depending on the provider, the information may be stored or processed in Japan or other countries.

**Retention.** We retain support, privacy, and security correspondence only for as long as reasonably necessary for the purpose for which it was provided, unless a longer retention period is required or permitted for legal, security, dispute-resolution, or compliance purposes.

---

## 5. Limited information processed by Apple iCloud (Apple ID scope)

To let your own Apple devices find each other on the same Wi-Fi, the App causes the following limited device-discovery information to be stored in **Apple iCloud Key-Value Storage** within your Apple ID account:

- A cryptographic **public key** generated on your device
- A **SHA-256 fingerprint** of that public key
- Your device's **name** (as set in iOS Settings → General → About → Name)
- Your device's **platform**, **model**, and the installed **app version**
- The **creation date** and **last-rotation date** of the key

This information is stored within your own Apple ID scope, inside Apple's iCloud service, and is not visible to other Apple ID holders or to CONEX. CONEX does not operate Apple iCloud and does not access this information on its own servers. Apple's handling is governed by Apple's own privacy policy and the iCloud terms.

**Depending on applicable law and your device-name settings, some of this information may be considered personal data** — for example, if your device name contains your full name. We describe it here for transparency. You can change your device name at any time in iOS Settings, and you can purge the App's identity (rotating its key and clearing the entry) from **Settings → Security → Reset all device security** in the App.

---

## 6. Network communication

HearRelay communicates **only** with other Apple devices that are:

1. Signed in to the same Apple ID, **and**
2. Connected to the same Wi-Fi / local network

Communication is encrypted with the **HearRelay Secure Channel** (X25519 ECDH key agreement + ChaCha20-Poly1305 AEAD with replay protection). HearRelay does **not** send any data over the internet to remote servers, nor does it support remote monitoring across networks. Remote use is deliberately prohibited to prevent covert surveillance.

---

## 7. Audio recordings you create

If you enable the recording feature:

- Recordings are saved **only on the device that created them**
- Recordings are stored inside the App's sandbox with **file-level encryption** (`NSFileProtectionComplete`)
- Recordings are **automatically deleted 24 hours** after creation, unless you explicitly choose to preserve them
- You can share or export recordings through iOS's share sheet, under your control
- Recordings are never uploaded to CONEX or to any third party by the App

You are responsible for confirming that any recording or live monitoring you perform complies with all applicable laws — including consent requirements that may apply where you are. See our [Terms of Use](/en/terms/) and [Support](/en/support/) for more.

---

## 8. Third parties, payments, and the App Store

- CONEX does **not** sell, rent, or share personal data for advertising, analytics, or tracking. Apple services and voluntary communications you send to us are described in this Policy (see §4 and §5).
- The App does **not** use advertising, analytics, or profiling SDKs.

Distribution and payments are handled by Apple through the App Store and In-App Purchase. **HearRelay Full Access is a Non-Consumable, one-time purchase, not an auto-renewing subscription.** Prices, taxes, refunds, and billing are processed by Apple under the App Store and Apple Media Services Terms. CONEX does not receive payment card numbers or billing details. You can restore a previous purchase using the **Restore Purchases** option in the App.

When Apple processes your purchase or delivers updates, Apple's own privacy policy applies to that activity. Any diagnostic information Apple collects from your device (e.g. crash logs sent through "Share With App Developers") is governed by your iOS Settings and Apple's developer terms.

---

## 9. Our website

The HearRelay website at <https://hearrelay.app/> is a static informational site hosted on GitHub Pages. We do **not** use advertising cookies, analytics cookies, tracking pixels, or third-party marketing tags.

As with most hosted websites, GitHub or infrastructure providers may process standard technical logs, such as IP addresses and request metadata, to deliver and secure the website. CONEX does not use these logs for advertising, analytics, or tracking.

If our use of the website materially changes, we will update this Policy and provide any notices or choices required by applicable law.

---

## 10. International users

Because HearRelay does not transfer data out of your devices to CONEX servers, there is no international transfer of personal data performed by CONEX. Voluntary email correspondence may be processed by service providers as described in §4.

### 10.1 Users in the European Economic Area (EEA), United Kingdom, Switzerland

The App is designed so that CONEX does not collect or receive audio, recordings, payment information, analytics data, advertising identifiers, or tracking data on its own servers.

Limited device-discovery information may be stored in Apple iCloud within your Apple ID account (§5). CONEX does not operate Apple iCloud and does not access this information on its own servers.

To the extent CONEX is regarded as a controller for such limited processing, the **purposes** of the processing are to enable device discovery, mutual authentication, security, and local peer-to-peer communication between your own devices.

The **legal bases** are:

- **performance** of the app license and related services requested by you, to enable device discovery, authentication, and local peer-to-peer communication (**GDPR Article 6(1)(b)**); and
- CONEX's **legitimate interests** in maintaining the security, integrity, abuse prevention, and privacy-preserving local-network architecture of the App (**GDPR Article 6(1)(f)**).

Where applicable law requires consent for a specific operation, **we will request and rely on your consent before that operation** (**GDPR Article 6(1)(a)**). You may withdraw that consent by disabling iCloud for the App, resetting the App's device security settings, or uninstalling the App, although doing so may prevent device discovery or pairing from working.

For **voluntary email correspondence** (§4), the legal bases are performance of any support, pre-contractual, or contractual obligation requested by you (**GDPR Article 6(1)(b)**), and CONEX's legitimate interests in responding to inquiries and maintaining App security (**GDPR Article 6(1)(f)**).

**EU representative.** CONEX has not currently designated a representative in the EEA. Based on CONEX's current assessment, the App is designed so that CONEX does not collect personal data on its own servers, and any processing for which CONEX may be regarded as responsible is limited, low-risk, and connected to local device discovery and security. We will reassess this position if our processing activities, user base, distribution regions, applicable guidance, or regulatory expectations materially change. This does not limit your right to contact us at **hearrelay-privacy@conex-cp.com** or to lodge a complaint with a competent supervisory authority.

### 10.2 Users in Brazil

The App's processing posture under LGPD mirrors §10.1. CONEX is not aware of any personal data processed on its own servers other than voluntary email correspondence (§4). CONEX has not appointed a local Encarregado (DPO) on the basis that no large-scale or high-risk personal-data processing occurs through CONEX. The contact above serves as the point of contact for LGPD requests.

### 10.3 Users in Japan

CONEX does not include third-party advertising, analytics, or tracking SDKs in the App, and does not transmit user-related information to its own servers. Apple iCloud Key-Value Storage is used solely to synchronize the limited device-discovery information described in §5 within your own Apple ID account; CONEX does not receive this information on its own servers.

This disclosure is provided for transparency and for CONEX's voluntary assessment of Japan's external-transmission notice rules under the Telecommunications Business Act. CONEX does not use third-party advertising, analytics, or tracking SDKs, and does not receive this information on its own servers.

### 10.4 Users in Hong Kong / Taiwan

The same processing posture applies. CONEX is mindful that PDPO (Hong Kong) and the Personal Information Protection Act (Taiwan) define personal data and personal information broadly; please refer to §5 and §12 for our position and the rights you may exercise.

---

## 11. Children's privacy

HearRelay is a utility intended for adults, typically parents or caregivers. It is **not directed at children under 13**, and CONEX does not knowingly collect personal data from children. The App's processing is local to your device, so no personal data of children is collected, stored, or transmitted to CONEX.

---

## 12. Your rights

For data we do not hold (§2), there is typically nothing for us to access, correct, delete, export, or restrict. For voluntary email correspondence we do receive (§4), and to the extent applicable law treats Apple-iCloud-scope device-discovery information (§5) as your personal data, depending on your location (EEA, UK, California, Brazil, Japan, Hong Kong, Taiwan, etc.), you may have statutory rights, including:

- Right of access
- Right to rectification
- Right to erasure
- Right to object or restrict processing
- Right to data portability
- Right to opt out of "sale" or "sharing" — CONEX does not sell or share personal data
- Right to lodge a complaint with your local supervisory authority

To exercise any right, contact **hearrelay-privacy@conex-cp.com**. Please note that to delete all data the App has stored locally, you only need to uninstall the App from your device. To purge the App's per-device identity from Apple iCloud (§5), use **Settings → Security → Reset all device security** in the App.

---

## 13. Security

### Data flow at a glance

```text
[Device A microphone]
         |
         | local processing only
         v
[Device A App] <─── same-Wi-Fi P2P encrypted channel ───> [Device B App]
         |
         | device-discovery metadata only (see §5)
         v
[Apple iCloud Key-Value Storage, Apple ID scope]

[Apple App Store + In-App Purchase]   ─── Apple processes payments
[CONEX server]                        ─── none
[Third-party analytics / ads / tracking SDKs]   ─── none
```

### Technical protections

- **HearRelay Secure Channel** (X25519 ECDH + ChaCha20-Poly1305 AEAD) for all device-to-device communication
- **P-256** identity keys generated and stored in the **Secure Enclave** where supported, with a Keychain fallback
- **Public-key pinning** through an iCloud-scoped trust list to prevent impostor devices from connecting
- **File protection** (`NSFileProtectionComplete`) for local recordings

No method of transmission or storage is perfectly secure. To report a vulnerability, please see our [Security page](/en/security/) and email **hearrelay-security@conex-cp.com**.

---

## 14. Changes to this policy

We may revise this Privacy Policy. The revision date will be updated at the top of this page, and material changes will be announced in the App's release notes. Where applicable law requires, we will obtain your consent or provide you with reasonable advance notice and a meaningful opportunity to stop using the App before the change takes effect.

---

## 15. Contact

- Privacy: **hearrelay-privacy@conex-cp.com**
- Support: **hearrelay-support@conex-cp.com**
- Security: **hearrelay-security@conex-cp.com**
- Web: <https://hearrelay.app/>

---

**Translations are available in:** [日本語](/ja/privacy/) · [Français](/fr/privacy/) · [Español](/es/privacy/) · [Português (Brasil)](/pt-BR/privacy/) · [简体中文](/zh-Hans/privacy/)

Where this Policy is provided in any language other than English, the **English version controls** to the extent permitted by applicable law. This precedence rule does not limit any rights granted to you by mandatory consumer-protection, privacy, or data-protection laws of your country or region.
