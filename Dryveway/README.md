# Dryveway

**Your garage, at a glance.** Dryveway is the vehicle-maintenance dashboard for anyone who's ever forgotten when the oil was last changed or missed a registration renewal. Add every car you own, log service in one tap, and let local reminders tell you what's due — before it becomes a problem. No account, no subscription, no cloud: everything lives on your phone.

A React Native (Expo) vehicle-maintenance dashboard — track multiple cars, log completed maintenance with one tap (odometer-confirmed), get advance notifications before anything is due, and keep a full service history with costs.

Built to the "Refined Blue" design handoff: 4px radii, Inter + JetBrains Mono type, light/dark themes, instrument-panel feel.

## Run it

```bash
npm install
npm start
```

`npm start` binds the dev server to the Tailscale IP (`100.101.236.104`) so the phone can connect over Tailscale — scan the QR with **Expo Go** (the project targets **Expo SDK 55** to match Expo Go 55.x). If the QR doesn't scan, open Expo Go and enter `exp://100.101.236.104:8081` manually.

Alternatives: `npm run start:lan` for plain LAN mode, `npm run web` for a quick desktop preview.

## Features

- **Garage home** — all vehicles with photo, mileage, and an "All good / N due" badge
- **Add Vehicle** — searchable Make → Model picker (bundled offline dataset of ~50 makes), plus free-type for anything missing; then year, mileage (required), nickname, VIN, plate, registration expiry
- **Car Detail** — mileage & registration stat cards, collapsible Service Timeline (every logged service with date, mileage, cost, notes + lifetime spend), and the Maintenance list with color-coded status (OK / DUE SOON / OVERDUE) and interval progress bars
- **One-tap logging** — tap an item → Mark Complete → confirm odometer (pre-filled), date, optional cost/notes
- **Auto or Manual scheduling** per item — interval math (miles and/or months, editable) or explicit next-due date/mileage
- **Registration & State Inspection** tracked as date-based items with expiry renewal flow
- **Per-car tracked items** — hide anything you don't want (e.g. no cabin filter on an EV); add custom items with their own intervals
- **Notifications** — local alerts N days before date-based dues; mileage-based alerts when an odometer update puts an item inside the alert window; configurable in Settings
- **Update mileage** — tap the Mileage stat card; sanity-check warns if the reading went down
- **Settings** — reminders on/off + lead time (days & miles), show/hide vehicle photos, System/Light/Dark theme
- **Photos** — tap the car photo header to pick one from your library
- Long-press a timeline entry to delete it; "…" menu on Car Detail for photo/mileage/delete vehicle

Everything persists locally (AsyncStorage) — offline-first, no account, no backend.

## Structure

```
App.tsx                 providers, fonts, navigation, notification rescheduler
src/theme/              light + dark design tokens ("Refined Blue")
src/data/               bundled make/model database, maintenance catalog + default intervals
src/store/              context + reducer + AsyncStorage persistence
src/logic/status.ts     derived due status / progress (never stored)
src/logic/notifications.ts  local notification scheduling
src/components/         Card, BottomSheet, Toggle, ProgressBar, icons, etc.
src/screens/            Garage, CarDetail, Settings + AddVehicle / LogMaintenance sheets
```

Note: local scheduled notifications work in Expo Go; remote push would require a development build (EAS).
