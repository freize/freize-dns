<div align="center">

# 🛡️ FreizeDNS — Official Website

**Landing page and release hub for FreizeDNS — a secure, customizable DNS-over-HTTPS client for Android & Android TV.**

[![Website](https://img.shields.io/badge/Website-app.freize.net-06b6d4?style=for-the-badge&logo=googlechrome&logoColor=white)](https://app.freize.net)
[![Platform](https://img.shields.io/badge/Android-5.0%2B-3DDC84?style=for-the-badge&logo=android&logoColor=white)](#)
[![Android TV](https://img.shields.io/badge/Android%20TV%20%2F%20Google%20TV-Supported-3b82f6?style=for-the-badge&logo=android&logoColor=white)](#)
[![Root](https://img.shields.io/badge/Root-Not%20Required-8b5cf6?style=for-the-badge)](#)

</div>

---

## ✨ About FreizeDNS

FreizeDNS is a lightweight, native DNS client designed for Android smartphones, tablets, and Android TV / Google TV devices.

- **Encrypted DNS-over-HTTPS (DoH):** Protects DNS queries from ISP tracking and tampering.
- **Android TV & Wide-Screen Ready:** Adaptive interface built for large displays and remote control navigation.
- **Built-in Firewall & App Exclusions:** Control network access per app without root privileges.
- **IPv6 Leak Protection:** Built-in IPv6 blocking for consistent privacy.
- **Trusted Wi-Fi:** Automatically pauses filtering on trusted home networks.
- **Local DNS Lists & Authorization:** Real-time local list processing and Freize ID support.
- **Bilingual UI:** Full English and Russian localization.

---

## 🌐 Website Features

- **Zero-Build Static Architecture:** Single `index.html` powered by Tailwind CSS (CDN) and vanilla JavaScript.
- **Auto Language Detection (EN / RU):** Detects browser language automatically with persistent `localStorage` switching.
- **Dynamic Version & Changelog:** Pulls the latest release version, localized changelog, and Universal APK URL directly from `/update-ng.json`.
- **Smart APK Architecture Detection:** Uses User-Agent Client Hints and Android heuristics to detect the visitor's device and highlight the best-matching APK (`ARM64`, `ARM32`, `x86_64`, `x86`, or `Universal`).
- **Screenshot Gallery & Lightbox:** Responsive horizontal album with keyboard navigation, touch swipe support, and full-screen preview.

---

## 📁 Repository Structure

```text
freize-dns/
├── index.html              # Main landing page
├── update-ng.json          # App release metadata & localized changelogs
├── screenshot/             # App screenshots for the gallery
│   ├── list.json           # Image manifest (required for GitHub Pages)
│   ├── 1.jpg
│   ├── 2.jpg
│   └── 3.jpg
└── updates/                # APK release builds
    ├── FreizeDNS-universal-release.apk
    ├── FreizeDNS-arm64-v8a-release.apk
    ├── FreizeDNS-armeabi-v7a-release.apk
    ├── FreizeDNS-x86_64-release.apk
    └── FreizeDNS-x86-release.apk
