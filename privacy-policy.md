# Privacy Policy for Clenvo

**Effective date:** [EFFECTIVE_DATE]

[DEVELOPER_NAME] ("we," "us," or "our") operates the Clenvo mobile application (the "App"). This Privacy Policy explains what information the App accesses, how it is used, and your choices — in plain language first, with the full detail below.

**This policy must be published at a public URL and that URL entered into Google Play Console before submission.** Everything in brackets (e.g. `[EFFECTIVE_DATE]`) is a placeholder to fill in before publishing.

## Summary

- Clenvo scans your photo library **entirely on your device**. Photos, thumbnails, and file data are never uploaded to us or to any server we control — there is no backend for photo data at all.
- We do not require an account, sign-in, or any personal information to use the App.
- The App shows ads (via Google AdMob) and offers a one-time "Pro" purchase (via Google Play Billing). These third-party services process limited technical data as described below.
- You can uninstall the App at any time to stop all data processing described here.

## 1. Information We Access

### 1.1 Photo and media library access
With your permission, Clenvo reads metadata about the photos on your device — such as file size, dimensions, file hash, and modification date — to detect exact and near-duplicate images. This processing happens locally, using on-device comparison. **Your photo files and this metadata are never transmitted off your device, uploaded to a server, or shared with us.**

On Android, this uses the following system permissions:
- `READ_MEDIA_IMAGES` (Android 13+) — read access to images
- `READ_MEDIA_VISUAL_USER_SELECTED` (Android 14+) — supports the OS's "select photos" partial-access option
- `READ_EXTERNAL_STORAGE` (Android 12 and below) — read access to media on older OS versions

### 1.2 Deleting photos
When you confirm a cleanup, Clenvo asks Android to move the selected photos to your device's system Trash (or, on OS versions without a Trash, to delete them), using the standard Android media-deletion permission flow. Each deletion requires your explicit, in-the-moment confirmation via the Android system dialog.

### 1.3 Purchase information
If you buy Clenvo Pro, the purchase is processed entirely by Google Play Billing. We receive only a purchase confirmation (via Google Play) sufficient to unlock Pro features on your device — we do not receive or store your payment details (card number, billing address, etc.); those are handled directly by Google Play.

### 1.4 Advertising
Clenvo shows ads through Google AdMob in the free version of the App. AdMob may collect and process device and advertising identifiers (such as your Android Advertising ID), approximate location, and ad-interaction data, to serve and measure ads — potentially including personalized ads, subject to the consent choice described in Section 3. This data is collected and processed by Google, not by us directly. Purchasing Clenvo Pro removes all ads and this data collection.

## 2. Information We Do Not Collect

We do not collect, and the App does not require:
- Your name, email address, or other account/profile information
- Your photos or videos themselves, or any copy of them
- Precise location data
- Contacts, messages, or other app data outside the photo library scope described above

## 3. Third-Party Services

Clenvo uses the following third-party services, each governed by its own privacy policy:

- **Google AdMob** (ads) — [Google Privacy & Terms](https://policies.google.com/privacy)
- **Google User Messaging Platform (UMP)** — used to present a consent form (where legally required, e.g. under GDPR) before any ad-related data is collected, letting you choose whether to allow personalized ads
- **Google Play Billing** (in-app purchase processing) — [Google Play Terms](https://play.google.com/about/play-terms/)

Where the consent form is shown, your choice is stored on your device and can be changed by reinstalling the App or through your device's ad-settings, per Google's own controls.

## 4. Data Retention

Since photo data is never sent to us, we have nothing to retain or delete on our end. Locally, Clenvo keeps a small on-device database of scan results (photo metadata and grouping, not photo content) to show your scan history and avoid re-scanning unchanged photos; this is deleted automatically when you uninstall the App.

## 5. Children's Privacy

Clenvo is not directed at children under 13 (or the relevant minimum age in your jurisdiction), and we do not knowingly collect personal information from children. If you believe a child has provided us with personal information, contact us using the details below and we will address it.

## 6. Your Choices

- **Ad personalization:** where a consent form is shown, you can decline personalized ads.
- **Photo access:** you can grant, limit (partial-selection), or revoke photo access at any time in your device's Settings.
- **Uninstall:** removing the App stops all data processing described in this policy and deletes the App's local on-device data.

## 7. Security

Because photo data never leaves your device, its security is governed by your device's own operating system protections. Purchase and advertising data handled by Google are protected under Google's own security practices.

## 8. Changes to This Policy

We may update this Privacy Policy from time to time. Material changes will be reflected by an updated "Effective date" above, and, where required, notified through the App or the Play Store listing.

## 9. Contact Us

Questions about this Privacy Policy can be sent to: [SUPPORT_EMAIL]

---

## Before you publish this — checklist

1. Replace `[EFFECTIVE_DATE]`, `[DEVELOPER_NAME]`, and `[SUPPORT_EMAIL]` with real values.
2. Host this document at a public URL (your own website, or a static page such as GitHub Pages) — Play Console requires a live URL, not a file upload.
3. Enter that URL in Play Console → **Policy → App content → Privacy policy**.
4. This text assumes the AdMob **test** App ID is replaced with your real AdMob App ID before release (`apps/mobile/android/app/src/main/AndroidManifest.xml` currently has a `TODO` for this) — the policy's ad-data description applies to production AdMob, not the test SDK.
5. Play Console will separately ask you to complete a **Data Safety** form and, because the App requests photo/media access, a **Permissions declaration** (and possibly a short screen-recording) under the Photo and Video Permissions policy — this document supports those, but doesn't replace filling them out in Play Console.
