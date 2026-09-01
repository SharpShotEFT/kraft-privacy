# Kraft Workout Tracker — Privacy Policy

**Effective date:** 12 June 2026
**Data controller:** Kraft is operated by Odin Skjærvik, Norway
**Contact:** support@kraftlift.com

Kraft is built local-first: local workout tracking works without an account, while Google sign-in is required for paid-upgrade verification and Pro cloud features. This policy explains exactly what data Kraft handles, what is optional, and what we never do.

## The short version

- Your workouts are stored **on your device**. By default, nothing is uploaded anywhere.
- Kraft shows **no ads**, contains **no third-party advertising or tracking SDKs**, and **never sells your data**.
- Local workout tracking works without an account. Google sign-in is required to verify paid upgrades and to use Pro cloud features.
- Cloud features (account, online backup, multi-device sync) are **optional** and hosted in the **EU**.

## 1. Data stored on your device

Everything you record in Kraft — workouts, sets, exercises, routines, body measurements, personal records, settings, and your membership tier — is stored in a local database on your phone. This data does not leave your device unless you enable the optional cloud features described in section 3 or export it yourself (CSV/backup files you create are readable, unencrypted files saved where you choose and are under your control).

Rest-timer notifications are scheduled locally on your device. Kraft does not use push notifications and has no notification server.

When you choose to export a CSV or local backup, Android may pass that file to the app or destination you select in the system share sheet. Kraft does not control the recipient or what it does with a file you choose to share.

## 2. Purchases

Upgrades (Kraft Basic, Kraft Pro) are processed by **Google Play Billing**. Google processes your payment and does not provide us with payment details such as card numbers. To verify a paid upgrade, Kraft sends the Google Play purchase token to our authenticated verification service. Supabase stores the product, entitlement state, acknowledgement state, subscription expiry when applicable, verification timestamps, and one-way hashes of purchase tokens. These records are used only to verify and maintain your Kraft entitlement; the purchase token itself is not stored by Kraft. Google's handling of your payment data is described in [Google Play's Terms of Service](https://play.google.com/about/play-terms/) and [Google's Privacy Policy](https://policies.google.com/privacy).

## 3. Account, online backup and sync (optional cloud features)

If you sign in to Kraft (optional for local-only use, but required for paid-upgrade verification and Pro cloud features), the following applies:

- **Account data.** Your e-mail address, internal user ID, and the basic Google profile fields made available during Google sign-in (such as display name and profile-image reference, where provided). This is used solely to operate your account and verify purchases.
- **Online backup.** Backup files are **encrypted on your device before upload** and stored in the EU. The encryption key is never stored on our servers, and we have no mechanism to decrypt your stored backups in normal operation. Because signing in necessarily passes your credentials to our authentication service, this is strong application-level encryption rather than a formal zero-knowledge guarantee.
- **Multi-device sync.** If you enable sync, your training data (the same records described in section 1) is stored in our EU database so your devices can stay in step. Sync data is encrypted in transit and at rest and is isolated per account through database-level access rules; unlike backups, it is not end-to-end encrypted, because the server must read rows to merge changes between devices.
- **Hosting.** Cloud features run on **Supabase** (project hosted in Stockholm, Sweden, EU), acting as our data processor under a GDPR Data Processing Addendum. Supabase runs on infrastructure sub-processors (AWS, Stockholm region) under equivalent data-protection obligations; any support access from outside the EEA is covered by Standard Contractual Clauses in the processor agreement.
  - **Server logs.** When you use cloud features, our servers record short-lived technical logs, including your IP address (which may indicate approximate location), for security and abuse prevention; these are deleted on a rolling schedule.

Enabling backup or sync is an explicit choice you make in the app. To the extent your body measurements and training records reveal information about your health, we process them in the cloud only with your explicit consent (Art. 9(2)(a) GDPR), which you give when you enable backup or sync and can withdraw at any time by disabling those features.

## 4. What we never do

- No advertising, no ad SDKs, no behavioural tracking, no analytics SDKs.
- No sale of personal data, ever.
- No sharing of your data with third parties beyond the processors named in this policy (Google Play for purchases, Supabase for cloud hosting), except when you explicitly choose to share an exported CSV or backup file through Android's share sheet. Those selected recipients process the file under their own policies. Google Play and Supabase process data only on our instructions or as independent controller for payments.

## 5. Legal bases (GDPR)

Our processing of personal data is based on the following legal bases under the GDPR:

| Processing | Legal basis |
|---|---|
| Operating optional account, backup and sync | Performance of a contract (Art. 6(1)(b)); explicit consent (Art. 9(2)(a)) to the extent the data reveals health information |
| Processing purchases via Google Play | Performance of a contract (Art. 6(1)(b)) |
| Security/server logs for cloud features | Legitimate interest (Art. 6(1)(f)) — keeping the service secure |

## 6. Retention and deletion

- **On-device data** is yours: delete it in the app ("Clear all data") or by uninstalling.
- **Cloud data** (account, purchase-entitlement metadata, backups, and sync rows) is kept while your account exists and deleted when you delete your account. Residual copies may persist for a limited period in our hosting provider's encrypted database backups and expire automatically on its rolling retention schedule.
- **Server logs** are deleted on a short rolling schedule.

## 7. Delete your account and data
{: #delete-your-account-and-data}

- **In the app:** Settings → Account → **Delete account**. This permanently removes your account data, sync rows and stored backups from our systems.
- **By e-mail:** send a deletion request to **support@kraftlift.com** from any address — you do not need the app installed. We will delete the data associated with your account and confirm.
- **On-device data** can be deleted anytime via Settings → "Clear all data", or by uninstalling the app.

## 8. Your rights

Under the GDPR you have the right to: access your personal data and obtain a copy of it; rectification of inaccurate data; erasure; restriction of processing; data portability — receiving the data you provided in a structured, commonly used, machine-readable format (the in-app export covers your training data); and to withdraw any consent at any time, without affecting the lawfulness of processing carried out before withdrawal.

**Right to object.** Where we process data based on legitimate interest (security logs, section 3), you have the right to object at any time on grounds relating to your particular situation (Art. 21 GDPR) by contacting us at the address above.

To exercise any of these rights, contact support@kraftlift.com. You also have the right to complain to a supervisory authority — in Norway, **Datatilsynet** (www.datatilsynet.no).

## 9. Children

Kraft is not directed at children. We do not knowingly process personal data of children below the age required to consent to information society services in their country (13 in Norway; between 13 and 16 elsewhere in the EEA). If you believe a child below that age has created an account, contact us and we will delete the data.

## 10. Changes to this policy

If this policy changes, the new version will be published at this address with an updated effective date. Material changes to how optional cloud features process data will be announced in the app.
