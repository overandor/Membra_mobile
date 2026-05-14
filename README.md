# Membra Mobile

**Membra Mobile is the owner-side proof app namespace for MEMBRA Labs and the MEMBRA Proof Network.**

It turns real-world owner actions into verified proof events that can activate campaigns, create audit records, and unlock reward eligibility.

## Company Context

- Company: **MEMBRA Labs**
- Flagship product: **MEMBRA Proof Network**
- Module: **Membra Mobile**
- Category: owner proof app, campaign offer app, QR/NFC scanner, proof-photo capture

## One-Line Thesis

Membra Mobile turns owner actions in the physical world into verified proof events.

## Product Role

Membra Mobile is the owner-facing app layer for:

- owner onboarding
- surface registration
- vehicle, window, wearable, bag, and sign capture
- campaign offer review
- media-kit receipt confirmation
- proof photo submission
- QR/NFC test scans
- reward status display
- claim/dispute submission
- profile and payout readiness

## Core Screens

1. home dashboard
2. register asset
3. campaign offers
4. media kit receipt
5. submit proof
6. QR/NFC scanner
7. reward status
8. claims and support
9. profile and payout readiness

## Proof Law

- no proof photo → no activation
- no receipt confirmation → no active media kit
- no approved proof → no reward eligibility
- no audit record → no trusted state change

## Integration Map

| Repo | Mobile Relationship |
|---|---|
| `overandor/Membra_api` | receives owner, asset, proof, and campaign actions |
| `overandor/Membra_ads` | defines campaign, media-kit, asset, and proof logic |
| `overandor/Membra_proofbook` | records proof hashes and audit records |
| `overandor/Membra_wallet` | tracks reward and payout readiness |
| `overandor/membra-qr-gateway` | displays dashboard analytics and public/private proof state |
| `overandor/Membra_admin-` | reviews owner-submitted proof and claims |
| `overandor/Membra_demo_data` | provides sample owner workflows for demo mode |

## Safety Rules

- no sensitive identity documents in public proof views
- no private location exposure without consent and access controls
- no reward display that implies guaranteed payout before review
- no upload flow without evidence retention policy
- no proof deletion without audit policy

## Productization Priority

This repo should become an Expo or React Native owner app after the backend and dashboard demo are stabilized.

Recommended build order:

1. static Expo shell
2. register asset screen
3. campaign offer screen
4. media-kit receipt screen
5. proof photo capture screen
6. QR/NFC scanner screen
7. reward status screen
8. API integration with `Membra_ads` or `Membra_api`

## Current Stage

Owner mobile workflow scaffold and product charter. Not yet a production mobile application.