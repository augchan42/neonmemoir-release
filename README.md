# Neon Memoir — Android release

Neon Memoir is an Android app from the [8-Bit Oracle](https://8bitoracle.com) archive. Each day it opens one archival image from the Kangxi court (1688–1722). You zoom in fixed steps and find text fragments, labelled ATTESTED (a documented fact with its source) or APOCRYPHAL (from a fictional Jesuit copyist's notebook). Built for the Solana Mobile "Clock In" hackathon on Radiants, and also submitted to the Colosseum World's Fair.

This repository holds the release build only. The source is private.

## Who can run it

- **Android only**, version 8.0 or later. There is no iPhone version.
- **On a Solana Seeker**, install it from the Solana dApp Store with one tap. You do not need the steps below.
- **On any other Android phone**, install the APK from this repository (sideload).

## Install on Android (sideload)

1. Download [`neon-memoir-v1.6.6-13.apk`](https://github.com/augchan42/neonmemoir-release/releases/download/v1.6.6/neon-memoir-v1.6.6-13.apk) (39.6 MB). Newer builds are on the [latest release](../../releases/latest) page.
2. Open the file on the phone. Android asks you to allow installs from the app that opened it, for example Chrome or Files. This permission is per app: you give it to that one app, not to the whole phone. You can turn it off again after the install.
3. Chrome can warn that the file "can harm your device", and Google Play Protect can say the app is unknown to it. Both warnings are normal for an app that is not from the Play Store. To continue, choose "Download anyway", then "Install anyway". If you are not sure, check the file first (see below).

### Check the file

The SHA-256 of `neon-memoir-v1.6.6-13.apk` is:

```
4c367c5a5f8df1756b9c89ee19e9f756a7a288768d2336edcf72c49bc4469517
```

On a computer: `sha256sum neon-memoir-v1.6.6-13.apk` (Linux), `shasum -a 256 neon-memoir-v1.6.6-13.apk` (macOS) or `certutil -hashfile neon-memoir-v1.6.6-13.apk SHA256` (Windows). Every release is signed with the same certificate, SHA-256 `2b43b32a940d2a5c2e5e03a73883f124d0b37ae30765a4d4da105c601ea37f63`, so a new version installs over an old one.

## Play without a wallet

You do not need a wallet to read the volume. You can open the day's image, zoom in, find the fragments and listen to the copyist. The day's seed comes from Solana devnet; if the phone is offline, the app uses a local seed.

A wallet is necessary only to **file** an examination: to record what you found as a memo on Solana devnet and get a reading.

## Set up a wallet to file

Filing uses devnet, Solana's test network. Devnet SOL is free and has no value.

1. Install [Solflare](https://solflare.com/) from the Play Store and create a wallet. Other Mobile Wallet Adapter wallets can also work, but Solflare is the tested one.
2. In Solflare's settings, change the network to **Devnet**.
3. Copy your wallet address. Get free devnet SOL from the [Solana faucet](https://faucet.solana.com/): paste the address, select devnet, and request a small amount. One filing costs much less than 0.01 SOL. The faucet has a daily limit; if it refuses, try again later.
4. In Neon Memoir, find at least one fragment, then tap FILE EXAMINATION. Solflare opens and asks you to connect and sign. After the transaction confirms, the page shows a FILED stamp that opens your reading.

## Solana

- Cluster: devnet only.
- Day seed: a devnet blockhash, drawn as the day's hexagram.
- Filing: FILE EXAMINATION sends a Memo program transaction through Mobile Wallet Adapter (tested with Solflare). The wallet needs devnet SOL.
- The memo links to a Plum Blossom reading on app.8bitoracle.com, cast from the filing's block time.

For judges: INDEX → SHOW ALL DAYS (DEMO) opens all eight artifacts.

## Credits and AI disclosure

Archive images are public-domain scans from Wikimedia Commons. The cover portrait is AI-generated (an OpenAI image model). The copyist's voice is synthetic (ElevenLabs). Volume I's text was drafted with Claude and checked against the cited sources. The film "Timeline path: Binary" is by 8-Bit Oracle; its music is *Lofi Synthwave* by ZephiraMusic, Pixabay Content License.
