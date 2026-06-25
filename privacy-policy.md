# Privacy Policy — Nishkam App

**Effective Date:** June 11, 2025
**Last Updated:** June 24, 2026
**App Package:** `com.nishkam.app`
**Developer:** Nishkam App (theaighth@gmail.com)

---

## 1. Introduction

Welcome to **Nishkam** ("we," "our," or "us"). This Privacy Policy explains how we collect, use, disclose, and safeguard your information when you use our Android mobile application ("App"). Please read this policy carefully. If you disagree with its terms, please discontinue use of the App immediately.

We are committed to protecting your privacy. Nishkam is built on an **offline-first, privacy-by-design** architecture — meaning we deliberately avoid collecting personal data unless strictly necessary for the App to function.

---

## 2. Applicability

This Privacy Policy applies to:
- All users of the Nishkam Android application
- All versions of the App available on the Google Play Store

It does **not** apply to third-party websites, services, or applications that may be linked to or from the App, which have their own privacy policies.

---

## 3. Information We Collect

### 3.1 Information We Do NOT Collect

Nishkam does **not** collect, transmit, store on external servers, or share any of the following:

| Data Type | Collected? |
|-----------|------------|
| Location or GPS data | ✗ No |
| Device identifiers (IMEI, Android ID, advertising ID) | ✗ No |
| Contacts, calendar, or media access | ✗ No |
| Usage analytics or behavioral tracking | ✗ No |
| Crash reports sent to external servers | ✗ No |
| Financial information of any kind | ✗ No |
| Biometric data | ✗ No |
| Voice, audio, or camera data | ✗ No |
| Browser history or search queries | ✗ No |

We do not use advertising SDKs, analytics SDKs, or tracking SDKs of any kind.

### 3.2 Information Collected When You Sign In With Google

