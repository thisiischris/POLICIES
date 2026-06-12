# Privacy Policy

**Stacked** is a personal credit card wallet manager. This policy describes how the app handles your data.

---

## Summary

Stacked does not collect, transmit, or share any personal information. All data you enter stays on your device.

---

## Data You Enter

When you add a card you may provide:
- Card name, issuer, and payment network
- Credit limit and current balance
- APR, annual fee, and due dates
- Rewards rates and categories
- Sign-up bonus details and spend tracking
- Perks, credits, and milestone information
- Card photos taken with your device camera (optional)
- Last four digits and expiration date (optional)

**None of this information is transmitted off your device.**

---

## How Data Is Stored

All card data is saved locally using `AsyncStorage` on your device. The data is stored in your app's private sandbox and is not accessible to other apps.

| Storage Key | Contents |
|---|---|
| `@cards/cards` | Your card records (JSON) |
| `@cards/theme-pref` | Your theme preference |
| `@cards/hide-balances` | Your balance-mask preference |

Data is deleted if you uninstall the app or use the "Delete all cards" option inside the app.

---

## Network Access

Stacked makes **no network requests**. There are no remote servers, no analytics, no crash reporting, and no cloud sync. The app works fully offline.

---

## Camera & Photo Library

If you add a card photo, the app requests permission to access your camera or photo library. Photos are stored locally on your device and are not uploaded anywhere.

---

## Excel Import

When importing cards from a spreadsheet, the file is read directly on your device using `expo-file-system`. The file contents are never sent to a server.

---

## Children

Stacked is not directed at children under 13 and does not knowingly collect information from children.

---

## Changes

This policy may be updated as the app evolves. Material changes will be noted in the app's release notes.

---

## Contact

For privacy questions, contact the developer at **sentbysignature@gmail.com**.
