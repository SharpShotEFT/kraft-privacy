# Kraft Workout Tracker — Privacy Policy

**Effective date:** 12 June 2026
**Developer / data controller:** Odin Skjærvik, Norway
**Contact:** odinskjaervik@gmail.com

Kraft is built local-first: your training data lives on your phone, and the app works fully without an account. This policy explains exactly what data Kraft handles, what is optional, and what we never do.

## The short version

- Your workouts are stored **on your device**. By default, nothing is uploaded anywhere.
- Kraft shows **no ads**, contains **no third-party advertising or tracking SDKs**, and **never sells your data**.
- Cloud features (account, online backup, multi-device sync) are **optional** and hosted in the **EU**.
- Contributing pseudonymized training data to improve recommendations is a **separate, off-by-default opt-in**.

## 1. Data stored on your device

Everything you record in Kraft — workouts, sets, exercises, routines, body measurements, personal records, settings, and your membership tier — is stored in a local database on your phone. This data does not leave your device unless you enable the optional cloud features described in section 3 or export it yourself (CSV/backup files you create are saved where you choose and are under your control).

Rest-timer notifications are scheduled locally on your device. Kraft does not use push notifications and has no notification server.

## 2. Purchases

Upgrades (Kraft Basic, Kraft Pro) are processed by **Google Play Billing**. Google processes your payment and shares no payment details (such as card numbers) with us. Kraft checks your purchases with Google Play to unlock the matching features; your purchase state is stored locally on the device. Google's handling of your payment data is described in [Google Play's Terms of Service](https://play.google.com/about/play-terms/) and [Google's Privacy Policy](https://policies.google.com/privacy).

## 3. Optional: account, online backup and sync (Kraft Pro)

If you create a Kraft account (optional, required only for Pro cloud features), the following applies:

- **Account data.** Your e-mail address (or, if you choose Google sign-in, the e-mail and basic profile reference Google provides) and an internal user ID. This is used solely to operate your account.
- **Online backup.** Backup files are **encrypted on your device before upload** and stored in the EU. The encryption key is never stored on our servers, and we have no mechanism to decrypt your stored backups in normal operation. Because signing in necessarily passes your credentials to our authentication service, this is strong application-level encryption rather than a formal zero-knowledge guarantee.
- **Multi-device sync.** If you enable sync, your training data (the same records described in section 1) is stored in our EU database so your devices can stay in step. Sync data is encrypted in transit and at rest and is isolated per account through database-level access rules; unlike backups, it is not end-to-end encrypted, because the server must read rows to merge changes between devices.
- **Hosting.** Cloud features run on **Supabase** (project hosted in Stockholm, Sweden, EU), acting as our data processor under a GDPR Data Processing Addendum. Supabase runs on infrastructure sub-processors (AWS, Stockholm region) under equivalent data-protection obligations; any support access from outside the EEA is covered by Standard Contractual Clauses in the processor agreement.
- **Server logs.** When you use cloud features, our servers record short-lived technical logs (including your IP address) for security and abuse prevention; these are deleted on a rolling schedule.

Enabling backup or sync is an explicit choice you make in the app. To the extent your body measurements and training records reveal information about your health, we process them in the cloud only with your explicit consent (Art. 9(2)(a) GDPR), which you give when you enable backup/sync or data contribution and can withdraw at any time by disabling those features.

## 4. Optional: pseudonymized data contribution (off by default)

Kraft has a separate setting — **"Contribute training data to improve recommendations"** — which is **off by default**. If you turn it on:

- Your training records are associated with a random pseudonymous ID, not your name, e-mail or account ID. Contributed records are pseudonymized — but until they are aggregated they remain personal data under the GDPR, which is why this processing is based on your consent.
- The data is used only to compute aggregate statistics and train recommendation features inside Kraft (for example "lifters with a similar bench press typically row this weight").
- Published statistics are aggregated and k-anonymous: no statistic is shown unless it is based on a sufficiently large group of contributors, and aggregates are no longer personal data.
- It is never sold, never shared with third parties, and never used for advertising.

You can turn the toggle off at any time. When you opt out or delete your account, your contributed records are deleted from the contribution dataset and excluded from all future statistics and training runs. Aggregate statistics already published are anonymous and cannot be traced back to you.

## 5. What we never do

- No advertising, no ad SDKs, no behavioural tracking, no analytics SDKs.
- No sale of personal data, ever.
- No sharing of your data with third parties beyond the processors named in this policy (Google Play for purchases, Supabase for cloud hosting), each of which processes data only on our instructions or as independent controller for payments.

## 6. Legal bases (GDPR)

Our processing of personal data is based on the following legal bases under the GDPR:

| Processing | Legal basis |
|---|---|
| Operating optional account, backup and sync | Performance of a contract (Art. 6(1)(b)); explicit consent (Art. 9(2)(a)) to the extent the data reveals health information |
| Processing purchases via Google Play | Performance of a contract (Art. 6(1)(b)) |
| Pseudonymized data contribution | Consent (Art. 6(1)(a) and 9(2)(a)) — withdrawable anytime |
| Security/server logs for cloud features | Legitimate interest (Art. 6(1)(f)) — keeping the service secure |

## 7. Retention and deletion

- **On-device data** is yours: delete it in the app ("Clear all data") or by uninstalling.
- **Cloud data** (account, backups, sync rows) is kept while your account exists and deleted when you delete your account. Residual copies may persist for a limited period in our hosting provider's encrypted database backups and expire automatically on its rolling retention schedule.
- **Contributed data** is deleted from the contribution dataset and excluded from all future statistics and training runs when you opt out or delete your account.
- **Server logs** are deleted on a short rolling schedule.

## 8. Delete your account and data

- **In the app:** Settings → Account → **Delete account**. This permanently removes your account data, sync rows and stored backups from our systems.
- **By e-mail:** send a deletion request to **odinskjaervik@gmail.com** from any address — you do not need the app installed. We will delete the data associated with your account and confirm.
- **On-device data** can be deleted anytime via Settings → "Clear all data", or by uninstalling the app.

## 9. Your rights

Under the GDPR you have the right to: access your personal data and obtain a copy of it; rectification of inaccurate data; erasure; restriction of processing; data portability — receiving the data you provided in a structured, commonly used, machine-readable format (the in-app export covers your training data); and to withdraw any consent at any time, without affecting the lawfulness of processing carried out before withdrawal.

**Right to object.** Where we process data based on legitimate interest (security logs, section 3), you have the right to object at any time on grounds relating to your particular situation (Art. 21 GDPR) by contacting us at the address above.

To exercise any of these rights, contact odinskjaervik@gmail.com. You also have the right to complain to a supervisory authority — in Norway, **Datatilsynet** (www.datatilsynet.no).

## 10. Children

Kraft is not directed at children. We do not knowingly process personal data of children below the age required to consent to information society services in their country (13 in Norway; between 13 and 16 elsewhere in the EEA). If you believe a child below that age has created an account or enabled data contribution, contact us and we will delete the data.

## 11. Changes to this policy

If this policy changes, the new version will be published at this address with an updated effective date. Material changes to how optional cloud features process data will be announced in the app.
