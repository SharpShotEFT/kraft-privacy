---
layout: default
title: "Kraft Workout Tracker — Privacy Policy"
permalink: /
---

# Kraft Workout Tracker — Privacy Policy

[Privacy](./) · [Support](./support.html) · [Terms](./terms.html)

**Effective date:** 9 September 2026

**Data controller:** Odin Skjærvik, Norway

**Contact:** support@kraftlift.com

This policy covers Kraft's available Android app and describes the iOS 1.3 release being prepared. Apple-specific features below apply when using a version that offers them; this policy does not announce iOS availability. Features and sign-in options can differ by installed version and platform.

Kraft is local-first. In versions with account-free Basic, Free and Basic work without a Kraft account. Basic is verified by the device's store and works offline after purchase. A Kraft account is optional for linking Basic across Android and iPhone, and required for Pro and cloud features. Signing in alone does not enable workout sync, upload a training backup or link an older standalone Basic purchase. Older installed versions can still require a Kraft account for Basic until updated.

## Your device and exports

Kraft stores exercises, routines, workout sets, dates, notes, personal records, body measurements and settings in its local database. Measurements can include weight, body fat and circumferences. Some training/body information may reveal health information.

Rest alerts are scheduled locally, without uploading your workout schedule to a push-notification server. This release does not use HealthKit or read Apple Health data.

CSV, local backup and routine-sharing files you export are not encrypted by Kraft. Your chosen Files/share destination handles its copy under its own rules. Those copies are separate from account deletion.

In versions with routine sharing, a routine file contains its name, exercise definitions/instructions, planned sets/reps, supersets and routine exercise notes. Target weights are optional and off by default. The export does not automatically include workout history, personal records, body measurements, account/session information or purchase proof. Review notes and instructions before sharing: text you entered can still contain personal information.

Kraft creates, previews and imports these files locally, without uploading the file to a Kraft sharing service. Your chosen file provider or messaging app may use a network or keep its own copy. An imported routine becomes a normal local record; if you already enabled Pro sync, that existing consent also applies to the imported routine. Sharing does not enable sync or backup.

Kraft's iOS database is configured to be excluded from automatic operating-system backups. Keep your own deliberate export or encrypted online backup for recovery. This does not control files you export to another app/provider.

## Accounts and sign-in

Kraft and Supabase process your internal account ID, provider identifiers, email and available profile details to authenticate and operate your account. Google may supply a name or profile-image reference. Native Apple sign-in requests email, not full name; Apple may provide a private relay email.

Apple and Google operate their sign-in services under their policies. Kraft receives authentication assertions, not your provider password. Supabase session credentials are saved on your device to keep you signed in.

The backend exchanges Apple's short-lived code and keeps an encrypted Apple refresh credential to revoke Kraft's authorization during account deletion. Durable grant storage does not retain the authorization code, raw nonce or identity token. This credential is separate from your Supabase session and backup recovery key.

Google and Apple sign-ins using the same verified email may automatically open the same Kraft account through Supabase's identity-linking policy. If emails differ or you use Apple's Hide My Email, open your existing Kraft account and connect the other method in Account before switching. Kraft does not merge two separate accounts or transfer purchases just because you enter matching emails. An Apple relay address may create a different account. Credentials already linked to another Kraft account cannot simply be moved by the app.

## Purchases

Apple App Store or Google Play processes payments; Kraft does not receive your card number. A standalone Basic purchase is verified through the store on your device, without sending its purchase proof to Kraft's verification service. Its verified unlock is kept locally for offline use. Store payment and restoration still involve the store's data processing.

You can choose Link Basic purchase in Account to share a previously purchased Basic upgrade across Android/iOS. Buying Basic while signed into Kraft also attempts account linking, as disclosed before checkout. Linking shares account and purchase information with Kraft, not workout records, and does not enable backup or sync. Linking failure does not remove a verified local Basic unlock. Pro requires account-linked backend verification.

