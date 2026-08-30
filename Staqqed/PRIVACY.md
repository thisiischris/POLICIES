# Privacy Policy

**Last updated:** July 2026

Staqqed is a personal credit card wallet app. This page explains how your information is handled when you use it.

---

## The short version

**Your card data never leaves your phone.** Everything you enter — card details, balances, rewards, everything — stays in local storage on your device. There are no accounts to create and no servers Staqqed sends your card data to.

The only network activity in the app is processing an optional one-time purchase (see "In-app purchases" below), which is handled by Apple and our payments provider, RevenueCat — not by us.

---

## What you enter

When you add a card, you might fill in things like:

- The card name, bank, and network
- Your credit limit and current balance
- APR, annual fee, and payment due date
- Rewards rates and categories
- Sign-up bonus details
- Perks and credits
- The last four digits or expiration date (optional)

All of this lives only on your device. It is never transmitted anywhere.

---

## Where it's stored

Your card data is saved in your phone's private local storage (AsyncStorage). No other app can read it, and it never touches the internet.

If you delete the app, your data is deleted with it. You can also remove everything yourself from within the app at any time.

---

## Internet access

Staqqed's core wallet features work entirely offline — adding, editing, and viewing cards makes no network requests at all. There are no analytics, no crash reporting, and no ads.

The one exception is unlocking **Staqqed Lifetime** (see below), which requires a network connection to process the purchase and verify your entitlement.

---

## In-app purchases

Staqqed offers an optional, one-time "Lifetime" purchase that unlocks unlimited cards, data export/backup, the payoff calculator, and premium reminders. There is no subscription and no recurring charge.

This purchase is processed by the App Store and managed using **RevenueCat**, a third-party subscription/purchase platform. When you make or restore a purchase, RevenueCat receives an anonymous device/purchase identifier and your transaction receipt from Apple in order to verify and store your entitlement status. RevenueCat does not receive any of your card data — it only ever sees purchase-related information. See [RevenueCat's privacy policy](https://www.revenuecat.com/privacy) for details on how they handle that data.

If you never purchase Staqqed Lifetime, this SDK still initializes on launch to check whether you already own it (e.g. after reinstalling), which involves a network request to RevenueCat with the same anonymous device identifier — no card data is ever included.

---

## Face ID / biometric balance lock

Staqqed lets you hide balances and limits with one tap, and use Face ID (or your device's equivalent biometric) to reveal them again. This authentication happens entirely on-device through Apple/Android's system frameworks — Staqqed never receives, stores, or transmits your biometric data.

---

## Reminders and notifications

If you unlock Staqqed Lifetime, you can enable reminders for due dates, promo APR expiration, annual fees, rotating categories, and milestones. These notifications are scheduled and delivered entirely on your device using local (not push) notifications — nothing is sent to a server to generate or trigger them.

---

## Importing from a spreadsheet

When you import cards from an Excel or CSV file, the file is read directly on your device. Nothing in that file is sent to any server.

---

## Children

Staqqed is not intended for children under 13 and does not knowingly collect information from anyone in that age group.

---

## Changes to this policy

If anything here changes, the update will be noted in the app's release notes.

---

## Questions?

Reach out anytime at **support+staqqed@signatureapps.app**.

---

[README](https://www.signatureapps.app/staqqed-readme)
