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
- **We do not access your device calendar** — schedules are stored only inside the app.
- Most data **never leaves your device**. Only some optional features (Pro briefing, weather) communicate with external services (see Section 3).
- **We do not use advertising.**

## 2. Stored Only on Your Device (Never Transmitted)

The following is stored only in local storage (`shared_preferences`) and local files on your device, and is not sent to any server.

| Item | Content | Notes |
| --- | --- | --- |
| Alarm settings | Time, repeat, label, sound, vibration, snooze | |
| Barcode lock | **Only a SHA-256 hash is stored — never the raw barcode** | Raw values and hashes are never logged |
| Barcode hint photo | Reference image taken at registration | Local file; deleted on re-registration |
| Voice lock sample | Recording of the dismissal phrase | Stored locally; can be deleted |
| App schedules (calendar) | Title, time | Not synced with the device calendar |
| Emergency PIN | Last-resort method to dismiss a locked alarm | Stored locally |

## 3. Information Sent to External Services

The following is transmitted **only when you use the relevant feature**.

| Feature | Data sent | Recipient | Personal data included |
| --- | --- | --- | --- |
| Weather lookup | The **city name / coordinates** you entered | Open-Meteo | No location permission or account data |
| AI news briefing (Pro) | Only the **topics** you selected | Company proxy → OpenAI | **No schedules or personal data** |
| Speech read-aloud (Pro) | The **text** to be read (opening, weather, schedule, news summary) | Company proxy → OpenAI (speech synthesis) | **If schedule read-aloud is enabled, schedule titles may be included in that text** |
| Subscription payment (when offered) | Store payment and an **anonymous subscription identifier** | Apple/Google, payment provider (RevenueCat) | The app does not directly store payment or receipt data |

- **API keys are not included in the app**; they are held by the Company's server proxy.
- All external communication uses **HTTPS** only.
- If you do not want schedule titles to be sent, **turn off schedule read-aloud** in the briefing settings.

## 4. Permissions

| Permission | Purpose | When requested |
| --- | --- | --- |
| Notifications | Showing alarms and reminders | When you use alarms |
| Camera | Scanning the barcode lock | When you use the barcode lock |
| Microphone / speech recognition | Recording and matching the voice lock | When you use the voice lock |
| Location | **Not requested** | — |
| Device calendar | **Not requested** | — |

Permissions are not requested all at once on first launch; they are requested **only when you enter the relevant feature**. If you deny a permission, the remaining features continue to work.

## 5. Retention and Deletion

- The information above is deleted from your device when you **uninstall the app** or run **Settings → Delete all data (reset)** in the app.
- The Service does not provide cloud backup (local only), so barcodes, PINs and similar settings must be re-registered when you change or reinstall on a device.
- Requests sent to external services are handled under those services' own policies. The Company may cache **non-personal** request results for a limited period for cost and quality reasons.

## 6. Logging and Security

- Raw barcodes and their hashes, spoken text, schedule contents, tokens, payment information, and full request/response bodies are **never written to logs.**
- Sensitive values are redacted in logs.
- The Company applies reasonable technical and administrative safeguards to protect personal information.

## 7. Your Rights

You can delete or reset stored data at any time through the app's settings. For other privacy-related requests, please contact us at the address below.

## 8. Children's Privacy

The Service is **not directed at children under the age of 14** and does not knowingly collect their personal information. If we learn that a child under 14 has provided personal information without the consent of a legal guardian, the Company will delete such information without delay. The Service does not require an account or sign-in, and most data is stored only on the device.

## 9. Third-Party Links

This policy does not apply to the privacy practices of third parties used by the Service (Open-Meteo, OpenAI, Apple/Google, RevenueCat, etc.). Please review each service's own policy.

## 10. Changes to This Policy

This policy may be amended in line with changes in law or the Service. Amendments will be announced with their effective date and substance within the Service or through the app stores.

## 11. Contact

Privacy inquiries: InnoCode · innocode.core@gmail.com

---

*Last updated: 2026-07-28 · This policy applies together with the [Terms of Use](terms.html).*
