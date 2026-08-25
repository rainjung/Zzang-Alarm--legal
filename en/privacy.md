---
layout: default
title: Privacy Policy
lang: en
---

# Privacy Policy

This policy explains how Zzang Alarm (the "Service") handles your personal information. The Service is built on the principles of **minimal collection** and **on-device (local-first) storage**.

---

## 1. Summary of Principles

- **No account, no sign-in** — the Service does not require registration.
- **We do not request location (GPS) permission** — weather is looked up by a city name you enter yourself.
- **We read your device calendars only if you turn it on** — an optional feature that shows events from the calendars you pick (Google, Samsung, …) alongside your app schedule. We **never add, change or delete** them, and what we read **never leaves your device**. The rest of the app works whether or not you allow it.
- **The Company operates no server.** There is no Company-side server that the app sends your data to.
- The only request the app itself sends out is **the weather lookup** (see Section 3).
- **Voice lock records and stores no audio.** Turning what you say into text is done by your **device's operating system**, and depending on the device and its settings **the OS may send that audio to Apple or Google for processing** (see Section 3).
- **We send no data to AI services.** Briefing read-aloud is handled by your device's own speech synthesis (TTS) and uses no network.
- **We do not use advertising.**

## 2. Stored Only on Your Device (Never Transmitted)

The following is stored only in local storage (`shared_preferences`) and local files on your device, and is not sent to any server.

| Item | Content | Notes |
| --- | --- | --- |
| Alarm settings | Time, repeat, label, sound, vibration, snooze | |
| Barcode lock | **Only a SHA-256 hash is stored — never the raw barcode** | Raw values and hashes are never logged |
| Barcode hint photo | Reference image taken at registration | Local file; deleted on re-registration |
| Voice lock phrase | The sentence you say to dismiss, **as text** | Stored on device only; **no audio is recorded or saved** |
| App schedules (calendar) | Title, time, location, memo, reminder settings | **Never exported** to the device calendar |
| Device calendar selection | Only the **identifiers** of the calendars you chose | Event contents are not stored — they are read each time you look |
| Emergency PIN | Last-resort method to dismiss a locked alarm | **Only a salted SHA-256 hash is stored — never the raw PIN** |
| Read-aloud settings | Voice, speed, pitch | Settings for the device TTS engine |
| Weather response cache | The most recent forecast (up to 3 hours) | Cached on the device; cleared when you change city |

## 3. Information Sent to External Services

The following is transmitted **only when you use the relevant feature**.

| Feature | Data sent | Recipient | Personal data included |
| --- | --- | --- | --- |
| Weather lookup | The **coordinates** of the city you selected | MET Norway (Norwegian Meteorological Institute) | No location permission or account data |
| Subscription payment (when offered) | Store payment and an **anonymous subscription identifier** | Apple/Google, payment provider (RevenueCat) | The app does not directly store payment or receipt data |

- The **weather lookup above is the only external API the app calls directly**. Payments are handled by each store's SDK.
- All external communication uses **HTTPS** only.

**Speech recognition performed by your operating system**

When you dismiss an alarm by voice, turning what you say into text is performed by your **device's operating system** (Apple speech recognition / Google speech recognition), not by the app. Depending on the device, language and settings, this may happen **on the device, or the OS may send the audio to that provider's servers.** Such transmission is carried out by the operating system and is governed by Apple's and Google's privacy policies; **we never receive the audio or the recognised text.** The app does not record audio or save it to a file — the recognised text is compared with your registered phrase and then discarded.

### What Is Not Sent

- **Briefing read-aloud (Pro)** — the narration text includes the date, weekday and weather along with **your schedule titles**. That text is **processed entirely by the speech synthesis (TTS) engine on your device and is never transmitted.** It works with no network connection.
- **Device calendar events** — titles, times and locations from the calendars you picked are shown in the app calendar and read aloud in your briefing. That content is **used only for on-screen display and on-device speech synthesis, and is never transmitted.** The app **only reads** the device calendar and never adds, changes or deletes anything (on Android it requests `READ_CALENDAR` only and does not even declare write access).
- **AI services** — the Service sends data to no AI provider, and the app contains no AI provider API key.
- **Company servers** — the Company operates no server that receives user data.
- **AI news briefing** — removed from the product on 2026-08-17. No news-related data is collected or transmitted.

> **Change history** — versions before 2026-08-23 sent read-aloud text through a Company server proxy to an external speech synthesis service (OpenAI). Narration has since moved on-device, so that transmission no longer occurs, and the server proxy has been retired.

## 4. Permissions

| Permission | Purpose | When requested |
| --- | --- | --- |
| Notifications | Showing alarms and schedule reminders | When you save an alarm, or turn on a schedule reminder |
| Camera | Scanning the barcode lock | When you use the barcode lock |
| Microphone / speech recognition | Dismissing by voice — what you say is turned into text and matched against your phrase | When you dismiss an alarm by voice |
| Exact alarms (Android) | Ringing the alarm at the exact time | When you save an alarm |
| Battery optimisation exemption (Android) | Preventing power-saving from delaying or dropping alarms | Only when you choose it from the in-app notice |
| Location | **Not requested** | — |
| Device calendar | **Read only** (optional) — shows and reads aloud events from the calendars you pick | When you turn on "Device calendars" |

These permissions exist to use device features; information obtained through them is not transmitted externally.

Permissions are not requested all at once on first launch; they are requested **only when you enter the relevant feature**. If you deny a permission, the remaining features continue to work.

## 5. Retention and Deletion

- The information above is deleted from your device when you **uninstall the app** or run **Settings → Delete all data (reset)** in the app.
- The Service does not provide cloud backup (local only), so barcodes, PINs and similar settings must be re-registered when you change or reinstall on a device.
- Requests sent to external services (weather, store payments) are handled under those services' own policies.
- Weather forecast responses are cached **on your device only**, for up to 3 hours (cleared immediately when you change city). They are not stored by the Company.

## 6. Logging and Security

- Raw barcodes and their hashes, spoken text, schedule contents, tokens, payment information, and full request/response bodies are **never written to logs.**
- Sensitive values are redacted in logs.
- The Company applies reasonable technical and administrative safeguards to protect personal information.

## 7. Your Rights

You can delete or reset stored data at any time through the app's settings. For other privacy-related requests, please contact us at the address below.

## 8. Children's Privacy

The Service is **not directed at children under the age of 14** and does not knowingly collect their personal information. If we learn that a child under 14 has provided personal information without the consent of a legal guardian, the Company will delete such information without delay. The Service does not require an account or sign-in, and most data is stored only on the device.

## 9. Third-Party Links

This policy does not apply to the privacy practices of third parties used by the Service (MET Norway, Apple/Google, RevenueCat). **Events held in your device calendars are managed by their providers (Google, Samsung, …); the Service only reads and displays them.** Please review each service's own policy.

## 10. Changes to This Policy

This policy may be amended in line with changes in law or the Service. Amendments will be announced with their effective date and substance within the Service or through the app stores.

## 11. Contact

Privacy inquiries: InnoCode · innocode.core@gmail.com

---

*Last updated: 2026-08-26 · This policy applies together with the [Terms of Use](terms.html).*
