---
layout: default
title: Privacy Policy
lang: en
---

# Privacy Policy

**Effective Date: March 24, 2026**

HanCutE (한컷에, hereinafter "the App") values and protects users' personal information. This Privacy Policy describes what information the App collects, how it is used, and what rights users have regarding their data.

[한국어 버전](/hancute-legal/privacy/ko)

---

## 1. Purpose of Processing Personal Information

The App processes personal information for the following purposes:

| Purpose | Description |
|---------|-------------|
| User Inquiry Handling | Receiving and responding to inquiries via email |
| App Stability | Collecting and analyzing crash reports |
| Service Improvement | Analyzing app usage patterns to improve features |
| Advertising | Displaying personalized or non-personalized ads |
| App Update Management | Checking minimum version and prompting updates |

## 2. Types of Personal Information Collected

### Information Provided by Users

| Item | When Collected | Required |
|------|---------------|----------|
| Email address | When submitting an inquiry | Required (inquiry only) |
| Inquiry content | When submitting an inquiry | Required (inquiry only) |
| Attached images | When submitting an inquiry | Optional |

### Automatically Collected Information

| Item | Collected By | Purpose |
|------|-------------|---------|
| Device info (OS version, device model, app version) | App / Firebase Crashlytics | Inquiry handling and crash analysis |
| App usage events (feature usage frequency, screen transitions) | Firebase Analytics | Service improvement |
| Crash logs (stack traces, device state) | Firebase Crashlytics | App stability |
| Advertising identifier (IDFA/GAID) | Google AdMob | Ad serving |
| Ad interaction data | Google AdMob | Ad performance measurement |

### Collection Methods

- Direct user input (inquiry form)
- Automatic collection via in-app SDKs (Firebase, AdMob)

## 3. Retention Period

| Item | Retention Period | Basis |
|------|-----------------|-------|
| Inquiry data (email, content, images) | 1 year after resolution | Dispute resolution |
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
| Supabase Inc. | Inquiry data storage and management | Email, inquiry content, device info, attached images |
| Google LLC (Firebase) | App analytics and crash reporting | App usage events, crash logs, device info |
| Google LLC (AdMob) | Ad serving | Advertising identifier, device info, ad interaction data |

## 6. Overseas Data Transfer

The App transfers personal information overseas for service provision:

| Recipient | Country | Data Items | Purpose | Retention |
|-----------|---------|------------|---------|-----------|
| Google LLC (Firebase Analytics) | USA | App usage events, device info | App usage analysis | 14 months |
| Google LLC (Firebase Crashlytics) | USA | Crash logs, device info | App stability | 90 days |
| Google LLC (AdMob) | USA | Ad identifier, device info, ad interaction data | Ad serving | Per Google policy |
| Supabase Inc. | USA | Email, inquiry content, device info, images | User inquiry handling | 1 year |

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

To exercise these rights, please contact us at the email address below. Requests will be processed without delay (within 10 business days).

## 9. Automatic Data Collection

### SDKs Used

| SDK | Purpose | How to Opt Out |
|-----|---------|---------------|
| Firebase Analytics | App usage analysis | Disable analytics sharing in device settings |
| Firebase Crashlytics | Crash reporting | Uninstalling the app stops collection |
| Google AdMob | Ad serving | iOS: Settings > Privacy > Tracking; Android: Settings > Google > Ads |

### Advertising Identifiers (IDFA/GAID)

- **iOS**: The app requests App Tracking Transparency (ATT) consent on first launch. If declined, non-personalized ads are shown.
- **Android**: You can delete your advertising ID or disable personalized ads in Settings > Google > Ads.

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
| Contact | hancute.app@gmail.com |

## 12. Changes to This Policy

This Privacy Policy may be updated due to changes in law, policy, or services. Changes will be announced via in-app notices or this page.

- **Current version**: 1.0
- **Effective date**: March 24, 2026

## 13. Children's Privacy

This service is not directed at children under the age of 14 (under Korean law) or 13 (under COPPA). We do not knowingly collect personal information from children. If we become aware that personal information has been collected from a child, we will delete it promptly.
