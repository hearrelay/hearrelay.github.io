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

## What we consider in-scope

The following are in-scope for reporting:

- The HearRelay iOS / iPadOS app
- The cryptographic handshake and TLS transport used between paired devices
- The iCloud Key-Value Storage–based peer discovery process
- Local file handling (recording storage and automatic deletion)
- The project website at `hearrelay.github.io`

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

1. **Data minimisation** — no audio or recordings leave your device; no analytics or advertising SDKs.
2. **Local network only** — paired devices communicate exclusively over the same Wi-Fi / local network, never over the internet.
3. **Cryptographic peer identity** — devices identify each other with **Curve25519 / P-256** keys, protected in the **Secure Enclave** where supported, and discovered via iCloud Key-Value Storage scoped to your Apple ID.

Transport is encrypted with **TLS 1.3** using only the AEAD cipher suites provided by iOS.

For a fuller internal write-up, see the project design docs.

---

## Contact

- Security reports: **hearrelay-security@conex-cp.com**
- General contact: **hearrelay-support@conex-cp.com**

---

**日本語版:** [セキュリティ](/ja/security/)
