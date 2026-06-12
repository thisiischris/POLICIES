# Stacked

A personal credit card wallet manager for iOS and Android. Track every card in your wallet — rewards rates, APR, credit limits, balances, fees, payment due dates, sign-up bonuses, and perks — all in one place, entirely on device.

---

## Features

### Wallet View
- Swipeable card stack and compact list view
- Search and filter by network, usage (personal/business), reward category, or favorites
- Gesture-driven card navigation with smooth morph transitions

### Card Tracking
- **Rewards** — per-category earn rates (dining, groceries, gas, travel, and 9 more)
- **Rotating categories** — track quarterly 5% categories with spend caps
- **APR** — purchase APR, intro/promo APR windows, balance transfer rates
- **Credit limits & balances** — statement balance, credit limit, utilization
- **Due dates & statement closing** — monthly calendar reminders
- **Annual fees** — track and compare across your portfolio
- **Sign-up bonus tracker** — spend requirement, deadline countdown, logged transactions
- **Milestone rewards** — annual free nights, spend thresholds, holding benefits
- **Perks & credits** — travel credits, Uber Cash, statement credits (annual/monthly/quarterly)

### Portfolio Overview
- Aggregate stats: total credit, total balance, utilization, annual fees
- APR breakdown across all cards
- Expiring soon and grace period alerts

### Import
- Import cards from a structured Excel (.xlsx) spreadsheet via the Import Wizard

### Privacy
- **Balance masking** — one tap hides all balance and limit values across the app
- **100% local** — no accounts, no servers, no network requests

### Appearance
- Light, dark, and system-auto themes
- Bundled card art for 60+ popular cards

---

## Tech Stack

| Layer | Technology |
|---|---|
| Framework | Expo SDK 55 / React Native 0.83.6 |
| Language | TypeScript 5.9.2 |
| Navigation | React Navigation v7 (native-stack) |
| Animations | React Native Reanimated 4 + Gesture Handler |
| Storage | AsyncStorage (on-device only) |
| Import | expo-document-picker + xlsx |
| UI | expo-linear-gradient, react-native-svg, @expo/vector-icons |

---

## Getting Started

### Prerequisites
- Node.js 18+
- Expo CLI (`npm install -g expo-cli`)
- Expo Go app on your iOS or Android device, or a simulator

### Install & Run

```bash
git clone <repo-url>
cd StackedApp
npm install
npm start          # starts Metro bundler
```

Scan the QR code with Expo Go or press `i` / `a` for iOS / Android simulator.

### Available Scripts

| Command | Description |
|---|---|
| `npm start` | Start Metro (LAN) |
| `npm run ios` | Run on iOS simulator |
| `npm run android` | Run on Android emulator |
| `npm run web` | Run in browser |

---

## Project Structure

```
src/
  screens/          # HomeScreen, AddEditScreen, DetailScreen
  components/       # CardWalletStack, CreditCardVisual, OverviewSheet, …
  addCard/          # Multi-step add card flow
  navigation/       # Transition helpers (morph, hero, FAB)
  data/             # Card database (issuer defaults, logos)
  hooks/            # Shared React hooks
  CardsContext.tsx  # Global card state + AsyncStorage persistence
  ThemeContext.tsx  # Theme + balance-mask state
  types.ts          # Core TypeScript types
assets/
  cards/            # Bundled card face art (60+ cards)
  banks/            # Bank logo assets
```

---

## Data & Storage

All data is stored locally using `@react-native-async-storage/async-storage`. Nothing leaves the device.

| Key | Contents |
|---|---|
| `@cards/cards` | JSON array of all card records |
| `@cards/theme-pref` | `"light"`, `"dark"`, or `"system"` |
| `@cards/hide-balances` | Boolean balance mask preference |

---

## License

Private — all rights reserved.
