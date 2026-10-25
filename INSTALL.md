# Installing Emilo

## Requirements

- macOS 15 Sequoia or later (Liquid Glass effects need macOS 26)
- Apple silicon or Intel Mac
- A Gmail or Google Workspace account

## Install

1. Go to the [latest release](https://github.com/atanu-app/Emailo-public/releases/latest) and download **Emilo-&lt;version&gt;.dmg** (under *Assets*).
2. Open the downloaded file. A window opens with **Emilo** and an **Applications** folder.
3. Drag **Emilo** onto **Applications**.
4. Eject the disk image (drag it to the Trash in the Dock, or press ⌘E in Finder).
5. Open **Emilo** from Applications or Launchpad.

### Check the download (optional)

Each release lists a SHA-256 checksum (`Emilo-<version>.dmg.sha256`). In Terminal:

```sh
shasum -a 256 ~/Downloads/Emilo-<version>.dmg
```

The result should match the checksum in the release.

## First launch

Until Emilo's builds are notarized by Apple, macOS asks you to confirm the first time you open it:

1. Open Emilo. macOS says *“Apple could not verify ‘Emilo’ is free of malware…”*. Click **Done** (not *Move to Trash*).
2. Open **System Settings › Privacy & Security**.
3. Scroll down to the message about Emilo and click **Open Anyway**, then confirm with your password or Touch ID.
4. Open Emilo again and click **Open**.

You only do this once per version. Releases marked *notarized* in the release notes open without these steps.

## Connect your Google account

Emilo signs in with your **own** Google Cloud sign-in, so your mail never passes through anyone else's app. The welcome screen walks you through it (about 3 minutes); the same steps are in [Connect your Google account](docs/google-setup.md).

On first use macOS may also ask for:

- **Keychain** — Emilo stores your Google sign-in in your Mac's keychain. Click **Always Allow**.
- **Notifications** — so new mail and alerts can reach you.
- **Calendar / Reminders** — only when you use *Share availability*, *Add to Calendar* or *Add to Reminders*.

## Updating

Emilo checks for a new version once a day and shows *“Emilo &lt;version&gt; is available”* with a **Download** button. You can also choose **Settings › General › Check now**. Install an update the same way: open the new DMG and drag Emilo to Applications, replacing the old one. Your accounts and settings are kept.

## Uninstalling

1. Quit Emilo (⌘Q). If *Open Emilo at login* is on, turn it off first in **Settings › General**.
2. Drag **Emilo** from Applications to the Trash.
3. To remove its local data too, delete `~/Library/Containers/llc.tcb.emilo`, and in **Keychain Access** delete the items named `llc.tcb.emilo.oauth`.
4. To revoke Emilo's access to your Google account, visit [myaccount.google.com/permissions](https://myaccount.google.com/permissions).

## Trouble?

- **“Emilo is damaged and can't be opened”** — the download was blocked. Follow [First launch](#first-launch); if it persists, run `xattr -dr com.apple.quarantine /Applications/Emilo.app` in Terminal and open Emilo again.
- **Sign-in fails or says “access blocked”** — check the steps in [Connect your Google account](docs/google-setup.md), especially the bundle ID and test users.
- Anything else: [open an issue](https://github.com/atanu-app/Emailo-public/issues/new/choose).
