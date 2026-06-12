# Factor Feed

Factor Feed is a serious, ad-free macroeconomic dashboard for U.S. and global economic data — built for people who actually want to read the numbers.

Every figure is live or marked "—". Nothing hardcoded, nothing fake.

— WHAT YOU GET —

• Inflation, interest rates, employment, GDP, housing, credit, federal debt, treasury yields, commodities, agriculture, sentiment, and money supply — all in one place.

• 40+ indicator detail pages, each with a chart, a plain-English explanation of why the number matters, and unique sub-widgets that break the indicator down (e.g. CPI by category, JOLTS labor flows, household wealth composition, the WTI–Brent–Dubai oil benchmark spread, the mortgage lock-in effect, the bond market's implied inflation forecast).

• 50 U.S. states — side-by-side comparisons of GDP, unemployment, median income, cost of living, poverty rate, minimum wage, and more.

• Global view — 40+ countries with live policy rates, 10-year yields, inflation, GDP growth, unemployment, debt-to-GDP, and central bank balance sheets. Tap any country to jump straight to its card.

• Terminal — categorised live-data terminal grouped by theme (Benchmark Yields, Labor Market, Housing & Credit, Consumer, Hard Assets, Agriculture, etc.) with a category stance pill that recomputes every refresh from the underlying live data — never a stale label.

• Macro Alerts — automated signals on the home screen flag yield-curve inversions, unemployment jumps, savings-rate stress, and other classic recession precursors as soon as the underlying series moves.

— DATA SOURCES —

FRED (St. Louis Fed), U.S. Treasury, BLS, BEA, U.S. Census Bureau, USDA NASS & ERS, NY Fed, World Bank, Eurostat, ECB, EIA, FDIC, FHFA, CNN Business Fear & Greed, [Alternative.me](http://Alternative.me), MetalpriceAPI, [worldgovernmentbonds.com](http://worldgovernmentbonds.com), and more. The full list with attribution is in Settings → Data Sources.

— ONE-TIME PURCHASE —

Pay $4.99 once. No subscriptions. No in-app purchases. No login. No ads. No analytics SDKs. No third-party trackers. We don't sell your data. The entire app unlocks immediately.

— PRIVATE BY DEFAULT —

No account creation. No behavioural or cross-app tracking. Optional push notifications for indicator alerts (off by default — only on if you enable them in Settings). Works offline using locally cached data.

— NOT INVESTMENT ADVICE —

Factor Feed is an informational app. There is no brokerage, no trading, no portfolio linking, no real-money transactions. Nothing here is a recommendation to buy, sell, or hold any security. Verify any number against the original source before making decisions.

Privacy policy: [https://github.com/thisiischris/FactorFeedApp/blob/main/PRIVACY.md](https://github.com/thisiischris/FactorFeedApp/blob/main/PRIVACY.md)

Support: [signatureappssupport+factorapp@gmail.com](mailto:signatureappssupport+factorapp@gmail.com)

## About Factor Feed

> Factor Feed turns the firehose of U.S. economic data into a clean, glanceable picture. Track inflation, interest rates, jobs, housing, agriculture, debt, and market sentiment — all in one place, refreshed from trusted official sources, and organized exactly the way you want. Compare all 50 states, see how the U.S. stacks up globally, and dive into any indicator for the full story in plain English. Whether you're an investor, a student, or simply economically curious, Factor Feed helps you understand where the economy is headed — without the jargon.

## Requirements

- Node.js (LTS recommended)
- [Expo CLI](https://docs.expo.dev/get-started/installation/) / `npx expo` as used in scripts
- For device testing: Expo Go or a **development build** (`expo-dev-client`)

## Install

```bash
npm install
```

(Or use your preferred package manager if you keep lockfiles in sync.)

## Run locally

```bash
npm run start
```

Starts Metro with **tunnel** mode (see `package.json`). Use the Expo Dev Tools QR code or terminal shortcuts to open iOS simulator, Android emulator, or web.

- **Web only:** `npm run start-web`
- **Lint:** `npm run lint`

## EAS environments

If you use [EAS Environment Variables](https://docs.expo.dev/eas/environment-variables/), pull them for a given profile:

```bash
npm run eas:env:pull:dev
npm run eas:env:pull:preview
npm run eas:env:pull:production
```

## Project layout (high level)


| Path              | Role                                                    |
| ----------------- | ------------------------------------------------------- |
| `app/`            | Screens and navigation (expo-router file-based routes)  |
| `components/`     | Reusable UI                                             |
| `providers/`      | React context (theme, query cache, notifications, etc.) |
| `hooks/` / `lib/` | Data hooks, formatting, API clients                     |


## Contact & support

If you experience any issues with the app or have questions about anything else, please reach out at [signatureappssupport+factorapp@gmail.com](mailto:signatureappssupport+factorapp@gmail.com).

## License

Private / not for redistribution unless the repository owner says otherwise.