---
layout: default
title: Privacy Policy
lang: en
---

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