The verification service processes product and transaction identifiers, store environment, renewal/expiry/refund status and verification times. It stores necessary entitlement/ownership records. Google purchase tokens are bound by one-way hashes and, after successful verification for cross-device refresh, stored as encrypted server-only credentials. This server-side Google handling can apply to existing Android installations when they verify a purchase; it is not limited to the future iOS release. In versions offering Apple billing, Pro purchases use a server-issued account token; optional Basic linking and Pro verification use verified transaction identifiers. Standalone Basic does not require that account token.

Credential encryption keys are held separately on the server; this is not end-to-end encryption. The same Kraft account can use linked access on either platform. Basic ownership is retained locally without a recurring verification deadline; confirmed refunds or revocations can remove the corresponding unlock. Cached Pro access remains account-scoped and time-limited. A locally retained unlock is not a transferable receipt. Apple/Google may retain their payment records after Kraft account deletion.

## Optional backup and sync

**Online backup:** each upload requires separate confirmation for the displayed Kraft account, describing the training/body snapshot. A successful upload replaces that account's previous backup; it does not turn on automatic backup. Kraft encrypts the snapshot on your device with AES-256-GCM before uploading it to Supabase. The normal service stores ciphertext, not your recovery key. Save the recovery code privately: support cannot reconstruct a lost code or decrypt a backup without its key.

The key is account-scoped in protected device credential storage. Ordinary sign-out or provider revocation intentionally retains it. Device changes and OS keychain behavior can affect availability; do not rely on uninstall/reinstall for recovery or guaranteed secure key erasure.

**Sync:** enabling multi-device sync is a separate, account-scoped choice. Completed workouts/sets, routines, exercise details, notes, personal records and body measurements go to Supabase to merge changes. An unfinished workout stays on its device until completed. Sync is encrypted in transit and at rest and has account-access protection, but is not end-to-end encrypted: the service can read its rows. Enabling sync does not create an encrypted backup.

**Consent/withdrawal:** decline an upload and keep using local tracking. Approval authorizes that upload, not automatic future backup or sync. To stop future backups, do not upload again; turn sync off in Account to stop future sync from that device. Signing out turns sync off and requires fresh enablement after signing in. Signing out or disabling sync does not delete existing cloud data. Use Account → Delete account or contact support@kraftlift.com for cloud-data deletion. Withdrawal does not make prior lawful processing unlawful.

## Providers and locations

- **Supabase:** authentication, entitlements, encrypted backup files, optional sync and backend security. Primary project storage is Stockholm, Sweden; platform logs, support and subprocessors may process data outside the EEA. An EU storage region does not make every operation EU-only.
- **Cloudflare:** Apple purchase verification/notifications, processing account-token and transaction identifiers, signed subscription evidence and technical request information. Its global infrastructure may process this outside the EEA. Kraft does not send training/body records or backup recovery keys to that verifier.
- **Apple/Google:** the sign-in/store service you use, under its applicable terms/privacy rules.
- **Support email:** a monitored Gmail mailbox handles information you voluntarily send to answer a request and verify account access. Google processes that correspondence under its applicable service/privacy terms. Do not send passwords, recovery codes, sign-in credentials or full sensitive training exports.

