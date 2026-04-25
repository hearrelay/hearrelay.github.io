---
title: Support — HearRelay
lang: en
---

# Support

**Document version: v3.2026-04-26**

Thanks for using **HearRelay**. This page gathers troubleshooting tips, important notices about lawful use, and how to get in touch.

---

## Important notices

### Recording and monitoring laws differ by place

Recording and live-monitoring laws vary by country, state, province, and place of use. Some places require consent from **all** parties before recording. Workplace, school, rental, medical, eldercare, childcare, and public-space monitoring may require special notice, written consent, or permission. **Do not record conversations or private spaces unless you are legally allowed to do so.** When in doubt, do not record.

You are responsible for confirming that any recording or live-monitoring you perform with HearRelay complies with all applicable law. See [Terms of Use §3](/en/terms/) for the prohibited-use list.

### HearRelay is not a safety, medical, or emergency device

HearRelay is a consumer utility for convenience monitoring. It is **not** a medical device, an emergency device, a security alarm, a childcare safety device, an eldercare safety device, a life-support device, or any equipment certified for safety-critical use. **Never use HearRelay as the sole means of supervision or emergency detection.** Always combine it with responsible direct supervision and any safety equipment certified for the purpose.

### Why HearRelay does not work over the internet

HearRelay deliberately requires both devices to be **signed in to the same Apple ID** *and* **connected to the same Wi-Fi / local network**. There is no internet-relay option, no remote-monitoring mode, and no "cloud" path. This is a security and privacy choice, not a missing feature:

- It prevents covert remote surveillance — a stolen or borrowed iPhone cannot stream audio out of someone's home.
- It keeps audio off CONEX servers (we operate none) and off the public internet.
- It limits the impact of an Apple ID compromise to devices already paired to that Apple ID.

If you need monitoring across networks, HearRelay is not the right tool — use a product certified for that purpose, with the appropriate parental, employment, or other legal notice.

---

## Quick help

### "No devices found" when I try to pair

Both devices need to:

1. Be signed in to **the same Apple ID**
2. Be connected to **the same Wi-Fi network** (same subnet)
3. Have **iCloud** turned on in iOS Settings
4. Have granted HearRelay the **Microphone** and **Local Network** permissions

If you still don't see the other device, tap the refresh button on the pair picker, or restart the App on both devices.

### The audio stutters or cuts out

- Move closer to your Wi-Fi router, or switch to a 5 GHz network
- Bluetooth headphones with poor reception may introduce dropouts — try wired or a different pair
- Heavy network traffic (large downloads, video calls) on the same Wi-Fi can affect real-time audio

### The sound from AirPods is strangely low quality in Standalone mode

HearRelay restricts the microphone to the **built-in mic** in Standalone mode to avoid forcing Bluetooth into a low-bandwidth mode (HFP). Use the built-in microphone for input and AirPods as output only. This is by design.

### Recording didn't stay

Recordings are automatically deleted **24 hours after creation** unless you tap **Preserve** on the recording. Once preserved, they stay until you delete them.

### HearRelay stopped recording when I locked the screen

HearRelay continues to capture and relay audio in the background while the screen is locked. If capture stops:

- Ensure **Background App Refresh** is allowed for HearRelay (iOS Settings → General → Background App Refresh)
- Ensure **Low Power Mode** is not aggressively suspending background tasks
- Some iOS versions suspend audio sessions when another audio app takes over — stop the other app

### The icon in Dynamic Island / Lock Screen disappeared

Live Activities have an OS-imposed maximum duration (around 8 hours). Once reached, the indicator may stop updating even though HearRelay keeps working. Re-open the App to refresh.

**Important:** Even if a Live Activity or Lock Screen widget stops updating due to OS limits, **background audio capture may continue while monitoring is active**. Use this only in lawful, disclosed monitoring situations. Do not place a device where it may capture people who have not received any legally required notice or consent. iOS may also show its system microphone / privacy indicators while audio capture is active.

---

## Purchases and subscriptions

### Is HearRelay a subscription?

**No.** HearRelay Full Access is a **Non-Consumable, one-time purchase** (a buy-out IAP). It is **not** an auto-renewing subscription. After the 14-day free trial, a single purchase unlocks the App for as long as you remain signed in to your Apple ID.

### Family Sharing

The unlock is enabled for **Family Sharing**, so members of your Family Sharing group can use HearRelay Full Access at no extra cost.

### How do I restore a previous purchase?

Open the App → tap the locked banner → **Restore Purchases**. Apple will check your Apple ID for the previous unlock and re-apply it.

### How do I get a refund?

Refund requests for App Store purchases must be submitted through Apple's standard refund process at <https://reportaproblem.apple.com>. Apple processes refunds under the App Store and Apple Media Services Terms. CONEX does not receive payment card numbers or billing details. Nothing in this paragraph limits any mandatory consumer rights you may have against CONEX under applicable law.

---

## Permissions checklist

| Permission | Required for | Setting path |
|---|---|---|
| Microphone | Any monitoring | Settings → HearRelay → Microphone |
| Local Network | Pair mode (sending / receiving to other devices) | Settings → HearRelay → Local Network |
| iCloud (signed in) | Pair mode (discover your other devices) | Settings → \[Your name\] → iCloud |
| Background App Refresh | Continued monitoring with screen off | Settings → General → Background App Refresh |

If Local Network or iCloud is not available, you can still use **Standalone** mode.

---

## Contact

- **Email:** hearrelay-support@conex-cp.com
- We aim to respond within a few business days. Please include your iOS version, device model, and a description of the steps you took.

For privacy questions, see the [Privacy Policy](/en/privacy/) or email **hearrelay-privacy@conex-cp.com**.
For security reports, see the [Security page](/en/security/) or email **hearrelay-security@conex-cp.com**.

---

**Translations are available in:** [日本語](/ja/support/) · [Français](/fr/support/) · [Español](/es/support/) · [Português (Brasil)](/pt-BR/support/) · [简体中文](/zh-Hans/support/)

Where this page is provided in any language other than English, the **English version controls** to the extent permitted by applicable law. This precedence rule does not limit any rights granted to you by mandatory consumer-protection, privacy, or data-protection laws of your country or region.
