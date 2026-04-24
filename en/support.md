---
title: Support — HearRelay
lang: en
---

# Support

Thanks for using **HearRelay**. This page gathers troubleshooting tips and how to get in touch.

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

**日本語版:** [サポート](/ja/support/)
