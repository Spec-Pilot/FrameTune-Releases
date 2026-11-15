# 📺 FrameTune Suite — Official Releases

<div align="center">

[![Latest Release](https://img.shields.io/github/v/release/Spec-Pilot/FrameTune-Releases?style=for-the-badge&color=0284c7&label=Latest%20Release)](https://github.com/Spec-Pilot/FrameTune-Releases/releases/latest)
[![Platform](https://img.shields.io/badge/Platform-Android%20TV%20%7C%20Google%20TV%20%7C%20Fire%20TV-38bdf8?style=for-the-badge&logo=android)](https://frametune.fyi/tv.html)
[![Trackers](https://img.shields.io/badge/Trackers-ZERO%20%2F%200%25-10b981?style=for-the-badge&logo=adblock)](https://frametune.fyi/privacy-tv.html)
[![Telemetry](https://img.shields.io/badge/Telemetry-None%20(100%25%20Private)-10b981?style=for-the-badge)](https://frametune.fyi/privacy-tv.html)
[![Website](https://img.shields.io/badge/Website-frametune.fyi-38bdf8?style=for-the-badge&logo=googlechrome)](https://frametune.fyi)

**The privacy-first, ad-free Android TV launcher, intelligent streaming companion, and low-latency mobile remote controller.**

[🌐 Official Website](https://frametune.fyi) • [📺 TV Suite Guide](https://frametune.fyi/tv.html) • [🔒 Privacy & Refund Policy](https://frametune.fyi/privacy-tv.html) • [❓ FAQ & Setup](https://frametune.fyi/faq.html) • [📥 Downloads](#-downloads--installation)

</div>

---

## 🛡️ Privacy First: Zero Trackers, Zero Monitoring, Zero Sharing

> **Your television, your data, your privacy.**  
> FrameTune is engineered from the ground up with a strict **zero-data collection architecture**.

* 🚫 **No Trackers or Analytics SDKs:** FrameTune contains **ZERO** tracking libraries, advertising IDs, or telemetry SDKs. We do not bundle Google Analytics, Firebase Analytics, Crashlytics, Mixpanel, AppsFlyer, or Facebook SDKs.
* 🚫 **No Activity Monitoring or Logging:** FrameTune does **NOT** monitor, log, or track what you watch, how long you stream, what search terms you enter, or what apps you launch.
* 🚫 **No User Data Sharing or Selling:** We do **NOT** collect, store, transmit, profile, or sell any user information or viewing habits to any third parties, advertisers, or brokers.
* 🔒 **100% Local On-Device Operation:** All UI automations, commercial muting, skip triggers, and DNS filtering operate strictly in volatile RAM on your television hardware and are discarded in milliseconds.
* 🏠 **Local Network Security:** Communication between the FrameTune Mobile Remote and TV occurs solely over your local home network (or offline Bluetooth HID), protected by ephemeral 6-digit PIN pairing and local cryptographic tokens.

For complete details, read our official [TV & Remote Privacy Policy](https://frametune.fyi/privacy-tv.html).

---

## 📥 Downloads & Installation

Download the latest signed release APKs directly below:

| Application | Target Hardware | Requirements | Direct Download |
|:---|:---|:---|:---|
| **FrameTune TV** | Android TV, Google TV, Fire TV, TV Boxes | Android 8.0+ (API 26+) | [⬇️ `FrameTune-TV.apk`](https://github.com/Spec-Pilot/FrameTune-Releases/releases/latest/download/FrameTune-TV.apk) |
| **FrameTune Remote** | Android Smartphones & Tablets | Android 7.0+ (API 24+) | [⬇️ `FrameTune-Remote.apk`](https://github.com/Spec-Pilot/FrameTune-Releases/releases/latest/download/FrameTune-Remote.apk) |

👉 **[Browse All Releases & Release Notes](https://github.com/Spec-Pilot/FrameTune-Releases/releases)**

---

## 📺 FrameTune TV Launcher

**A fast, elegant, bloat-free TV home launcher designed for television lovers.**

Modern smart TV home screens (Android TV, Google TV, Fire TV) have become cluttered with full-screen sponsored advertisements, forced video recommendations, sluggish animations, and continuous background tracking. 

FrameTune TV replaces that bloated experience with a high-performance, tvOS-inspired Leanback home launcher that puts your installed apps and personal entertainment first:

### 🌟 Key Launcher Highlights:
* **Ad-Free Obsidian Slate Theme:** Clean, high-contrast dark aesthetic with specular white focus outlines and dynamic 1.10x elevation card scaling. No sponsored banners, no forced ads, and no unwanted autoplay videos.
* **Direct Boot Persistence (`directBootAware="true"`):** Starts instantly on TV reboot or power-on. Runs seamlessly in the background across restarts without needing a PC or ADB connection.
* **Dynamic App Drawer & Custom Sorting:** Automatically detects and displays every installed app using `QUERY_ALL_PACKAGES`. Easily organize and rearrange your favorite streaming apps using the TV remote or mobile companion.
* **Two-Column Master-Detail Navigation:** 
  * *Left Column:* Quick-switch between streaming platforms (Netflix, Prime Video, JioHotstar, YouTube, Sony LIV, ZEE5, MX Player, Viki), inputs, and built-in system tools.
  * *Right Column:* Dynamic automation cards showing per-app toggles, recent actions, and launch shortcuts.
* **Top Status Header & Quick Settings:** Instant status pills for Wi-Fi, Bluetooth, Network Shield, Mesh Tunnel, TV Settings, and Launcher Quick Settings with smooth D-pad chaining.
* **Integrated TV Maintenance & Diagnostics:**
  * **TV Storage Cleaner:** 1-click cache purge to free up TV flash memory.
  * **TV Speed Tester:** Real-time download/upload network speed benchmarking directly on your TV.
  * **Diagnostics Dashboard:** Monitor live CPU load, RAM utilization, and system uptime.
  * **Standby Microphone Sentinel:** Audits smart TV background activity and warns you if the TV microphone or telemetry processes activate during sleep mode.
* **4K Ambient Cinematic Screensaver:** Curated ultra-high-definition wallpapers (NASA, USGS, NOAA, CC0 public domain) with a live clock and hyper-local weather forecast powered by Open-Meteo.
* **Mobile Media Hub Streamer:** Connect a spare phone via high-speed USB tethering (RNDIS) or Wi-Fi to stream 4K video backdrops and photo carousels directly to your TV backdrop with zero TV storage usage.

---

## ⚡ Intelligent Streaming Automations

FrameTune TV runs alongside your official streaming applications (untouched and unmodified) using standard Android `AccessibilityService` and `AudioManager` APIs to eliminate streaming friction:

* **Smart Commercial Silencing:** Automatically mutes TV audio (`STREAM_MUSIC`) the instant an unskippable video commercial or countdown timer begins. Restores volume automatically when content resumes, protected by a fail-safe **2-second watchdog timer** so audio is never left muted.
* **Native Button Auto-Skipping:** Intelligently detects and clicks "Skip Intro", "Skip Recap", "Skip Ad", and "Next Episode" prompts without you having to reach for the remote.
* **Amazon Prime Video Visual Detector:** Custom visual scanner for Prime Video's C++/OpenGL Ignite rendering engine to auto-trigger Skip Intro and "Next Up in X" via synthetic center click.
* **Hotstar Smart Ad Fast-Forward & Speed Restoration:** Fast-forwards ads at 4.0x where unskippable, and smoothly restores playback speed to 1.0x with a state-locked safety window before normal DRM movie playback resumes.
* **Movie End Time HUD:** Displays a sleek glassmorphic overlay showing the exact wall-clock finish time (e.g., `Ends at 10:45 PM • 1h 15m remaining`). Dynamically adapts to custom playback speeds and remains visible during pause.
* **Per-App Ad Skip Mode:** Toggleable via physical TV remote (**Double-tap DOWN** then **Double-tap UP** within 3 seconds) to drop ad delivery connections via a local TUN sinkhole while leaving video streams untouched.
* **Local Network Shield (Zero-Latency DNS Sinkhole):** Intercepts port 53 DNS queries via a local `/32` sinkhole, blocking advertising and telemetry domains with 0% video buffering overhead. Includes 8 pre-loaded presets (AdGuard, Control D, NextDNS, Cloudflare 1.1.1.1, Quad9, Google) and custom IPv4 entry.

---

## 📱 FrameTune Remote Mobile Companion

Transform your Android smartphone into the ultimate precision TV controller with dual simultaneous connection modes:

* **Bluetooth HID Remote Mode (Works 100% Offline):** Registers your phone as a native USB-IF HID keyboard and consumer remote. Wakes the TV from deep standby sleep via hardware interrupt and controls basic functions (Power, D-Pad, Volume, Mute, Home, Back) without requiring Wi-Fi.
* **Local Wi-Fi Server Mode (Port 8765):** Connects simultaneously over local Wi-Fi with secure 6-digit PIN pairing and 256-bit token authentication to unlock advanced streaming features.
* **Tri-Mode D-Pad Cockpit:**
  * **🔘 Arrows Mode:** Discrete directional taps with 3-stage seek acceleration (100s/s → 133s/s → 200s/s).
  * **🕹️ Joystick Mode:** Radial thumbstick with snap-back physics and tap-for-OK.
  * **🖱️ Fluid Touchpad & TV Cursor Overlay:** 250dp tactile surface driving a hardware-accelerated 60fps cyan pointer on your TV screen with double-tap Enter and visual click ripple.
* **Direct Smartphone Typing:** Type on your phone's virtual keyboard to insert text directly into active TV search bars and password fields.
* **Live Interactive Media Scrubber:** Real-time playback telemetry (`positionMs`, `durationMs`, `speed`, `title`) streamed directly to your phone without triggering DRM blackouts. Features touch-freeze scrubbing and instant `SEEK_TO`.
* **3-Tier Media Transport Deck:** Discrete ±30s and 15m jumps, hero Play/Pause card, and continuous playback speed control (`0.25x` to `8.00x` with ±0.05x precision steppers).
* **Installed TV App Launcher:** Browse and launch installed TV applications directly from the phone with custom drag-and-drop ordering.
* **TV Quick Tools:** TV Task Manager (view and terminate background processes), Parental Controls (daily screen time limits and app locks), and Standby Surveillance Audit.

---

## 🌐 Home Mesh Relay & Hotel Travel Tunnel (Optional)

Turn your primary living room TV into a secure, encrypted residential gateway on UDP port 51820:

* **Bypass Hotel Geoblocks:** While traveling abroad or staying at hotels, route your mobile or travel TV streaming traffic securely through your home residential broadband to eliminate regional blackouts and datacenter VPN bans.
* **Zero-Config Router Port Forwarding:** Uses UPnP IGD and RFC 6886 NAT-PMP to open UDP port 51820 automatically without manual router configuration.
* **Modern WireGuard-Style Cryptography:** Pure Kotlin RFC 7748 Curve25519 (X25519) key exchange + ChaCha20-Poly1305 AEAD symmetric encryption.
* **Air-Tight Egress Security:** Blocks internal RFC 1918 private subnets to prevent guest devices from accessing home LAN resources (NAS, router admin, security cameras).

---

## 🚀 1-Step Setup Guide

Installing FrameTune TV requires **zero PC or ADB commands**:

1. **Install the APK:** Transfer `FrameTune-TV.apk` to your TV via USB flash drive or install it using the **Downloader** app directly on Android TV / Fire TV.
2. **Launch FrameTune TV:** Open the app from your TV launcher.
3. **1-Step Setup:** 
   * A prompt will appear: *"1-Step TV Setup Required: Enable FrameTune TV Service"*.
   * Press **OK** on your TV remote to open Android TV's Accessibility Settings.
   * Select **FrameTune TV Observer** and toggle it to **ON**.
4. **Pair the Mobile Remote (Optional):**
   * Install `FrameTune-Remote.apk` on your Android smartphone.
   * Ensure both devices are on the same Wi-Fi network (or pair via Bluetooth).
   * Enter the 6-digit PIN displayed on your TV screen to pair.
5. **Done!** FrameTune is now fully active and will remain permanently active across all TV restarts and reboots.

---

## 📋 Compatibility

| Feature | Supported Operating Systems & Devices |
|:---|:---|
| **FrameTune TV (`:app`)** | Android TV 8.0+ (Oreo, API 26) through Android 14+ (API 34+)<br>• Google TV (Chromecast with Google TV, Sony Bravia, TCL, Hisense, Philips)<br>• Fire OS 7+ (Fire TV Stick 4K, Fire TV Cube)<br>• AOSP Android TV Boxes (Nvidia Shield TV, Xiaomi Mi Box) |
| **FrameTune Remote (`:remote`)** | Android 7.0+ (Nougat, API 24) through Android 14+ (API 34+)<br>• All Android smartphones and tablets |

---

## 🔗 Official Links & Resources

* 🌐 **Website:** [https://frametune.fyi](https://frametune.fyi)
* 📺 **TV Section:** [https://frametune.fyi/tv.html](https://frametune.fyi/tv.html)
* 🔒 **Privacy Policy (TV & Remote):** [https://frametune.fyi/privacy-tv.html](https://frametune.fyi/privacy-tv.html)
* ❓ **FAQ & Help:** [https://frametune.fyi/faq.html](https://frametune.fyi/faq.html)
* 💬 **Support:** [https://frametune.fyi/support.html](https://frametune.fyi/support.html)
* 📦 **Release Repository:** [https://github.com/Spec-Pilot/FrameTune-Releases](https://github.com/Spec-Pilot/FrameTune-Releases)

---

<div align="center">
  <sub>Built with ❤️ for a cleaner, faster, privacy-first television experience.</sub>
</div>