Applicable processor agreements and transfer safeguards govern provider processing. Contact us for information about safeguards relevant to your data. See [Supabase DPA](https://supabase.com/legal/customer-resources/data-processing-addendum), [Cloudflare DPA](https://www.cloudflare.com/cloudflare-customer-dpa/), [Apple Privacy](https://www.apple.com/legal/privacy/) and [Google Privacy](https://policies.google.com/privacy).

## SDKs, technical information and advertising

Kraft has no ads, does not sell personal information and does not use training/body records for advertising. It does not intentionally perform cross-app advertising tracking.

Providers may process identifiers, IP/network information and service-usage/security data. Google's packaged iOS sign-in SDK declares linked name, email, phone, approximate location, user/device identifiers, other usage and other data, with functionality/analytics purposes depending on the category. This does not mean Kraft asks you for every field or reads precise GPS; it identifies provider practices that also matter. [Google sign-in disclosure](https://developers.google.com/identity/sign-in/ios/app-privacy).

Sentry's library is included but is not configured to send crash reports in the current release settings. Crash reporting defaults off and requires an explicit on-device opt-in even if an endpoint is configured later. Settings can withdraw that opt-in; diagnostics are never required for Basic. Native crash queues, automatic session tracking, performance tracing and logs are disabled. Future activation still requires accurate disclosures and working controls. Kraft does not claim every packaged SDK is analytics-free.

Technical logs and minimal operational records support security, reliability, verification and deletion completion. Application code avoids logging recovery keys, raw purchase credentials, signed purchase payloads or training records.

## Purposes and legal bases

Subject to applicable law, requested account/services and purchase validation rely on performing the service contract; security/abuse prevention relies on legitimate interests. Optional cloud processing revealing health information requires explicit purpose-specific consent in addition to an applicable general legal basis. Support processes what is needed to respond and protect the account.

These bases do not remove your rights. The [GDPR](https://eur-lex.europa.eu/eli/reg/2016/679/oj/eng) provides general bases and additional conditions for health-related data.

## Retention and deletion

Local records remain until deleted. Exports remain where you saved/shared them. Online account deletion does not erase your local workout database.

Account, purchase metadata, sync and online backup data are kept to provide the services you use. Account deletion removes your account and cloud training/body records and deletes backups or initiates any remaining storage cleanup. If cleanup cannot be confirmed immediately, Kraft reports the limitation and retries. It is not a promise that every security, purchase or deletion record disappears immediately.

Encrypted Apple authorization material and minimal identifiers may survive account deletion to finish revocation or resolve an interrupted authorization safely. Verified revocation clears sensitive grant fields. Unknown attempts are not marked successful by age alone. Unresolved authorization/revocation/deletion cases are reviewed weekly to pursue completion and remove material no longer needed; weekly review is not a promise that Apple or another provider will resolve a case within a week. Minimal deletion guards/opaque receipts prevent unsafe retries; they do not continue operating your deleted training account.

Encrypted Google refresh handles are removed with the Kraft account. Resolved support correspondence is retained for 12 months after resolution. Necessary legal/security exceptions are documented and reviewed, not a reason to keep every support case indefinitely. Other independent store transaction records, provider backup copies and security logs follow their applicable necessary purposes/retention requirements. Residual backups can outlast deletion from active systems; we do not promise immediate erasure from every independent provider. Kraft minimizes retained operational data rather than keeping unnecessary payloads by default.

Kraft attempts to clear a deleted account's local backup key on that device. A cleanup failure, another device, OS keychain copy or written recovery code can remain. Manage your external recovery codes/exports separately.

## Delete your account and data
{: #delete-your-account-and-data}

Use Settings → Account → Delete account, or request deletion at support@kraftlift.com without the app. Proportionate account-ownership verification may be required; never send a password or recovery code.

Deleting your account does **not** cancel App Store/Google Play billing. Cancel with the store separately. Settings → Clear all data removes local records; cloud and exported copies are separate.

## Rights and questions

Where applicable, request access, correction, deletion, restriction, portability or processing/safeguard information. You may withdraw consent or object to legitimate-interest processing on grounds relating to your situation. Email support@kraftlift.com. Local training export is not a complete export of provider/account metadata.

You may complain to your supervisory authority; in Norway, [Datatilsynet](https://www.datatilsynet.no/).

## Children and young people

Kraft is a general fitness tracker, not a service specifically directed at children. The app does not currently verify age or provide a parental-consent flow. A store content rating is not confirmation that someone can independently consent to every use of their personal information; applicable requirements depend on the person, processing and jurisdiction.

If you are concerned about a child's information or want help exercising rights on their behalf, contact support@kraftlift.com. We assess the request and may need proportionate confirmation of authority before disclosing or deleting information. Do not send a child's identity documents, health records or account credentials in an initial email.

Policy changes will carry an effective date. Material changes to optional sensitive-data processing require appropriate notice/consent before that processing begins.
