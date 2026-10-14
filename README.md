# SoCim: Barangay Report for Android

SoCim is a community reporting app for **Barangay 73, Zone 7, District II, Caloocan City**. A resident sends a report about a problem in the barangay, adds photos and a place on the map, and follows what happens to the report. This repository holds the Android app file for download.

> **This is a capstone trial build. It is not an official government service.**
> **It is not an emergency service.** In an emergency, call **911** or the hotline for your need. Do not wait for a report to be read.

## Download

- **Newest version: [SocimAI.apk](https://github.com/charlesmema/scaling-octo-fishstick/releases/latest/download/SocimAI.apk)** (about 26 MB)
- All versions and their notes: [Releases](https://github.com/charlesmema/scaling-octo-fishstick/releases)
- You can also scan the QR code on the Download page of the SoCim website.

Open the link on your **Android phone**. An iPhone cannot install this file.

## What you need

- An Android phone with **Android 9 or later**.
- Internet to send a report. A report that you write without internet is saved on your phone and sent when the phone is online again.
- Location switched on, or a pin that you place on the map by hand, to send a report.

## Install

1. On your phone, tap the download link above. The file `SocimAI.apk` downloads.
2. When the download is done, open the file (from the notification, or from the Downloads folder in the Files app).
3. Android can say that your browser or Files app is not allowed to install unknown apps. Tap **Settings**, switch on **Allow from this source**, and go back.
4. Tap **Install**.
5. Google Play Protect can show a warning such as "App not scanned" or "Unrecognized developer". The app is not in Google Play, so this is expected. If you trust where you got the file, tap **More details**, then **Install anyway**.
6. Tap **Open**. You can **Sign in**, **Create account**, or **Continue as guest**.

After the install, you can switch the "unknown apps" permission off again for your browser.

### Update

Download the newest `SocimAI.apk` and install it over the old app. Your saved data stays. The app does not update itself and does not tell you when a new version exists, so look at the [Releases](https://github.com/charlesmema/scaling-octo-fishstick/releases) page now and then.

## What the app does

- **Report a problem.** Choose the problem from a list, put a pin on the map, add 1 to 5 photos, write what happened, and send. The report waits on your phone if there is no internet.
- **My reports.** See each report with its status and the message that the barangay staff send you. Search your reports.
- **Rate a resolved report.** When the barangay marks your report as resolved, the app asks you to give 1 to 5 stars and an optional comment. After you send it, a short survey (a Google Form) opens in your browser. You do not have to answer the survey.
- **Create an account or sign in.** You sign in with your **mobile number** and a **password that you choose**. A new account is checked by the barangay. The barangay can ask you to show proof of residence at the hall.
- **Emergency numbers.** A list of emergency contacts with Call and Copy buttons. Your phone makes the call.
- **News and events.** Posts and events of the barangay.
- **Guest.** Without an account you can see the emergency numbers and the general screens. You cannot send or see reports.
- **Display.** Dark mode (default) and light mode, and an optional bionic reading mode.

## What the app asks to use

| Permission | Why |
| --- | --- |
| Internet and network state | To send reports and read their status. |
| Location (precise or approximate) | The app reads your position **once** when you send a report or an account request. It does not track you and it does not read your position in the background. |
| Notifications (Android 13 and later) | To tell you when your account request cannot be accepted. |

The app does not ask for access to your photos. You choose photos with the Android photo picker, or you take them with your camera app.

## Your data

The full text is in the app: **Create account**, then **Terms of use**. In short:

- **Account request:** your name, email, mobile number, barangay, the password you choose (the server keeps only a scrambled copy, never the password itself), your optional gender and emergency contact, and one position.
- **Report:** the problem, your text, the address you type or the pin, your photos, the time, the position of the problem, and a snapshot of your own position when you send. The title and the text of the report go to an AI service that suggests a category and a priority. Your name, address and position are not sent to it. Do not write phone numbers or the names of other people in a report.
- Barangay staff can see reports and account details. The app keeps you signed in on your phone until you sign out.
- The app does not collect audio, video, your contacts, or your position all the time.
- **Map pictures** come from OpenFreeMap (OpenStreetMap data). The map server can see the network address of your phone and the area of the map that you look at. It does not receive your report.
- To ask about your data, or to ask for it to be deleted, go to the barangay hall or ask the project team.

This text describes the trial. It is not a legal-compliance review.

## Limits of this trial

- Android only.
- The map pictures need internet. Without internet the map is empty, but your pin and your report still work. The map does not need Google Play services.
- The app has no in-app update and no push messages. It checks the status of your reports while the screen is open.
- Other phone makers change the install screens. Your steps can look a little different.

## Help

If you have a problem with your registration or your account, **go to the Barangay 73 hall**. For a problem with the file or the install, open an issue in this repository. **Do not write your password, your mobile number or other personal details in an issue.** Everyone can read it.

## For the project team: how a release is made in this repository

- Make a release with a tag such as `1.2` (the same style as `1.0` and `1.1`), and attach the file with the exact name **`SocimAI.apk`**. The download link above and the SoCim website use that name and the address `releases/latest/download/SocimAI.apk`. A different file name breaks the link.
- Raise the version code for every release. Android refuses an update with a lower version code.
- Do not attach a build that holds a secret key.

## Licence

See the file `LICENSE` for the files in this repository. The source code of SoCim is not in this repository.
