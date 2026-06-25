# Security Policy — Nishkam App

**Last Updated:** June 24, 2026

---

## Supported Versions

We maintain security support for the following versions:

| Version | Supported |
|---------|-----------|
| Latest release on Play Store | ✅ Active support |
| Previous major version | ⚠️ Critical fixes only |
| Older versions | ✗ Not supported — please update |

---

## Reporting a Vulnerability

We take security seriously. If you discover a security vulnerability in the Nishkam App, **please do not open a public GitHub issue.** Publicly disclosing a vulnerability before we have had a chance to fix it could put users at risk.

### How to Report

Please report security vulnerabilities via **private email**:

**Email:** theaighth@gmail.com
**Subject line:** `[SECURITY] <brief description>`

### What to Include

To help us triage and fix the issue as quickly as possible, please include:

1. **Type of vulnerability** (e.g., data exposure, insecure storage, code injection, unintended permission, etc.)
2. **Steps to reproduce** — clear, step-by-step instructions
3. **Impact assessment** — what could an attacker achieve? What user data (if any) is at risk?
4. **App version** affected (visible in Settings → About)
5. **Device and Android version** used during testing
6. **Any proof-of-concept code or screenshots** (attach to email, do not paste in public channels)

### What Happens Next

1. **Acknowledgement:** We will acknowledge receipt of your report within **72 hours**.
2. **Assessment:** We will evaluate the severity and impact within **7 days**.
3. **Fix timeline:** We aim to release a fix within **30 days** for critical vulnerabilities and **90 days** for lower-severity issues.
4. **Disclosure:** We will coordinate a public disclosure date with you once a fix is available and deployed.
5. **Credit:** With your permission, we will credit you in the release notes and/or our security hall of fame.

---

## Security Architecture

### Data at Rest

- All Bhagavad Gita verse content is encrypted using **AES-256** encryption before bundling in the App.
- User preferences (name, path, progress, bookmarks) are stored in Android's private app data directory (`SharedPreferences`), which is inaccessible to other apps on non-rooted devices.

### No External Data Transmission

- The App transmits **zero user data** to any external server.
- There are no network calls made by the App during normal operation.
- The App does not use analytics, advertising, or crash-reporting SDKs.

### Production Integrity Check

- In release builds, the App performs a **device integrity check** to detect rooted/compromised environments. On rooted devices, the App exits in release mode to protect locally stored user data from potential exploitation by other malicious apps.

### Permissions

- The App requests the minimum permissions necessary for its features. We do not request permissions not directly required by a specific user-facing feature.

---

## Known Limitations

| Limitation | Notes |
|-----------|-------|
| Local data unprotected on rooted devices | The integrity check mitigates this in release mode |
| No remote wipe | We cannot delete local user data remotely since we never held it |

---

## Responsible Disclosure Policy

We follow a **coordinated disclosure** model:
- We ask researchers to give us a reasonable time (30–90 days depending on severity) to fix the issue before any public disclosure.
- We will not take legal action against researchers who follow this policy and act in good faith.
- We request that researchers do not access or modify user data beyond what is necessary to demonstrate the vulnerability.
- We request that researchers do not perform denial-of-service attacks or degrade service for other users.

---

## Contact

**Security reports:** theaighth@gmail.com (use subject line `[SECURITY]`)
**General issues:** [github.com/itsaakashn/NishkamApp/issues](https://github.com/itsaakashn/NishkamApp/issues)

Thank you for helping keep Nishkam users safe.
