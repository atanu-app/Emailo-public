# Privacy

Emilo is built to keep your mail between you and Google.

**What Emilo connects to**
- **Google** — Gmail and Google sign-in, using the Google Cloud sign-in you set up yourself.
- **GitHub** — once a day, to check this repository for a newer version (only a small version file is downloaded; you can turn this off in Settings › General).
- **xAI** — only if you add your own xAI API key in Settings › AI, and only when you click Summarize or Write with Grok. Summaries and replies send the conversation; a new email sends only its subject, your note and first names. Names, email addresses, phone numbers, links and long numbers are replaced with placeholders before the text is sent, and requests ask xAI not to store them. Your key stays in your Mac's keychain.
- Nothing else is contacted unless you choose to: for example opening a link or loading a message's images.

**What stays on your Mac**
- Your Google sign-in is stored in your Mac's keychain.
- Mail lists, drafts, the Outbox, snoozes, rules and settings are stored in Emilo's container on your Mac.
- Sorting, alert detection, phishing checks, bills and package detection all run on your Mac.

**What Emilo doesn't do**
- No Emilo servers, accounts, analytics, ads or tracking.
- Remote images and tracking pixels in emails are blocked until you allow them.

**Spotlight** (optional, off by default) adds subjects, senders and previews to your Mac's Spotlight index so you can find mail from Spotlight.

**Removing your data** — see [Uninstalling](INSTALL.md#uninstalling).

Questions: [open an issue](https://github.com/atanu-app/Emailo-public/issues/new/choose).
