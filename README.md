# CardFlow Pro

CardFlow Pro is a Windows desktop app for credit card bill-payment shops. It
keeps the day's work in one place: bills paid for customers, swipes and cash-out
recovered, what each customer still owes, payment-account balances, and daily
reports. It works in English and Telugu, and it runs on the shop laptop without
needing an internet connection.

This page is the public download and update channel. The app's source code is
private.

## Download

1. Open the [latest release](../../releases/latest).
2. Under **Assets**, download `CardFlow-Pro-Setup-<version>.exe`.
3. Run it and follow the installer.

Requires Windows 10 or 11, 64-bit. Only download from this page.

## If Windows shows a warning

The installer is not yet signed with a paid publisher certificate, so Windows
may say it doesn't recognise it. The file is not damaged.

- **"Windows protected your PC"**: click **More info**, then **Run anyway**.
- **Microsoft Defender removes the file**: open **Windows Security > Virus &
  threat protection > Protection history**, select the CardFlow Pro entry and
  choose **Restore** or **Allow on device**, then run the installer again.

To confirm the download is unchanged, compare its checksum with the one listed
in the release notes. In PowerShell:

```powershell
Get-FileHash .\CardFlow-Pro-Setup-<version>.exe -Algorithm SHA256
```

## First-time setup

A new shop is asked for an **activation code** before the business setup form.
Contact the CardFlow Pro owner to get one. Laptops that are already set up, and
restoring an existing shop's data, do not ask for a code.

## Updates

Installed copies check for new versions on their own and download them in the
background. The update installs when you close the app, or sooner if you click
**Restart to update**. To check yourself, open **Settings > App Version &
Updates** and press **Check for updates**.

## Your data

Shop data is stored on the laptop. The app makes automatic local backups, and
can back up to Google Drive (encrypted) if that option is set up. Uninstalling
or updating the app does not delete your data.

## Releases

Each release is a version of the installer. Release notes list what changed.
Releases are published from the private source repository; this repository
only hosts the installers and update files (`latest.yml`) that the app reads.
