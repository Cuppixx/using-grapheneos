# Using GrapheneOS – A Daily Driver Experience

Welcome to Using GrapheneOS, a personal log and resource for anyone curious about what it’s like to use GrapheneOS as a daily driver.

While the web is full of reviews on social media, this repo aims to cut through some of the noise and give a realistic, user-level perspective. I’ll cover the open-source apps I rely on, the commercial software I haven’t found good FOSS replacements for (yet), the settings and tweaks I personally like, and even the small annoyances that come up along the way.

Whether you're considering switching to GrapheneOS, already made the jump, or just curious about using a privacy-focused, de-googled Android fork — this should help to get some insights.

## 🧭 What You’ll Find Here

- This repo is structured more like a growing journal than a formal review. Expect things like:
- 📦 A curated list of all the apps I use and what I use them for
- 🛠️ My personal GrapheneOS setup: settings, features, and configuration
- 💬 Honest notes on what works well and what doesn’t
- 🔄 Ongoing updates as I test alternatives, swap apps, or refine my usage
- 🚫 Gaps in the FOSS ecosystem where I still need to use proprietary apps
- 💡 Occasional tips, workarounds, and mini-guides based on experience

## 📦 Apps I Use – Overview

Here’s a quick breakdown of all the apps I currently use on my GrapheneOS device, what category they fall into, and what I use them for. This list includes both FOSS and proprietary apps.

### 🟩 Native GrapheneOS Apps

These are the system apps that come pre-installed with GrapheneOS. They're sandboxed, secure, and cover most basic functions.

- **App Store** – Used for installing trusted apps (via GOS's "Apps" app, including sandboxed Play Services)
- **Auditor** – Verifies device integrity and security
- **Calculator** – Lightweight, basic calculator
- **Camera** – Secure default camera app, though lacking features like document scanning
- **Clock** – Alarm, timer, stopwatch, and world clock
- **Contacts** – Local contact management
- **Files** – Basic file manager with storage access framework
- **Gallery** – View local media (photos, videos)
- **Info** – System and device information viewer
- **Messaging** – Basic SMS app (non-RCS)
- **PDF Reader** – View PDFs offline
- **Settings** – System settings and GrapheneOS features
- **Telephone** – Dialer and call management
- **Vanadium** – Hardened browser based on Chromium, optimized for privacy

### 🟩 Open Source 3rd-Party Apps

Chosen to replace proprietary tools or add functionality missing from GrapheneOS.

- **Aegis** – 2FA code manager; secure, open source alternative to Google Authenticator
- **AvesLibre** – Lightweight and privacy-friendly image/video viewer
- **Bitwarden** – Password manager; secure cloud sync with open source backend
- **FUTO Keyboard** – Privacy-respecting keyboard alternative; no network access
- **KDE Connect** – Cross-device sync and file sharing between Android and Linux desktops
- **Mastodon** – Decentralized social media client
- **NewPipe** – YouTube front-end with no ads, background playback, and downloads
- **Obtainium** – Auto-update FOSS apps from GitHub, F-Droid, etc. outside app stores
- **OpenReads** – Lightweight eBook/PDF reader (alternative to proprietary readers)
- **OpenScan** – Scan documents to PDF; chosen because the stock Camera app lacks scanning
- **OpenTracks** – GPS tracking for workouts and trips; fully offline
- **Orbot** – Tor routing for apps; useful for privacy or circumventing censorship
- **Organic Maps** – Offline maps and navigation; ideal for privacy-first users
- **Proton Calendar** – Encrypted calendar sync with Proton services
- **Syncthing-Fork** – Peer-to-peer file sync; local-first, no cloud needed
- **Termux** – Terminal emulator and Linux environment; powerful for scripting or sysadmin tasks
- **Thunderbird** – Full-featured email client; FOSS, cross-platform (note: Android version still evolving)
- **Twire** – Open source Twitch client; ad-free and privacy-respecting

### 🔒 Proprietary / Closed Source Apps

Used when no equivalent FOSS app meets functionality needs — trade-offs acknowledged.

- **Crunchyroll** – Streaming anime; no reliable FOSS front-end
- **Discord** – Communication app; unfortunately no fully featured open alternative
- **Fallout Shelter** – Mobile game; included for fun
- **Gwent** – Card game; proprietary but no open version exists
- **Joyn** – TV/streaming app for live content
- **KARDS** – Online WWII card game
- **Loxone** – Smart home control app; needed for existing home setup
- **Malwarebytes** – On-demand scanning for peace of mind (not always running)
- **Netflix** – Streaming video; no workaround for DRM content
- **Obsidian** – Markdown-based note-taking; syncs across devices (uses proprietary plugins)
- **Paypal** – Financial app; no practical alternative for certain payments
- **Play Games / Play Store** – Installed sandboxed via GOS to support games and some services (e.g. login in Pokemon Go)
- **Pokemon Go** – AR game; requires Google Play Services (sandboxed)
- **Spotify** – Music streaming; no full-featured FOSS client for offline/download
- **Tailscale** – Mesh VPN; used for remote access and secure networking
- **Teams** – Required for work communication; no compatible FOSS option
- **WhatsApp** – Used for social reasons (contacts, family); reluctantly used due to network effect
- **Banking App** – Proprietary app required for managing bank account
- **Breeze Weather** – Reliable weather app with good UI and data

## 🧠 Apps I Use - Thoughts

Let’s get a few things out of the way.

The default **GrapheneOS App Store** isn't really an "app store" in the traditional sense. Its main purpose is to update GrapheneOS system apps and optionally install sandboxed Google Play Services. Yes, you *can* install [Accrescent](https://accrescent.app/) through it — another FOSS app store — but personally, I’ve never been fully satisfied with either F-Droid or Accrescent.

That’s why I use **Obtainium**. While it's not technically a "store," it's more like a lightweight package manager that pulls APKs directly from trusted upstream sources like GitHub or GitLab. It gives me full control over updates and sources, without relying on middlemen.

As for some of the native apps:

- I’ve never had much use for the **Auditor** or **Info** apps.
- The default **Gallery** app is a rough experience — basic and clunky.
- In contrast, **Aves Libre** has become my go-to media viewer. It feels more like a desktop app, which is a vibe I also appreciate in the **Files** app.

Speaking of Files: one of the things I really like about GrapheneOS is that it doesn’t try to hide the file system. With the default **Files** app, you can easily browse the contents of your device without artificial limitations. That’s rare these days.

The rest of the built-in apps generally do their job well enough that I haven't felt the need to replace them.

Special mention goes to **Vanadium**, the hardened default browser. It strikes a great balance between usability and security. I haven’t felt the need to replace it with something like Brave or Firefox Hardened — those offer more features, sure, but they also come with more settings bloat. Vanadium just works, securely and comfortably.

Among the third-party FOSS apps, there’s a core group I consider essential for a security-hardened setup:

- **Aegis** – for managing 2FA codes securely
- **Bitwarden** – for password management
- **Malwarebytes** – for on-demand scanning (not always active)
- **Orbot** – for routing traffic through Tor when needed

These four cover a lot of bases when it comes to digital hygiene and peace of mind.

GrapheneOS doesn’t ship with voice input out of the box, and most keyboards either require network access or lack features. That’s why I use **FUTO Keyboard** — it offers offline speech-to-text, solid typing feel, and a fully local privacy model. It’s one of the few keyboards that hits the sweet spot of usability and privacy.



