# Neon Memoir — Android release

Neon Memoir is an Android app from the [8-Bit Oracle](https://8bitoracle.com) archive. Each day it opens one archival image from the Kangxi court (1688–1722). You zoom in fixed steps and find text fragments, labelled ATTESTED (a documented fact with its source) or APOCRYPHAL (from a fictional Jesuit copyist's notebook). Built for the Solana Mobile "Clock In" hackathon.

This repository holds the release build only. The source is private.

## Install

1. Download `neon-memoir.apk` from the [latest release](../../releases/latest).
2. Open it on an Android phone (Android 8.0 or later) and allow installing from this source.

## Solana

- Cluster: devnet only.
- Day seed: a devnet blockhash, drawn as the day's hexagram.
- Filing: FILE EXAMINATION sends a Memo program transaction through Mobile Wallet Adapter (tested with Solflare). The wallet needs devnet SOL.
- The memo links to a Plum Blossom reading on app.8bitoracle.com, cast from the filing's block time.

For judges: INDEX → SHOW ALL DAYS (DEMO) opens all eight artifacts.

## Credits and AI disclosure

Archive images are public-domain scans from Wikimedia Commons. The cover portrait is AI-generated (an OpenAI image model). The copyist's voice is synthetic (ElevenLabs). Volume I's text was drafted with Claude and checked against the cited sources. The film "Timeline path: Binary" is by 8-Bit Oracle; its music is *Lofi Synthwave* by ZephiraMusic, Pixabay Content License.
