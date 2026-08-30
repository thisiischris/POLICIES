# Privacy Policy

**Effective Date: June 30, 2026**

Factor Feed does not require a user account. Most preferences and cached data stay on your device; uninstalling the App removes that local data. If you enabled push notifications, we also stored a device push token and alert preferences on our servers so delivery could work — turn off Notification Alerts in Settings (or revoke system notification permission) to stop using that token, and email support+factorfeed@signatureapps.app or use Contact Support in Settings if you want confirmation of server-side deletion beyond uninstall.

## Introduction

This Privacy Policy describes how Factor Feed ("we," "us," or "our") handles information when you use the Factor Feed mobile application (the "App"). Factor Feed is a client for economic and market information; your preferences and cached data are stored primarily on your device.

By using the App, you acknowledge this Policy. If you do not agree, please discontinue use of the App.

## What we do not do

The App does not require you to create a user account. We do not collect your name, email address, or similar profile information through a sign-in flow for use in our own customer database.

The production App does not include third-party advertising SDKs, cross-app behavioral tracking, or sale of personal information for targeted advertising. The one exception is RevenueCat, which processes optional Factor Feed Pro subscription/purchase status — see "Subscriptions (Factor Feed Pro)" below.

## Information stored on your device

The App persists data locally using the platform’s AsyncStorage (and similar mechanisms) so that your experience works offline-first and restarts quickly. Categories of locally stored information include:

- **Appearance and layout:** theme (light/dark) and related UI preferences.
- **Macro and economy preferences:** which indicators you track, section order, overview customization, optional notes you attach to indicators, date-range selections, sparkline time ranges, and related display settings.
- **Terminal preferences:** which terminal categories and widgets you enable.
- **Lists and UI state:** for example, pinned U.S. states and view modes where the App provides those controls.
- **Cached responses:** the App uses TanStack Query with a persisted cache (macro and market payloads you have already fetched) so charts and figures can render from the last known good data. Cache entries are bounded by age and version as configured in the App.

This locally stored information resides on your device unless you copy it elsewhere. Uninstalling the App or clearing the App’s storage (where the operating system allows) generally deletes this data.

## Network requests and servers

When you use live or refreshed data, the App makes HTTPS requests to our configured backend endpoints. In production, consolidated market and macro series are requested from our Supabase Edge Function using the project’s publishable (anon) API key in request headers where required by the gateway. Those requests identify the data resources being fetched (for example, FRED series identifiers or structured resource IDs), not your personal identity.

Our Edge Function and related server-side logic may call upstream public and commercial data providers (such as FRED, U.S. Treasury, Census, BLS-related releases, World Bank, NY Fed, Alternative.me for crypto sentiment indices, RapidAPI-hosted indices where we have configured access, and similar sources listed in the App’s Data Sources disclosure) to assemble responses. Those providers receive requests from our infrastructure under their own terms and privacy policies.

In limited configurations, the App may call a third-party API directly from your device (for example, when a RapidAPI key is present and our unified proxy is unavailable). Such calls transmit only what is needed to retrieve the requested index or time series (typically API key headers and endpoint parameters), not an app-specific user ID.

Standard web servers and cloud platforms may automatically process technical metadata such as IP address, TLS information, timestamps, and request size. We use this category of information only in the ordinary course of operating and securing the service, not to build individual marketing profiles about you.

## Notifications

When you turn on Notification Alerts (or leave granular alert types enabled) and grant the operating system’s notification permission, the App obtains an Expo push token and sends it, together with your on/off preferences for each alert category, to our Supabase Edge Function using the same publishable project key as other API calls. Tokens are stored in our database only so we can deliver the notifications you asked for.

Push delivery is relayed through Expo’s push notification service, which in turn uses Apple (APNs) on iOS and Google (FCM) on Android. Expo and those providers process technical identifiers needed to deliver messages; see their respective privacy notices for details.

If you turn off Notification Alerts, the App registers your choice with the server and stops associating a push token with delivery for that device install. You can withdraw consent at any time using the toggles in Settings or by revoking notification permission in the system settings for Factor Feed. Uninstalling the App removes local preferences; you may request deletion of server-side push rows by emailing support+factorfeed@signatureapps.app or via Contact Support in Settings if you need confirmation beyond uninstall.

## Subscriptions (Factor Feed Pro)

Factor Feed is free to use; an optional auto-renewing subscription, Factor Feed Pro, unlocks additional features. Purchases are processed by Apple's App Store and by [RevenueCat](https://www.revenuecat.com/privacy), which we use to validate receipts and manage subscription entitlement status. RevenueCat receives a device/app identifier and your purchase/subscription state; it does not receive your name, email, or payment card details, which are handled entirely by Apple. We do not sell or share this data with advertisers. See RevenueCat's own privacy policy for how it processes this information. You can view or cancel your subscription at any time in iOS Settings → your name → Subscriptions.

## Links and embedded browsing

Where the App opens external web pages (for example, news or feed links), those pages are opened in the system browser or an in-app browser session provided by the platform. Those sites are governed by their own privacy policies, not this Policy.

## Analytics and diagnostics

The production Factor Feed app distributed on the App Store and Google Play does not integrate third-party crash-reporting or behavioral analytics SDKs, and does not automatically send crash reports or usage analytics to us. If we add such a service in the future, we will update this Policy and the store listing before enabling it.

## Children’s privacy

The App is a general-audience financial information tool and is not directed at children under 13 (or the minimum age required in your jurisdiction). We do not knowingly collect personal information from children for targeted purposes. If you believe a child has provided personal information in a context we control, contact us at support+factorfeed@signatureapps.app or through Contact Support in Settings.

## International users

If you access the App from outside the United States, your information may be processed in the United States or other countries where our service providers operate. Those countries may have data protection laws that differ from those in your country.

## Your choices and retention

You may adjust many data-related behaviors inside the App (for example, which indicators to track, terminal categories, and theme) through Settings and related screens. Clearing cached queries or uninstalling the App removes locally persisted caches subject to operating-system behavior.

Our hosting providers may retain standard server and security logs in accordance with their own retention policies. We do not use those logs to build or maintain a personal profile of you within the App.

## Security

We use industry-standard transport security (HTTPS) for network calls. API keys that ship in the client are publishable keys scoped to our data proxy, not privileged database credentials. You should still treat your device as sensitive: anyone with access to an unlocked device may see cached economic data and preferences stored by the App.

## Changes to this Policy

We may update this Privacy Policy from time to time to reflect changes in the App, legal requirements, or data practices. When we make material changes, we will revise the Effective Date at the top of this Privacy Policy (currently May 13, 2026). Continued use of the App after an update constitutes acceptance of the revised Policy where permitted by law.

## Contact

For privacy questions or requests regarding this Policy, email support+factorfeed@signatureapps.app or use the Contact Support row in the App’s Settings screen (About section).

---

Readme: [https://www.signatureapps.app/factor-feed-readme](https://www.signatureapps.app/factor-feed-readme)

Privacy policy: [https://www.signatureapps.app/factor-feed-privacy](https://www.signatureapps.app/factor-feed-privacy)

© 2026 Factor Feed. All rights reserved.
