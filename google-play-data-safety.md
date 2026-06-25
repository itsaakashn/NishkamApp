# Google Play Data Safety — Nishkam App

This document provides the answers for Google Play Console's **Data Safety** form, required for all apps published on the Play Store. It is published here for transparency so that users can independently verify the claims made in our Play Store listing.

**Last Updated:** June 22, 2026

---

## Summary

| Question | Answer |
|----------|--------|
| Does your app collect or share any of the required user data types? | **Yes — limited to Name and Email address, both tied to the mandatory Google Sign-In required to use the app** |
| Is all data collected encrypted in transit? | **Yes** — the Google Sign-In flow is encrypted via Google's own HTTPS/TLS infrastructure |
| Does your app provide a way for users to request that their data is deleted? | **Yes** — by signing out, via Android Settings → Apps → Nishkam → Clear Data, or by uninstalling |

> Nishkam requires Google Sign-In to use the app — there is no guest/anonymous mode. The two items below are collected for every user as a result.

---

## Data Types — What We Collect, Share, and Why

### Data Collection

> "Collected" means data is transmitted off the device to an external party (here: Google's own sign-in service, not a server we operate).

| Category | Data Type | Collected? | Shared? | Required / Optional | Purpose |
|----------|-----------|-----------|---------|-------------------|---------|
| Personal info | Name | ✓ Collected (from Google Sign-In) | ✗ Not shared | Required — Google Sign-In is mandatory to use the App | App functionality / personalization |
| Personal info | Email address | ✓ Collected (from Google Sign-In, used transiently for authentication only — never stored by the App) | ✗ Not shared | Required — Google Sign-In is mandatory to use the App | Account management (authentication) |
| Personal info | Phone number | ✗ Not collected | ✗ | — | — |
| Personal info | Race and ethnicity | ✗ Not collected | ✗ | — | — |
| Personal info | Religious or political beliefs | ✗ Not collected | ✗ | — | — |
| Personal info | Sexual orientation | ✗ Not collected | ✗ | — | — |
| Financial info | Credit cards / bank accounts | ✗ Not collected | ✗ | — | — |
| Location | Precise location | ✗ Not collected | ✗ | — | — |
| Location | Approximate location | ✗ Not collected | ✗ | — | — |
| Web browsing | Web history | ✗ Not collected | ✗ | — | — |
| App activity | App interactions | ✗ Not collected | ✗ | — | — |
| App activity | In-app search history | ✗ Not collected | ✗ | — | — |
| App activity | Installed apps | ✗ Not collected | ✗ | — | — |
| App activity | Other user-generated content | ✗ Not collected | ✗ | — | — |
| Device IDs | Device or other IDs | ✗ Not collected | ✗ | — | — |
| Photos / videos | Photos | ✗ Not collected | ✗ | — | — |
| Audio | Voice / sound recordings | ✗ Not collected | ✗ | — | — |
| Health & fitness | Health info | ✗ Not collected | ✗ | — | — |
| Messages | Emails / SMS | ✗ Not collected | ✗ | — | — |
| Contacts | Contacts | ✗ Not collected | ✗ | — | — |
| Calendar | Calendar events | ✗ Not collected | ✗ | — | — |

**Note on "collected" vs. our servers:** We do not operate any backend server. The Name and Email address above are exchanged directly between the user's device and Google's own authentication service during the mandatory Google Sign-In flow — Nishkam never receives, stores, or has server-side access to this data. We store only the display name locally on-device after sign-in completes; the email address itself is discarded immediately and never persisted anywhere, by us or in local storage.

### Data Stored Locally on Device (not transmitted to us)

The following data is stored **only on the user's device** and never transmitted to any server we operate:

| Data | Storage | User Can Delete? |
|------|---------|----------------|
| Display name (from Google sign-in) | Android SharedPreferences | Yes — Sign out / Clear Data / Uninstall |
| Date of birth (optional) | Android SharedPreferences | Yes — Clear Data / Uninstall |
| Guidance path selection (Student / Professional / Grihastha) | Android SharedPreferences | Yes — Clear Data / Uninstall |
| Display language (English / Hindi / Gujarati) | Android SharedPreferences | Yes — Clear Data / Uninstall |
| Reading progress | Android SharedPreferences | Yes — Clear Data / Uninstall |
| Bookmarked verses | Android SharedPreferences | Yes — Clear Data / Uninstall |
| Notification time preference | Android SharedPreferences | Yes — Clear Data / Uninstall |

---

## Security Practices

| Play Store Question | Our Answer |
|--------------------|----|
| Does your app use encryption in transit? | **Yes** — the only network traffic (the mandatory Google Sign-In flow) runs over Google's own HTTPS/TLS-secured infrastructure |
| Does your app follow the Families Policy? | Yes — appropriate for all ages |

---

## Play Store Data Safety Form Answers (Verbatim)

Use these answers directly in the Play Console Data Safety section:

### Section: Data collection and security

**Does your app collect or share any of the required user data types?**
→ **Yes**

**Is all data collected encrypted in transit?**
→ **Yes**

**Do you provide a way for users to request that their data is deleted?**
→ **Yes**
→ *(Deletion method: Users can sign out to clear the locally stored Google display name, clear all app data via Android Settings → Apps → Nishkam → Storage → Clear Data, or uninstall the app to permanently delete all local data.)*

### Section: Data types

| Category | Item | Declare as |
|----------|------|-----------|
| Personal info | Name | **Collected**, not shared, **required**, purpose: App functionality |
| Personal info | Email address | **Collected**, not shared, **required**, purpose: Account management |
| All other categories (Location, Financial info, Health & fitness, Messages, Photos & videos, Audio, Files & docs, Calendar, Contacts, App activity, Web browsing, App info & performance, Device IDs) | every item | **No data collected** |

---

## Contact for Data Safety Questions

**Email:** theaighth@gmail.com

---

*This document reflects the current state of the Nishkam App and will be updated whenever data practices change (e.g. if Google Sign-In is removed or extended). The Play Store Data Safety declaration must be updated to match whenever this document changes.*
