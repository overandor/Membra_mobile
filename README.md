# Membra Mobile

Membra Mobile is the owner-side proof app for the MEMBRA ecosystem.

It lets owners register physical ad surfaces, receive campaign offers, confirm media-kit receipt, capture proof photos, submit location-backed placement proof, scan QR/NFC tags, and track reward status.

## One-line thesis

Membra Mobile turns real-world owner actions into verified proof events that can activate campaigns and unlock reward eligibility.

## Product role

- Owner onboarding
- Surface registration
- Vehicle, window, wearable, bag, and sign capture
- Campaign offer review
- Media-kit receipt confirmation
- Proof photo submission
- QR/NFC test scans
- Reward status display
- Claim/dispute submission

## Core screens

1. Home dashboard
2. Register asset
3. Campaign offers
4. Media kit receipt
5. Submit proof
6. QR/NFC scanner
7. Reward status
8. Claims and support
9. Profile and payout readiness

## Integration map

- `Membra_api` receives owner, asset, proof, and campaign actions.
- `Membra_ads` defines campaign and media-kit logic.
- `Membra_proofbook` records proof hashes.
- `Membra_wallet` tracks reward and payout readiness.
- `membra-qr-gateway` displays dashboard analytics.

## Proof law

No proof photo means no activation.

No receipt confirmation means no active media kit.

No approved proof means no reward eligibility.

## Current stage

Owner mobile workflow scaffold. Next step is a lightweight Expo/React Native app shell using the API flows documented in this repo.
