# Privacy Policy

_Last updated: 2026-11-20_

Dryveway is an offline-first vehicle maintenance tracker. This policy explains what data the app uses and, just as important, what it doesn't.

## Data storage

All data you enter — vehicles, mileage, service history, notes, costs, and settings — is stored locally on your device using AsyncStorage. Dryveway has no backend server and no user accounts. Your data is never transmitted off your device, and we (the developers) have no access to it.

## Photos

If you attach a photo to a vehicle, Dryveway accesses your device's photo library only when you tap to pick an image. Photos are stored locally alongside your other vehicle data and are never uploaded anywhere.

## Location

When you log or edit a service, you can tap to fill in the service location from where you are. Only then does Dryveway ask for location access "While Using the App", read your current position once, and convert it to a street address using your device's built-in geocoding service (on iOS, Apple's). The resulting address is saved with that service record on your device; your coordinates are not stored.

Dryveway never accesses your location in the background and does not use motion or fitness data.

## Mileage estimates

If you turn on Estimate mileage for a vehicle, Dryveway projects that vehicle's odometer from the driving rate you enter (miles or kilometers per year or month) and your last recorded reading, so maintenance can come due between updates. This is simple arithmetic done on your device — it does not track your driving, location, or movement.

## Notifications

Dryveway schedules local, on-device notifications to remind you about upcoming maintenance and registration renewals, and (unless you turn it off in Settings) a weekly reminder to update your mileage. These reminders are generated and delivered entirely on your phone — no notification content or scheduling data is sent to any external service.

## Backup and export

Dryveway can export your data to a CSV file, which you choose to save or share using your device's standard share sheet (for example, to email it to yourself, save it to a cloud-synced folder, or AirDrop it). This only happens when you tap "Export data" — Dryveway itself never sends this file anywhere.

If Auto Backup is turned on, Dryveway silently keeps a single CSV file (and your vehicle photos) up to date in the app's own document storage. On iOS, this file and your photos are visible in the Files app under On My iPhone → Dryveway, which lets you access, copy, or move them yourself — but Dryveway does not transmit them anywhere on its own.

## Official recall checks

Tapping "Check official recalls" in a vehicle's Glovebox sends your saved VIN (or year, make, and model if no VIN is saved) to the public NHTSA recall database to look up that vehicle's recalls. This only happens when you tap that button — Dryveway never checks recalls in the background.

## Vehicle and maintenance data lookups

When you add or edit a vehicle, Dryveway may look up the exact model names for the make and year you chose from the public NHTSA vehicle database. Only the make and model year are sent.

Dryveway also periodically downloads its catalog of recommended maintenance intervals from a public file hosted on GitHub, so intervals can be corrected without an app update. This is a plain file download — no vehicle or personal data is included.

## Affiliate links

A few screens include optional outbound links to other sites: a parts search on maintenance items and an OBD-II scanner link on the Fault Codes screen (via Amazon Associates), and a vehicle history report link in the Glovebox (via VinspectorAI). These are plain links that only open when you tap them — Dryveway doesn't send any vehicle or personal data through them, and only earns a commission if you follow one and complete a purchase. Once you leave the app through one of these links, the destination site's own privacy policy applies.

## Third parties

Dryveway does not integrate with analytics, advertising, or crash-reporting services, and does not share data with any third party on its own. The only outbound network requests are the ones described above: converting your location to an address when you ask it to, NHTSA model and recall lookups, the maintenance-interval catalog download, and affiliate links you explicitly tap. As with any internet request, the services receiving them can see your device's IP address. Your vehicles, service history, notes, and photos never leave your device.

## Deleting your data

Uninstalling the app removes all locally stored data. There is no account to delete because none is created.

## Changes to this policy

If Dryveway's data practices change (for example, if a future version adds optional cloud sync), this policy will be updated to reflect that before the change ships.

## Contact

Questions about this policy, or about the app in general, can be sent to **support+dryveway@signatureapps.app**.

## About the app

[Readme](https://www.signatureapps.app/dryveway-readme)
