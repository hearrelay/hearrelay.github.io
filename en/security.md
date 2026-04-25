---
title: Security — HearRelay
lang: en
---

# Security

Thank you for helping us keep HearRelay users safe. This page explains how to report vulnerabilities and summarises HearRelay's security posture.

---

## Reporting a vulnerability

Please email **hearrelay-security@conex-cp.com** with the following information:

- A clear description of the issue
- Steps to reproduce (or proof-of-concept)
- The version of HearRelay and the iOS / iPadOS version used
- Any suggested mitigation you have in mind
- Whether you would like public credit

We prefer email for the initial report. If needed, we can set up a **GitHub Security Advisory (Private Disclosure)** for ongoing coordination.

**Please do not** publish details of a vulnerability before we have had a chance to respond and ship a fix.

---

## Safe-harbor for good-faith security research

We do not currently offer a bug bounty or monetary rewards.

When testing or reporting vulnerabilities, please:

- **Do not** access, modify, delete, or exfiltrate data that does not belong to you.
- **Do not** perform denial-of-service testing, spam, phishing, social-engineering attacks, or any physical attack.
- **Do not** test against Apple services, third-party hardware, or any system you do not own.
- Limit testing to your own devices and your own Apple ID.

If you make a good-faith report within the scope of this policy and comply with these rules, **CONEX will not intentionally pursue legal action against you based solely on that report**, subject to applicable law. This safe-harbor commitment does not waive any rights you have under applicable law and does not bind any third party (including Apple).

---

## What we consider in-scope

The following are in-scope for reporting:

- The HearRelay iOS / iPadOS app
- The HearRelay Secure Channel handshake (X25519 ECDH + P-256 ECDSA + ChaCha20-Poly1305 AEAD)
- The iCloud Key-Value Storage–based peer discovery process
- Local file handling (recording storage and automatic deletion)
- The project website at `hearrelay.app`

---

## Out of scope

- Vulnerabilities in Apple's operating systems, frameworks, or iCloud infrastructure — please report those to Apple directly
- Vulnerabilities in third-party Wi-Fi routers, Bluetooth headphones, or other hardware
- Social-engineering attacks against the developer or other users
- Missing security headers on GitHub Pages beyond what the platform allows us to configure
- Issues requiring a jailbroken or otherwise compromised device

---

## Response targets

| Severity | First response | Target resolution |
|---|---|---|
| Critical | within 24 hours | within 7 days |
| High | within 3 days | within 30 days |
| Medium / Low | within 7 days | next regular release |

These are targets, not guarantees.

---

## Coordinated disclosure

- We will keep you informed as we investigate.
- We will agree on a public disclosure date together, usually when a fix is released.
- On release, we will publish a security advisory and (with your permission) credit you.

---

## Security posture summary

HearRelay is designed around three principles:

1. **Data minimisation** — audio and recordings never leave your device; no analytics or advertising SDKs.
2. **Local network only** — paired devices communicate exclusively over the same Wi-Fi / local network, never over the internet.
3. **Cryptographic peer identity** — devices identify each other with **P-256** signing keys (stored in the **Secure Enclave** where supported, with a Keychain fallback), and discover each other via iCloud Key-Value Storage scoped to your Apple ID.

Transport uses the **HearRelay Secure Channel**: X25519 ECDH for forward-secret key agreement, ChaCha20-Poly1305 AEAD with replay protection, and per-frame counter-derived nonces.

You can rotate your device's identity key, forget a peer device, or wipe all device security state at any time from **Settings → Security** in the App.

For a fuller internal write-up, see the project design docs.

---

## Contact

- Security reports: **hearrelay-security@conex-cp.com**
- General contact: **hearrelay-support@conex-cp.com**

---

**Translations are available in:** [日本語](/ja/security/) · [Français](/fr/security/) · [Español](/es/security/) · [Português (Brasil)](/pt-BR/security/) · [简体中文](/zh-Hans/security/)

Where this page is provided in any language other than English, the **English version controls** to the extent permitted by applicable law. This precedence rule does not limit any rights granted to you by mandatory consumer-protection, privacy, or data-protection laws of your country or region.
