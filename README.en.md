<p align="center">
  <a href="README.md">Русский</a> · <b>English</b>
</p>

<p align="center">
  <img src="media/app-icon.png" alt="SubsTrack" width="144" />
</p>

<h1 align="center">SubsTrack</h1>

<p align="center">A subscription, payment, and reminder tracker for Android and the web.</p>

<p align="center">
  <a href="https://substrack.top"><b>Open website</b></a>
  &nbsp;·&nbsp;
  <a href="https://github.com/svllvsxprod/substrack-releases/releases/latest"><b>Download APK</b></a>
  &nbsp;·&nbsp;
  <a href="#installation"><b>Installation</b></a>
</p>

<p align="center">
  <img alt="Android 7+" src="https://img.shields.io/badge/Android-7.0%2B-3DDC84?style=for-the-badge&amp;logo=android&amp;logoColor=white">
  <img alt="Web" src="https://img.shields.io/badge/Web-substrack.top-2F6DF6?style=for-the-badge&amp;logo=googlechrome&amp;logoColor=white">
  <img alt="RU and EN" src="https://img.shields.io/badge/locales-RU_%C2%B7_EN-7657F6?style=for-the-badge">
  <img alt="Release 0.1.6" src="https://img.shields.io/badge/release-0.1.6-18A66A?style=for-the-badge">
</p>

## About

SubsTrack keeps recurring expenses in one place and shows which payments are paid, pending, skipped, or overdue. Multiple subscriptions to the same service can have distinct accounts, prices, and billing schedules.

The website and Android app use the same account. The interface supports Russian and English, with light and dark themes.

## Features

- Monthly payment overview and upcoming charges.
- Payment calendar with month navigation.
- Subscription accounts, categories, notes, domains, and service icons.
- Monthly, annual, and custom billing intervals.
- Multi-period prepayments with an optional promotional total that does not overwrite the regular subscription price.
- A user-selected base currency with conversion from other currencies.
- Monthly, category, and largest-expense analytics.
- Push and Telegram reminders.
- Data synchronization between the web app and Android.
- Google, GitHub, and Telegram sign-in.

## Screenshots

All screenshots use demonstration data and contain no user information.

### Web

<table align="center">
  <tr><td><img src="media/web-today.png" alt="SubsTrack overview" width="100%" /></td><td><img src="media/web-calendar.png" alt="SubsTrack calendar" width="100%" /></td></tr>
  <tr><td><img src="media/web-subscriptions.png" alt="SubsTrack subscriptions" width="100%" /></td><td><img src="media/web-insights.png" alt="SubsTrack insights" width="100%" /></td></tr>
</table>

### Android

<table align="center">
  <tr><td><img src="media/android-today.png" alt="SubsTrack Android overview" width="290" /></td><td><img src="media/android-calendar.png" alt="SubsTrack Android calendar" width="290" /></td><td><img src="media/android-subscriptions.png" alt="SubsTrack Android subscriptions" width="290" /></td></tr>
  <tr><td><img src="media/android-dark-today.png" alt="SubsTrack Android dark overview" width="290" /></td><td><img src="media/android-dark-calendar.png" alt="SubsTrack Android dark calendar" width="290" /></td><td><img src="media/android-dark-subscriptions.png" alt="SubsTrack Android dark subscriptions" width="290" /></td></tr>
</table>

## Installation

1. Open the [latest release](https://github.com/svllvsxprod/substrack-releases/releases/latest).
2. Download `SubsTrack-0.1.6-sideload.apk`.
3. Open the APK on your Android device and allow installation from the selected source.
4. Allow notifications on first launch if you want payment reminders.

Android 7.0 or newer is required. Version 0.1.6 upgrades an existing 0.1.4 or 0.1.5 installation without removing the app. The web version is always available at [substrack.top](https://substrack.top).

The APK checksum is attached to the release and stored in `SubsTrack-0.1.6-sideload.apk.sha256`.

## Privacy

- Sign-in uses Google, GitHub, or Telegram; SubsTrack does not receive passwords for those services.
- Account data is synchronized with the SubsTrack server over an encrypted connection.
- Reminders can be configured or disabled at any time.
- Read the [Privacy Policy](https://substrack.top/privacy) and [Terms of Service](https://substrack.top/terms).

## Repository

This public repository contains release builds, release notes, and screenshots only. The SubsTrack source code is not published here.

Found a bug or have a feature request? Open an [Issue](https://github.com/svllvsxprod/substrack-releases/issues) or contact the [Telegram channel](https://t.me/svllvsxprod).
