---
layout: default
title: Privacy Policy
lang: en
---

> [Read the proposed changes](https://thkim0118.github.io/hancute-legal/upcoming/1.0.9/notice/en) · [Read the current policy](#current-policy)


# Privacy Policy

> **Public review proposal** — This proposal is not final and does not replace the current policy. Unverified matters remain identified for review; the content and planned effective time may change.

- Preparation time: `2026-10-27T09:21:50+09:00`
- Planned effective time: `2026-11-03T18:00:00+09:00` (Korea Standard Time)


**Effective Date: November 3, 2026, 6:00 p.m. (planned, Korea Standard Time)**

HanCutE (한컷에, hereinafter "the App") values and protects users' personal information. This Privacy Policy describes what information the App collects, how it is used, and what rights users have regarding their data.

---

The revised App 1.0.9 implementation uses Firebase Analytics and Crashlytics, defaulting usage analytics and error reporting to ON when no preference exists and preserving existing OFF choices. **TO CONFIRM:** default ON is not explicit consent. Verify purpose/region-specific processing grounds, release binaries, provider settings, and store disclosures.

## Usage analytics and error-reporting settings

- Usage analytics and error reporting are ON by default and can be turned OFF separately in Settings. Existing OFF choices are preserved on upgrade.
- A default or continued service use is not recorded as consent. Initial defaults and explicit setting changes are distinguished; these records do not establish separate consent evidence.
- Allowlisted photo selection, editing, layout, face-covering, and export events and errors are sent to the applicable Firebase service. Custom events exclude photos, face coordinates, inquiry text, and access tokens.
- Turning OFF stops app-issued events/error reports. Native Crashlytics automatic reporting changes may take effect on the next launch; this does not delete previously transmitted records.
- The previously selected uniform 90-day policy cannot be asserted for Firebase. Standard Analytics user/event retention settings are 2 or 14 months and do not equally apply to standard aggregated reports. Crashlytics retains associated report data for 90 days before starting deletion. **TO CONFIRM:** actual production settings and final disclosures.
- Do not treat the revised documents as ready for publication or production deployment until the applicable processing grounds and platform requirements have been verified.

## 1. Purpose of Processing Personal Information

The App processes personal information for the following purposes:

| Purpose | Description |
|---------|-------------|
| User Inquiry Handling | Receiving and responding to inquiries via in-app inquiry form, including follow-up conversations |
| Advertising | Displaying personalized or non-personalized ads |
| App Update Management | Checking minimum version and prompting updates |
| Usage analytics | Understand feature usage to improve the service |
| Error/crash diagnostics | Diagnose errors and improve stability |

## 2. Types of Personal Information Collected

### Information Provided by Users

| Item | When Collected | Required |
|------|---------------|----------|
| Inquiry content | When submitting an inquiry | Required (inquiry only) |
| Follow-up messages | When continuing a conversation after receiving a reply | Optional |
| Attached images (up to 3, max 5MB each) | When submitting an inquiry | Optional |

> The server generates an inquiry token and returns it to the App. The App stores it locally and sends it when retrieving the inquiry or adding follow-up messages. Do not share the token: it is used to access the inquiry. The in-app inquiry form does not require an email address. If you contact us directly by email, your sender address and message are processed.

### Automatically Collected Information

| Item | Collected By | Purpose |
|------|-------------|---------|
| Device info (OS version, device model, app version) | App | Inquiry handling when an inquiry is submitted |
| Advertising identifier (IDFA/GAID) | Google AdMob | Ad serving |
| Ad interaction data | Google AdMob | Ad performance measurement |
| Allowlisted feature events, app/device information, SDK identifiers | Firebase Analytics | Usage analysis; OFF control in Settings |
| Error/crash reports, app/device information, SDK identifiers | Firebase Crashlytics | Stability diagnostics; OFF control in Settings |
| App version, device info, Firebase installation ID | Firebase Remote Config / Installations | Update, maintenance, and app configuration |
| Consent status | Google UMP (User Messaging Platform) | Advertising privacy choices |
| Request IP address, timestamp, requested function | Inquiry API | Rate limiting and abuse prevention |
| Device/app information, SDK performance and usage metrics | Google ML Kit (Android) | Face detection SDK diagnostics and maintenance |

### Collection Methods

- Direct user input (inquiry form)
- Automatic collection via in-app SDKs (including Firebase, AdMob, and Android ML Kit)

## 3. Retention Period

> **TO CONFIRM:** Retention must be checked against production settings and deletion procedures. Writing a retention period does not implement automatic deletion.

| Item | Proposed treatment and outstanding confirmation |
|------|----------------------------------------------|
| Inquiries, replies, follow-ups, attached images | Retain for one year after resolution (confirmed by the operator on October 26, 2026). Production resolution tracking and a five-minute retention job were activated and verified on October 26, 2026. Fourteen legacy resolved inquiries with unknown completion dates are excluded without guessing dates. Email copies and backups need separate confirmation |
| Rate-limit IP logs | Records older than one hour are cleaned by the five-minute job. Expired-row cleanup was verified in production on October 26, 2026. Failures or downtime can delay cleanup; this is not an absolute retention bound |
| Firebase Analytics user/event data (1.0.9 and previous versions) | **TO CONFIRM:** actual production retention and reset-on-new-activity settings. Standard properties offer 2 or 14 months, with expired data deleted monthly. This setting does not apply to standard aggregated reports |
| Firebase Crashlytics reports (1.0.9 and previous versions) | Under Google policy, crash traces, extracted minidump data, and associated identifiers are retained for 90 days before removal from live and backup systems begins. This does not promise deletion of all copies on day 90 |
| Administrator inquiry notification emails/logs | Confirm Resend plan/settings and separate retention/deletion for the receiving administrator mailbox |
| Firebase installation IDs (Remote Config) | Google describes retention until an API deletion request and removal from live/backup systems within 180 days afterward. Operator deletion/request-identification procedures require confirmation |
| Advertising, consent, ML Kit diagnostics | Confirm processing and retention under the applicable Google service policies |

Deletion procedures must cover the database, attachments, and separate email copies. Uninstalling the App does not delete server-side inquiries or administrator emails.

## 4. Disclosure to Third Parties

The App does not, in principle, provide users' personal information to third parties, except:

- When the user has given prior consent
- When required by law or by a lawful request from an investigative authority

## 5. Outsourced Processing

The App outsources personal data processing to the following service providers:

| Processor | Task | Data Processed |
|-----------|------|---------------|
| Supabase Inc. | Inquiry storage and management | Inquiries, replies, follow-ups, inquiry tokens, device info, attached images, rate-limit IP logs |
| Google LLC (Firebase Analytics / Crashlytics) | Usage analysis and error/crash diagnosis | Event/diagnostic data, app/device information, SDK identifiers; verify actual settings |
| Google LLC (Firebase Remote Config / Installations) | Update, maintenance, and app configuration | App version, device info, Firebase installation ID |
| Google LLC (AdMob) | Ad serving | Advertising identifier, device info, ad interaction data |
| Google LLC (UMP) | Advertising privacy choices | Consent status, device identifiers |
| Google LLC (ML Kit, Android) | Face detection SDK diagnostics and maintenance | Device/app information, performance and usage metrics; no editing photos or detection results are transmitted |
| Resend | Inquiry notification emails to the Operator | Excerpts of inquiries/follow-ups, app name, inquiry management links, administrator recipient address |
| Vercel Inc. | Hosting server functions for the inquiry administration BO | Inquiry/reply information handled through the BO and request information |

## 6. Overseas Data Transfer

The verified production Supabase region for inquiry database and attachment storage is Japan (Tokyo, ap-northeast-1). This does not mean all provider support, logs, or subprocessor activity is limited to Japan.

| Recipient | Verified processing and outstanding confirmation |
|-----------|-----------------------------------------------|
| Supabase Inc. | Inquiry/attachment storage: Japan (Tokyo). **TO CONFIRM:** support/log/subprocessor locations, transfer basis, and retention/deletion conditions |
| Google LLC | Firebase, AdMob, UMP, and Android ML Kit diagnostics. **TO CONFIRM:** countries, data items, transfer timing/basis, and retention for each service |
| Resend | Administrator inquiry notification delivery. **TO CONFIRM:** storage/processing countries and retention under the actual contract and subprocessors |
| Vercel Inc. | Inquiry administration server processing. **TO CONFIRM:** production execution region, logging, subprocessor countries, and retention |

Inquiry tokens are transmitted in API requests, inquiry content/images on submission, and administrator notifications when the notification task runs. Transfer refusal methods and consequences must also be finalized before finalization.

- [Google Privacy Policy](https://policies.google.com/privacy)
- [ML Kit privacy information](https://developers.google.com/ml-kit/terms)
- [Supabase Privacy Policy](https://supabase.com/privacy)
- [Resend Data Processing Addendum](https://resend.com/legal/dpa)
- [Vercel Privacy Policy](https://vercel.com/legal/privacy-policy)

## 7. Data Destruction

### Procedure

Inquiries with recorded completion dates become eligible one year after resolution. The five-minute job removes recorded attachments before deleting the inquiry, replies and follow-ups, and retries failures. Unknown legacy completion dates are not inferred. IP logs use a separate one-hour threshold. **TO CONFIRM:** handling of unknown-date records, administrator email copies, backups and unreferenced attachments, including procedures and owners.

### Method

- Electronic files: Permanently deleted using methods that prevent recovery
- Other records: Shredded or incinerated

## 8. User Rights

Users may exercise the following rights regarding their personal information:

1. **Right to access**: Request access to personal information being processed
2. **Right to correction/deletion**: Request correction of inaccurate information or deletion
3. **Right to suspend processing**: Request suspension of personal information processing
4. **Right to withdraw consent**: Withdraw previously given consent

To exercise these rights, contact us at the email address below. We process requests and communicate results without undue delay within the period applicable to the request and jurisdiction. Under Korean law, access requests are generally handled within 10 days; any legally permitted deferral or restriction is explained with the reason and objection procedure. Correction, deletion, and suspension requests follow the applicable statutory procedures and deadlines. Requests governed by the GDPR follow the timeline in Article 12(3), as described in Section 16.

For inquiry-related requests, we verify the request using the minimum information needed to connect it to the inquiry. Do not post inquiry tokens publicly. We do not routinely require a copy of an identity document.

## 9. Automatic Data Collection

### SDKs Used

| SDK | Purpose | How to Opt Out |
|-----|---------|---------------|
| Firebase Analytics | Usage analytics | App Settings > turn off Send usage statistics |
| Firebase Crashlytics | Error/crash diagnostics | App Settings > turn off Send crash reports. Native automatic reporting changes may take effect on the next launch |
| Firebase Remote Config | Update/maintenance management | Essential for service operation; cannot be disabled separately |
| Google AdMob | Ad serving | iOS: Settings > Privacy > Tracking; Android: Settings > Google > Ads |
| Google UMP | Advertising privacy choices | Reopen advertising privacy choices in Settings when UMP requires this entry point. Verify actual regional console settings |
| Apple SKAdNetwork | Privacy-preserving ad attribution | Apple framework that does not track individual users |

### Advertising Identifiers (IDFA/GAID)

- **iOS**: The operating system's App Tracking Transparency (ATT) choice applies. Declining restricts access to the advertising identifier; it does not mean all SDK collection stops or guarantee a particular ad type.
- **Android**: You can delete your advertising ID or disable personalized ads in Settings > Google > Ads.

## 9-1. On-Device Data Storage

The App stores the following information locally (SharedPreferences). Inquiry tokens and pending inquiries are transmitted for support; not all locally stored data remains exclusively on-device.

| Item | Purpose |
|------|---------|
| Premium feature unlock expiry | Managing 24-hour feature unlock status from rewarded ads |
| Custom ratios (up to 3) | Preserving user settings |
| Notice confirmation status | Preventing re-display of already confirmed notices |
| Analytics/error-reporting preferences and history | Preserve choices and diagnose preference application errors. Purpose, ON/OFF, default/legacy/user action, time, and notice version stay on-device and are not uploaded |
| API response cache (notices/FAQ/categories) | Minimizing network requests |
| Privacy notice shown flag | Managing one-time privacy notice display |
| Update snooze timestamp | Managing 24-hour soft update snooze |
| Inquiry token, content preview, creation time | Local inquiry list and server inquiry retrieval/follow-ups |
| Pending inquiry content and device information | Retry after a failed request |

Preference history is limited to the latest 50 entries. Entries older than 90 days are pruned during initialization or preference changes. No cleanup occurs while the App is not running, so deletion within 90 days of creation is not guaranteed. Current ON/OFF preferences are stored separately to preserve choices. History is not evidence of consent.

Usage analytics and error reporting can be changed separately in Settings. Initial defaults and explicit user changes are distinguished; default ON is not consent. OFF choices persist after restarting. Updating or changing preferences is not a deletion request for previously transmitted data.

## 10. Security Measures

The App takes the following measures to ensure the safety of personal information:

1. **Encryption in transit**: All data transfers use HTTPS (TLS) encryption
2. **Access control**: Row-Level Security (RLS) policies on the database (Supabase) prevent unauthorized access
3. **Data minimization**: Only the minimum information necessary for service provision is collected
4. **Local image processing**: Photo merging, face-region detection, blur, and emoji compositing run on-device. Android uses Google ML Kit and iOS uses Apple Vision. The App does not create or store server-side facial identity/authentication data. Editing photos and detection results are not sent to the Operator's servers. Images voluntarily attached to inquiries or shared with another app are separate transfers.

Android ML Kit sends SDK diagnostic, performance, and usage data to Google separately from photos/detection results. Analytics/error-reporting preferences are separate from processing by AdMob, UMP, Remote Config, ML Kit, and other services.

## 11. Privacy Officer

For inquiries, complaints, or remedies regarding personal information processing:

| Item | Detail |
|------|--------|
| Name | Taehyung Kim |
| Position | Representative (Individual Developer) |
| Location | Republic of Korea |
| Contact | choir0118@gmail.com |

For reporting privacy violations or seeking consultation (Korean agencies):
- KISA Privacy Center: [privacy.kisa.or.kr](https://privacy.kisa.or.kr) / 118
- Personal Information Dispute Mediation Committee: [kopico.go.kr](https://www.kopico.go.kr) / 1833-6972
- Supreme Prosecutors' Office Cyber Investigation: [spo.go.kr](https://www.spo.go.kr) / 1301
- National Police Agency Cyber Bureau: [police.go.kr](https://www.police.go.kr) / 182

## 12. Data Breach Response

In the event of a personal data breach, we take steps to limit harm and notify individuals and authorities according to the requirements and deadlines of applicable law. Where the GDPR applies, we notify the supervisory authority without undue delay and, where feasible, within 72 hours of awareness, unless the breach is unlikely to result in a risk to individuals’ rights and freedoms. We explain any delay. Where a high risk is likely, we also inform affected individuals without undue delay unless a statutory exception applies. Notifications include the information required by law, such as the nature of the breach, likely effects, mitigation measures, and contact details.

## 13. Changes to This Policy

This Privacy Policy may be updated due to changes in law, policy, or services. Changes will be announced via in-app notices or this page.

- **Proposed version**: 1.3
- **Effective date**: November 3, 2026, 6:00 p.m. (planned, Korea Standard Time)

## 14. Children's Privacy

The App is available to everyone without an age restriction. Eligibility to use the service is separate from safeguards required for processing children’s personal information. Where consent is required under Korea’s Personal Information Protection Act to process information about a child under 14, consent from the legal representative and verification are required. Children’s privacy rules in other countries, including US COPPA, must be assessed under their applicable scope.

**TO CONFIRM — implementation review before finalization:** Reconcile advertising, analytics, crash reporting, inquiries, and store target-age settings with a service that includes child users. Procedures for obtaining and verifying parental consent where required, handling rights requests, and deleting children’s information have not yet been verified. These safeguards are not represented as implemented merely by updating this document.

## 15. California Residents (CCPA/CPRA)

**TO CONFIRM:** Check actual AdMob personalization and restricted-data-processing settings before determining sale/sharing under CCPA/CPRA and applicable opt-out methods. Do not make an unverified blanket no-sale/no-sharing declaration.

**Categories of personal information collected in the past 12 months:**

| Category | Items Collected | Source | Purpose | Third-Party Sharing |
|----------|----------------|--------|---------|-------------------|
| Identifiers | Advertising ID (IDFA/GAID), inquiry token | Device and server generated | Advertising, inquiry handling | Google (AdMob), Supabase |
| Device info | OS version, device model, app version | Automatic collection | Crash analysis, inquiry handling | Google (Firebase), Supabase |
| Usage data | App usage events, crash logs, and SDK identifiers (1.0.9 and previous versions) | Firebase SDKs | Service improvement, stability | Google (Firebase) |
| User content | Inquiry content, attached images | Directly provided by user | Inquiry handling | Supabase, Vercel, Resend (notification excerpts) |
| Request/SDK diagnostic information | Request IP/time/function; Android ML Kit device/app/performance information | API and SDK | Abuse prevention, SDK maintenance | Supabase, Google (ML Kit) |

**Your rights as a California resident:**
1. **Right to know**: Confirm the categories of personal information collected, sources, purposes, and sharing recipients
2. **Right to delete**: Request deletion of collected personal information
3. **Right to correct**: Request correction of inaccurate personal information
4. **Non-discrimination**: You will not be discriminated against for exercising your rights

**Rewarded ads disclosure:** The rewarded ad program (watch an ad to unlock premium features for 24 hours) may constitute a "financial incentive" under CCPA Section 1798.125(b). Users who choose not to watch ads can still use the App's core functionality (photo merging, saving, sharing) without limitation.

To exercise these rights, contact us at choir0118@gmail.com.

## 16. Information for EEA Users (GDPR)

If you are located in the European Economic Area (EEA), the following additional information applies:

**Data Controller:**

| Item | Detail |
|------|--------|
| Name | Taehyung Kim |
| Location | Republic of Korea |
| Contact | choir0118@gmail.com |

**Legal basis for processing — TO CONFIRM:**

The revised 1.0.9 implementation uses default-ON Firebase Analytics/Crashlytics with separate OFF controls. This is not described as explicit opt-in consent. Advertising separately checks UMP choices and ad-request permission. Before publication, finalize the basis and actual production settings for remaining purposes including inquiries, advertising, Remote Config, and ML Kit diagnostics. Default-ON implementation does not establish a processing ground or prove consent.

**Your Rights under GDPR:**
1. **Right of access** (Article 15): Request a copy of your personal data being processed
2. **Right to rectification** (Article 16): Request correction of inaccurate personal data
3. **Right to erasure** (Article 17): Request deletion of your personal data
4. **Right to restriction of processing** (Article 18): Request restriction of processing in certain circumstances
5. **Right to data portability** (Article 20): Receive your data in a structured, commonly used, machine-readable format (JSON)
6. **Right to object** (Article 21): Object to processing based on legitimate interest. Upon objection, we will cease the relevant processing unless we demonstrate compelling legitimate grounds.
7. **Rights related to automated decision-making** (Article 22): Face detection assists editing. Verify advertising-provider profiling and the related rights information against actual settings before finalization.

To exercise any of these rights, contact us at choir0118@gmail.com. In accordance with GDPR Article 12(3), requests will be processed within one month, with a possible extension of up to three months for complex requests.

**Right to lodge a complaint:** EEA users have the right to lodge a complaint with their local data protection supervisory authority.

**EU consumer protection:** For users residing in the EU, nothing in this policy deprives you of the protection afforded by the mandatory provisions of the law of your country of residence.

**International transfers:** See Section 6. Finalize provider-specific transfer bases and safeguards before finalization; data is not described as transferring exclusively to the United States.

<!-- Sources checked 2026-10-26: https://firebase.google.com/docs/projects/manage-installations ; https://firebase.google.com/support/privacy ; https://support.google.com/analytics/answer/7667196 . Retention descriptions cover current and prior-version data. Actual Analytics property settings remain unverified. -->

<!-- proposed-legal-content-sha256: fd7a2b7a7fc649150c8ef1ea975f3b080ab64098b495e9824a463aa28df6ba1e -->


---

<span id="current-policy"></span>

## Current policy in effect


# Privacy Policy

**Effective Date: March 29, 2026**

HanCutE (한컷에, hereinafter "the App") values and protects users' personal information. This Privacy Policy describes what information the App collects, how it is used, and what rights users have regarding their data.

---

## 1. Purpose of Processing Personal Information

The App processes personal information for the following purposes:

| Purpose | Description |
|---------|-------------|
| User Inquiry Handling | Receiving and responding to inquiries via in-app inquiry form, including follow-up conversations |
| App Stability | Collecting and analyzing crash reports |
| Service Improvement | Analyzing app usage patterns to improve features |
| Advertising | Displaying personalized or non-personalized ads |
| App Update Management | Checking minimum version and prompting updates |

## 2. Types of Personal Information Collected

### Information Provided by Users

| Item | When Collected | Required |
|------|---------------|----------|
| Inquiry content | When submitting an inquiry | Required (inquiry only) |
| Follow-up messages | When continuing a conversation after receiving a reply | Optional |
| Attached images (up to 3, max 5MB each) | When submitting an inquiry | Optional |

> Inquiries are identified by an anonymous token generated on the user's device. No email address is collected.

### Automatically Collected Information

| Item | Collected By | Purpose |
|------|-------------|---------|
| Device info (OS version, device model, app version) | App / Firebase Crashlytics | Inquiry handling and crash analysis |
| App usage events (feature usage frequency, screen transitions) | Firebase Analytics | Service improvement |
| Crash logs (stack traces, device state) | Firebase Crashlytics | App stability |
| Advertising identifier (IDFA/GAID) | Google AdMob | Ad serving |
| Ad interaction data | Google AdMob | Ad performance measurement |
| App version and device info | Firebase Remote Config | Update/maintenance management |
| Consent status | Google UMP (User Messaging Platform) | GDPR consent management |

### Collection Methods

- Direct user input (inquiry form)
- Automatic collection via in-app SDKs (Firebase, AdMob)

## 3. Retention Period

| Item | Retention Period | Basis |
|------|-----------------|-------|
| Inquiry data (content, follow-up messages, images) | 1 year after resolution | Dispute resolution |
| Crash reports | 90 days from collection | Firebase Crashlytics default |
| App usage events | 14 months from collection | Firebase Analytics default |
| Ad data | Per Google's Privacy Policy | AdMob terms of service |

Data is deleted without delay once the retention period expires or the purpose of processing is achieved.

## 4. Disclosure to Third Parties

The App does not, in principle, provide users' personal information to third parties, except:

- When the user has given prior consent
- When required by law or by a lawful request from an investigative authority

## 5. Outsourced Processing

The App outsources personal data processing to the following service providers:

| Processor | Task | Data Processed |
|-----------|------|---------------|
| Supabase Inc. | Inquiry data storage and management | Inquiry content, follow-up messages, device info, attached images |
| Google LLC (Firebase Analytics) | App usage analysis | App usage events, device info |
| Google LLC (Firebase Crashlytics) | Crash reporting | Crash logs, device info |
| Google LLC (Firebase Remote Config) | Update/maintenance management | App version, device info |
| Google LLC (AdMob) | Ad serving | Advertising identifier, device info, ad interaction data |
| Google LLC (UMP) | GDPR consent management | Consent status, device identifiers |

## 6. Overseas Data Transfer

The App transfers personal information overseas for service provision:

| Recipient | Country | Data Items | Purpose | Transfer Method | Retention |
|-----------|---------|------------|---------|----------------|-----------|
| Google LLC (Firebase Analytics) | USA | App usage events, device info | App usage analysis | Transmission via network | 14 months |
| Google LLC (Firebase Crashlytics) | USA | Crash logs, device info | App stability | Transmission via network | 90 days |
| Google LLC (Firebase Remote Config) | USA | App version, device info | Update/maintenance management | Transmission via network | Per Google policy |
| Google LLC (AdMob) | USA | Ad identifier, device info, ad interaction data | Ad serving | Transmission via network | Per Google policy |
| Google LLC (UMP) | USA | Consent status, device identifiers | GDPR consent management | Transmission via network | Per Google policy |
| Supabase Inc. | USA | Inquiry content, follow-up messages, device info, images | User inquiry handling | Transmission via network | 1 year |

Recipient contact information for personal data inquiries: Google LLC — https://support.google.com/policies/contact/general_privacy_form, Supabase Inc. — privacy@supabase.io

Google LLC holds ISO 27001 and SOC 2 certifications and participates in the EU-US Data Privacy Framework. Supabase Inc. holds SOC 2 Type II certification.

For details on each provider's data protection practices:

- [Google Privacy Policy](https://policies.google.com/privacy)
- [Supabase Privacy Policy](https://supabase.com/privacy)

## 7. Data Destruction

### Procedure

Personal information is destroyed without delay when the retention period expires or the purpose of processing is achieved.

### Method

- Electronic files: Permanently deleted using methods that prevent recovery
- Other records: Shredded or incinerated

## 8. User Rights

Users may exercise the following rights regarding their personal information:

1. **Right to access**: Request access to personal information being processed
2. **Right to correction/deletion**: Request correction of inaccurate information or deletion
3. **Right to suspend processing**: Request suspension of personal information processing
4. **Right to withdraw consent**: Withdraw previously given consent

To exercise these rights, please contact us at the email address below. Requests will be processed without delay (within 10 days).

We may request identification documents to verify your identity when processing rights requests.

## 9. Automatic Data Collection

### SDKs Used

| SDK | Purpose | How to Opt Out |
|-----|---------|---------------|
| Firebase Analytics | App usage analysis | Disable analytics sharing in device settings |
| Firebase Crashlytics | Crash reporting | Uninstalling the app stops data collection |
| Firebase Remote Config | Update/maintenance management | Essential for service operation; cannot be disabled separately |
| Google AdMob | Ad serving | iOS: Settings > Privacy > Tracking; Android: Settings > Google > Ads |
| Google UMP | GDPR consent management | Required for EU legal compliance |
| Apple SKAdNetwork | Privacy-preserving ad attribution | Apple framework that does not track individual users |

### Advertising Identifiers (IDFA/GAID)

- **iOS**: The app requests App Tracking Transparency (ATT) consent on first launch. If declined, non-personalized ads are shown.
- **Android**: You can delete your advertising ID or disable personalized ads in Settings > Google > Ads.

## 9-1. On-Device Data Storage

The App stores the following data locally on your device (SharedPreferences). This data is never transmitted outside your device.

| Item | Purpose |
|------|---------|
| Premium feature unlock expiry | Managing 24-hour feature unlock status from rewarded ads |
| Custom ratios (up to 3) | Preserving user settings |
| Notice confirmation status | Preventing re-display of already confirmed notices |
| API response cache (notices/FAQ/categories) | Minimizing network requests |
| Privacy notice shown flag | Managing one-time privacy notice display |
| Update snooze timestamp | Managing 24-hour soft update snooze |
| Inquiry token | Retrieving inquiry history (anonymous identifier) |

## 10. Security Measures

The App takes the following measures to ensure the safety of personal information:

1. **Encryption in transit**: All data transfers use HTTPS (TLS) encryption
2. **Access control**: Row-Level Security (RLS) policies on the database (Supabase) prevent unauthorized access
3. **Data minimization**: Only the minimum information necessary for service provision is collected
4. **Local image processing**: Photo merging is performed entirely on-device. Photos are never uploaded to servers. (Except images voluntarily attached by users when submitting inquiries)

## 11. Privacy Officer

For inquiries, complaints, or remedies regarding personal information processing:

| Item | Detail |
|------|--------|
| Name | Taehyung Kim |
| Position | Representative (Individual Developer) |
| Location | Republic of Korea |
| Contact | choir0118@gmail.com |

For reporting privacy violations or seeking consultation (Korean agencies):
- KISA Privacy Center: [privacy.kisa.or.kr](https://privacy.kisa.or.kr) / 118
- Personal Information Dispute Mediation Committee: [kopico.go.kr](https://www.kopico.go.kr) / 1833-6972
- Supreme Prosecutors' Office Cyber Investigation: [spo.go.kr](https://www.spo.go.kr) / 1301
- National Police Agency Cyber Bureau: [police.go.kr](https://www.police.go.kr) / 182

## 12. Data Breach Response

In the event of a personal data breach, we will notify affected users and relevant authorities without undue delay in accordance with applicable law (Korean PIPA Article 34, GDPR Articles 33-34). In accordance with GDPR Article 33, the relevant supervisory authority will be notified within 72 hours of becoming aware of the breach. The notification will include the types of data affected, the circumstances of the breach, measures taken to mitigate harm, and contact information for further inquiries.

## 13. Changes to This Policy

This Privacy Policy may be updated due to changes in law, policy, or services. Changes will be announced via in-app notices or this page.

- **Current version**: 1.2
- **Effective date**: March 29, 2026

## 14. Children's Privacy

This service is not directed at children under the age of 14 (under Korean Personal Information Protection Act) or 13 (under US COPPA). We do not knowingly collect personal information from children. If we become aware that personal information has been collected from a child, we will delete it promptly.

## 15. California Residents (CCPA/CPRA)

The App does not sell or share users' personal information.

**Categories of personal information collected in the past 12 months:**

| Category | Items Collected | Source | Purpose | Third-Party Sharing |
|----------|----------------|--------|---------|-------------------|
| Identifiers | Advertising ID (IDFA/GAID), inquiry token | Device/app auto-generated | Advertising, inquiry handling | Google (AdMob) |
| Device info | OS version, device model, app version | Automatic collection | Crash analysis, inquiry handling | Google (Firebase), Supabase |
| Usage data | App usage events, crash logs | Automatic collection | Service improvement, stability | Google (Firebase) |
| User content | Inquiry content, attached images | Directly provided by user | Inquiry handling | Supabase |

**Your rights as a California resident:**
1. **Right to know**: Confirm the categories of personal information collected, sources, purposes, and sharing recipients
2. **Right to delete**: Request deletion of collected personal information
3. **Right to correct**: Request correction of inaccurate personal information
4. **Non-discrimination**: You will not be discriminated against for exercising your rights

**Rewarded ads disclosure:** The rewarded ad program (watch an ad to unlock premium features for 24 hours) may constitute a "financial incentive" under CCPA Section 1798.125(b). Users who choose not to watch ads can still use the App's core functionality (photo merging, saving, sharing) without limitation.

To exercise these rights, contact us at choir0118@gmail.com.

## 16. Information for EEA Users (GDPR)

If you are located in the European Economic Area (EEA), the following additional information applies:

**Data Controller:**

| Item | Detail |
|------|--------|
| Name | Taehyung Kim |
| Location | Republic of Korea |
| Contact | choir0118@gmail.com |

**Legal Basis for Processing:**
- **Legitimate interest**: Crash reporting (Article 6(1)(f) GDPR). We have determined that our legitimate interest in ensuring app stability outweighs any potential impact on users' rights and freedoms.
- **Consent**: App usage analytics (Firebase Analytics) and personalized advertising (Article 6(1)(a) GDPR). Consent is collected via Google UMP.
- **Contract performance**: Inquiry handling, update/maintenance management (Article 6(1)(b) GDPR)

**Your Rights under GDPR:**
1. **Right of access** (Article 15): Request a copy of your personal data being processed
2. **Right to rectification** (Article 16): Request correction of inaccurate personal data
3. **Right to erasure** (Article 17): Request deletion of your personal data
4. **Right to restriction of processing** (Article 18): Request restriction of processing in certain circumstances
5. **Right to data portability** (Article 20): Receive your data in a structured, commonly used, machine-readable format (JSON)
6. **Right to object** (Article 21): Object to processing based on legitimate interest. Upon objection, we will cease the relevant processing unless we demonstrate compelling legitimate grounds.
7. **Rights related to automated decision-making** (Article 22): The App does not engage in automated decision-making, including profiling.

To exercise any of these rights, contact us at choir0118@gmail.com. In accordance with GDPR Article 12(3), requests will be processed within one month, with a possible extension of up to three months for complex requests.

**Right to lodge a complaint:** EEA users have the right to lodge a complaint with their local data protection supervisory authority.

**EU consumer protection:** For users residing in the EU, nothing in this policy deprives you of the protection afforded by the mandatory provisions of the law of your country of residence.

**International Transfers:** Data is transferred to the United States. Google LLC participates in the EU-US Data Privacy Framework. All transfers are encrypted via HTTPS/TLS.

<!-- legal-content-sha256: 4d88df9e8e83734eeec90829afc8844d1772d5fe90d454dcac7d541659ff29b7 -->
