<p align="center">
  <img src=".github/readme/icon.svg" width="128" height="128" alt="BLEAKFATE Android icon: a phone outline with a black hole on its screen, on a deep green tile">
</p>

<h1 align="center">BLEAKFATE for Android</h1>

<p align="center">
  <b>The BLEAKFATE VPN app for Android: sign in, press one button, renew without leaving the app.</b>
</p>

<p align="center">
  Our own Android client for BLEAKFATE VPN, built on the same Xray core that runs on our servers. Your account, subscription, devices and payments live in the app.
  <br><i>This repository holds the releases only: the source code is closed.</i>
</p>

<p align="center">
  <img alt="version: 0.8.5" src="https://img.shields.io/badge/version-0.8.5-3f7d6b?style=flat-square">
  <img alt="stage: beta" src="https://img.shields.io/badge/stage-beta-3f7d6b?style=flat-square">
  <img alt="platform: Android 7.0+" src="https://img.shields.io/badge/platform-Android%207.0%2B-2a5a4d?style=flat-square&logo=android&logoColor=white">
  <img alt="UI: Russian and English" src="https://img.shields.io/badge/UI-RU%20%2B%20EN-31566e?style=flat-square">
  <img alt="source: closed" src="https://img.shields.io/badge/source-closed-6b7280?style=flat-square">
</p>

<p align="center">
  <a href="https://github.com/MostViable/bleakfate-android/releases/latest/download/BLEAKFATE.apk"><b>Download BLEAKFATE.apk</b></a> ·
  <a href="README.ru.md"><b>Русская версия</b></a> ·
  <a href="https://bleakfate.com">bleakfate.com</a> ·
  <a href="https://t.me/BleakFateBot">@BleakFateBot</a> ·
  <a href="https://t.me/BleakFateSupportBot">Support</a>
</p>

<p align="center">
  <img src=".github/readme/screens/en/home-off.png" width="24%" alt="Home with the VPN off: a dark black hole and the Connect button">
  <img src=".github/readme/screens/en/home-on.png" width="24%" alt="Home with the VPN on: the black hole glows, connected through Smart Auto">
  <img src=".github/readme/screens/en/servers.png" width="24%" alt="Servers: Smart Auto and the list of countries">
  <img src=".github/readme/screens/en/settings.png" width="24%" alt="Settings: split tunneling, appearance, connection">
  <br><sub>Real screenshots of version 0.8.2: Home with the VPN off and on, Servers, Settings.</sub>
</p>

> [!NOTE]
> The app is in beta. It needs a BLEAKFATE subscription: sign in with the account you use in the bot or on the website, or paste your subscription link.

<p align="center">
  <a href="#install">Install</a> ·
  <a href="#check-the-file">Check the file</a> ·
  <a href="#updates">Updates</a> ·
  <a href="#what-it-can-do">What it can do</a> ·
  <a href="#privacy">Privacy</a> ·
  <a href="#license-and-credits">License and credits</a>
</p>

## Install

1. Download [`BLEAKFATE.apk`](https://github.com/MostViable/bleakfate-android/releases/latest/download/BLEAKFATE.apk) from the latest release.
2. Open the file. Android asks to allow installing apps from your browser or file manager: allow it for this installation.
3. Open BLEAKFATE and sign in through Telegram or with your email, or choose "I have a subscription link".

Requires Android 7.0 or newer (arm64-v8a or armeabi-v7a).

## Check the file

Every release has `BLEAKFATE.apk.sha256` next to the APK. All releases are signed with the same key; the SHA-256 of the signing certificate is:

```
b6fa737b90b114ed4144ee2f0c7d00559fcbc81fbe890f59636d3142e93c51f8
```

With the Android SDK: `apksigner verify --print-certs BLEAKFATE.apk` must show this digest. A file signed with any other key is not ours.

## Updates

Install a new release over the old one: your settings, servers and sign-in stay. Updating from inside the app is coming later; for now take the new APK from [Releases](https://github.com/MostViable/bleakfate-android/releases).

## What it can do

- **One button** to connect, and **Smart Auto**, which picks a working server for the network you are on.
- **Servers by country**, favourites, ping check and a speed test.
- **Split tunneling**: choose which apps go through the VPN.
- **Account in the app**: sign in through Telegram or email, see your subscription and devices, renew and pay (SBP, card, crypto).
- **Trusted Wi‑Fi networks** where the VPN switches off, modes such as Home or Work, a leak check.
- **Light and dark themes**, Russian and English.

## Privacy

No ads and no analytics. Error reports go to our server only if you allow them (Settings → Connection log); they hold event codes, the name of a crash, the app version and the phone model, never addresses, subscription links or keys. The speed test talks to `speed.cloudflare.com`. The full policy is on [bleakfate.com](https://bleakfate.com/legal/privacy/).

## License and credits

© MostViable. All rights reserved. You may download and use the app with a BLEAKFATE subscription; the source code is not published.

The app uses open-source components under their own licenses: [libXray](https://github.com/XTLS/libXray) (MIT) and [Xray-core](https://github.com/XTLS/Xray-core) (MPL-2.0, unmodified; source of the version used: [v26.10.31](https://github.com/XTLS/Xray-core/tree/v26.10.31)), [hev-socks5-tunnel](https://github.com/heiher/hev-socks5-tunnel) with its modules (MIT, lwIP under BSD-3-Clause), Kotlin, AndroidX and Jetpack Compose, OkHttp, ZXing (Apache-2.0). Full texts: [`THIRD_PARTY_NOTICES.txt`](THIRD_PARTY_NOTICES.txt) and in the app (About BLEAKFATE → Open source licenses).