Nishkam requires you to sign in with your Google account to use the App. When you sign in:
- We use Google's official `google_sign_in` library to authenticate you directly with Google. **We do not use Firebase Authentication or any other intermediary — your credentials are handled entirely by Google's own sign-in flow.**
- We request only the `email` OAuth scope, solely to complete the sign-in handshake with Google.
- We **store only your Google account's display name** locally on your device, to personalize greetings and the shareable verse poster. **Your email address itself is never stored by the App, before or after sign-in.**
- Google's handling of your account data during this process is governed by [Google's own Privacy Policy](https://policies.google.com/privacy).
- You can sign out at any time from Settings; doing so returns you to the sign-in screen and clears your locally stored display name.

### 3.3 Information Stored Locally on Your Device

Beyond your Google account sign-in above, Nishkam stores the following data **exclusively on your device** using Android's local app-private storage (`SharedPreferences`). This data never leaves your device:

| Data | Purpose |
|------|---------|
| Display name (from Google sign-in) | Personalizes greetings, the verse poster, and share card |
| Date of birth (optional, user-provided) | Enables age-appropriate contextual features on the Student path |
| Chosen guidance path (Student / Professional / Grihastha) | Customizes verse takeaways and reflections per path |
| Chosen display language (English / Hindi / Gujarati) | Displays verse content and app text in your preferred language |
| Reading progress (which verses are read, current verse) | Tracks your journey through all 701 verses |
| Bookmarked verses | Stores your saved verse library |
| Notification time preference | Schedules your daily verse reminder |
| Login state | Determines whether onboarding has been completed |

**None of this data is transmitted to us, our servers, or any third party.**

### 3.4 Encrypted App Content

The Bhagavad Gita verse content bundled within the App is stored in an encrypted format (`assets/data/gita.enc`) using AES-256 encryption. This is a content-protection measure to protect our intellectual property — it is not a mechanism to collect or access your data.

---

## 4. How We Use the Information

We do not use any information for profiling, advertising, or any commercial purpose. The locally stored preferences listed in Section 3.3 are used solely to:

- Display your progress and greet you by name within the App
- Deliver your daily verse reminder notification at your preferred time
- Customize the verse takeaway (Student, Professional, or Grihastha perspective) in your chosen language
- Pre-fill your name in the downloadable verse poster

---

## 5. Sharing of Information

We do **not** sell, trade, rent, or otherwise transfer any information about you to any third party.

### 5.1 User-Initiated Sharing

The App includes a feature to export a verse as an image ("Liquid Glass Poster") and share it via Android's system share sheet. When you use this feature:

- The image is generated entirely on your device and written only to the App's private, sandboxed cache directory — no separate storage permission is needed or requested.
- The image is then handed to Android's built-in share mechanism — you choose where to send it (WhatsApp, Instagram, email, etc.).
- We do not receive, intercept, or log any information about what you share or where you share it.

### 5.2 No Third-Party Tracking SDKs

Nishkam does not embed any third-party SDKs that independently collect or transmit data, including:
- No Google Analytics / Firebase Analytics
- No Facebook SDK
- No Crashlytics or Sentry
- No advertising networks (AdMob, etc.)

### 5.3 Google Sign-In

As described in Section 3.2, Google Sign-In is implemented using Google's official `google_sign_in` library, which communicates directly with Google's authentication servers (the only network communication this App performs). No Firebase product is used for this feature.

---

## 6. Permissions Requested

| Android Permission | Reason |
|--------------------|--------|
| `POST_NOTIFICATIONS` | To deliver your opted-in daily verse reminder notification |
| `RECEIVE_BOOT_COMPLETED` | To re-register your notification alarm after device restart |
| `INTERNET` | Required for the Google Sign-In flow, to communicate with Google's servers |
| `VIBRATE` | Used for tactile feedback on taps and selections, and by the notification channel |

We do **not** request access to contacts, camera, microphone, location, phone state, storage, or any other sensitive permission.

---

## 7. Data Retention and Deletion

All data described in Section 3.3 is stored exclusively on your device. You can delete it at any time by:

1. **Clearing app data:** Go to Android Settings → Apps → Nishkam → Storage → Clear Data.
2. **Uninstalling the App:** All local data is permanently and irreversibly deleted when you uninstall.
3. **Signing out:** Signing out from Settings clears your locally stored name and returns you to the sign-in screen.

We have no ability to recover this data on your behalf, as we never held it.

---

## 8. Children's Privacy (COPPA Compliance)

Nishkam's content is appropriate for users of all ages, but a Google account is required to use the App. We do not separately collect or verify age — account eligibility is governed entirely by Google's own age requirements and parental-supervision tools (such as Google Family Link) for account holders. We do not knowingly collect personal information beyond what is described in Section 3.2 from any user, consistent with the Children's Online Privacy Protection Act (COPPA).

If you believe a child has used the App in a manner inconsistent with COPPA, please contact us at the address below.

---

## 9. International Users and GDPR

Nishkam minimizes personal data processing wherever possible. For users in the European Economic Area (EEA), the United Kingdom, and other jurisdictions with data protection laws:

- **Legal basis for processing:** Signing in with Google is necessary to provide the App's core functionality (performance of a contract at your request). For all other locally stored preferences, the basis is the same — performance of the App's core functionality you have requested.
- **Data subject rights (access, rectification, erasure, portability):** All data we hold resides on your own device; you have full, direct control of it via Section 7.
- **Data Protection Officer (DPO):** Not required given the limited scope of data processed.

---

## 10. Security

We employ the following technical safeguards:

- All app content is AES-256 encrypted at rest within the App bundle.
- Local preferences are stored in Android's private app data directory, inaccessible to other apps on non-rooted devices.
- The App performs a device integrity check in production builds to detect compromised (rooted) environments where local data could be at greater risk.
- We do not operate any servers or databases that hold your personal data.

Your data's security on the device depends on your device's security measures. We strongly recommend using a strong screen lock (PIN, pattern, or biometric).

---

## 11. Links to Third-Party Services

The App may contain attribution links or references to third-party websites (e.g., our GitHub repository, Play Store listing) and uses Google Sign-In as described above. We are not responsible for the privacy practices or content of those third-party services. We encourage you to review their privacy policies before engaging with them.

---

## 12. Changes to This Privacy Policy

We may update this Privacy Policy periodically. When we do:

- The "Last Updated" date at the top of this document will be revised.
- If the changes are material, we will include a notice within the App on next launch.
- Continued use of the App after the revised policy takes effect constitutes your acceptance of the new policy.

We recommend reviewing this policy whenever you update the App.

---

## 13. Contact Us

If you have questions, concerns, or requests regarding this Privacy Policy, please contact us:

**Email:** theaighth@gmail.com
**GitHub Issues:** [github.com/itsaakashn/NishkamApp/issues](https://github.com/itsaakashn/NishkamApp/issues)

We aim to respond to all privacy-related inquiries within **30 days**.

---

*This Privacy Policy was written to be clear, complete, and free of legal jargon. If any section is unclear, please reach out — we're happy to explain.*
