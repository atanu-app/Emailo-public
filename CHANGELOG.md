# Changelog

All notable changes to Emilo. Versions follow the app's version number (Emilo › About Emilo).

## 2.2 — 2026-10-25

**Signature images fixed**
- Logos and other images in your Gmail signature now show up for the people you email. Images stored inside the signature are sent as proper inline images, the way Gmail sends them, instead of a format Gmail and many other mail apps don't display.
- Sending a draft you saved earlier no longer adds your signature logo as a separate attachment.

**Known limitations**
- This build is not yet notarized by Apple: confirm it once in System Settings › Privacy & Security (see the [install guide](INSTALL.md#first-launch)).
- AI features need an xAI account with credits ([console.x.ai](https://console.x.ai)); each request is billed by xAI.

## 2.1 — 2026-10-25

**Write with Grok**
- **Write with Grok** is in every new message and reply, not just replies. Say what you want in a few words, or tap a starting point like *Say yes*, *Politely decline* or *Ask for a meeting*.
- Emails are written as you, to the person you're writing to: short, clear and natural, without stock phrases like "I hope this email finds you well". Anything Grok doesn't know becomes a [placeholder] instead of a guess.
- Grok's text is ordinary text you can edit freely. **Try again** rewrites it, **Remove** puts back what you had (⌘Z undoes), **Keep** makes it yours.
- If your Gmail signature is attached, Grok doesn't add your name a second time.
- For a new email, only the subject, your note and first names are sent, with personal details replaced first. Email addresses are never sent.

**New templates**
- Eight ready-to-send templates: Follow-up, Meeting request, Thank you, Got it, Status update request, Reschedule, Polite decline and Sending a file.
- **Note:** updating replaces your current template list with these eight, once. If you made your own templates, copy their text somewhere before updating.

**Known limitations**
- This build is not yet notarized by Apple: confirm it once in System Settings › Privacy & Security (see the [install guide](INSTALL.md#first-launch)).
- AI features need an xAI account with credits ([console.x.ai](https://console.x.ai)); each request is billed by xAI.

## 2.0 — 2026-10-25

**AI now runs on Grok by xAI, with your own key**
- Summaries and reply drafts use **Grok** through your own **xAI API key** instead of Claude.
- **Settings › AI** is new: paste your key (it's checked with xAI before it's saved, and kept in your Mac's Keychain), see the connection status, and pick the Grok model (grok-4.7, xAI's recommended model, by default).
- Clear messages when something's wrong — wrong key, no credits, rate limit, model unavailable, offline — with a button that takes you straight to the setting to fix it.
- Personal details are still replaced before anything leaves your Mac, and requests ask xAI not to store them.
- The Anthropic key Emilo stored before is removed from your Keychain.

**Also in this release**
- Quick replies under each conversation, and "Did you mean to attach a file?" before sending.
- Phishing warnings for lookalike senders, impersonation, deceptive links and failed sender checks.
- Today and the Inbox put unread mail first and open on **Unread** while there's unread mail.

**Known limitations**
- This build is not yet notarized by Apple: confirm it once in System Settings › Privacy & Security (see the [install guide](INSTALL.md#first-launch)).
- AI features need an xAI account with credits ([console.x.ai](https://console.x.ai)); each request is billed by xAI.

## 1.0 — 2026-10-25

First public release.

**Focus**
- Today: everything that arrived today, unread first, sorted on your Mac into Codes & security, Priority, People, Updates, Newsletters and Social.
- Smart Unread filter in Today and the Inbox: opens on Unread while there's unread mail, switches to Everything when you're done.
- Alerts: recognises failure and incident emails from monitoring and CI tools, groups repeats, closes them on recovery, and highlights critical ones with a banner, row badges and notifications. Acknowledge and Resolve add Gmail labels.
- Screener for new senders, Focus delivery at set times, Set aside, Waiting on (follow-up reminders).

**Gmail**
- Folders, labels with counts, label management (create, rename, colour, nest, delete), Move to and Label as.
- Inbox tabs: Primary, Social, Promotions, Updates, Forums.
- Search across accounts; select all conversations in a mailbox.
- Compose with formatting, your Gmail signature, templates, quick replies, send later, send separately and an Outbox; reopen and edit Gmail drafts.
- Settings › Gmail: vacation responder, signatures, filters and blocked senders.
- Several Gmail and Workspace accounts.

**Safety and privacy**
- Remote images and tracking pixels blocked until you allow them; link tracking removed.
- Phishing warnings for lookalike senders, impersonation, deceptive links and failed sender checks.
- "Did you mean to attach a file?" before sending.

**Mac**
- Light and dark mode, Liquid Glass on macOS 26, menu-bar item, Spotlight (optional), Shortcuts actions, morning briefing, attachment library, bills & receipts and packages & travel views.
- Built-in update check.

**Known limitations**
- This build is not yet notarized by Apple: confirm it once in System Settings › Privacy & Security (see the [install guide](INSTALL.md#first-launch)).
- Each user connects Emilo with their own Google Cloud sign-in ([how](docs/google-setup.md)).
- Critical alerts can't yet break through Focus / Do Not Disturb.
