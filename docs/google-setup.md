# Connect your Google account

Emilo signs in to Gmail with a Google Cloud sign-in that **you** own. Nobody else's app sits between you and your mail, and you can revoke access at any time. Setting it up takes about 3 minutes and is free.

## 1. Create a project

Open [console.cloud.google.com](https://console.cloud.google.com) and create a project — for example **Emilo**.

## 2. Turn on the Gmail API

**APIs & Services › Library › Gmail API › Enable.**

## 3. Set up the consent screen

**APIs & Services › OAuth consent screen**:

- **User type:** *Internal* if your account is on Google Workspace; otherwise *External*, and add your own address under **Test users**.
- **Scopes:** add
  - `https://www.googleapis.com/auth/gmail.modify` — read, send and organise your mail
  - `https://www.googleapis.com/auth/gmail.settings.basic` — vacation replies, filters and signatures

## 4. Create the client

**APIs & Services › Credentials › Create credentials › OAuth client ID**:

- **Application type:** iOS
- **Bundle ID:** `llc.tcb.emilo`

Copy the **Client ID** (it ends in `.apps.googleusercontent.com`). No client secret is needed.

## 5. Paste it into Emilo

Paste the Client ID on Emilo's welcome screen (or later in **Settings › Accounts**) and click **Sign in with Google**. Choose your account and allow access. You can add more Gmail or Workspace accounts the same way.

## Good to know

- Apps in Google's *Testing* mode get a new sign-in every 7 days: Emilo shows **Sign in again** when that happens.
- To use **Settings › Gmail** (vacation replies, filters, signatures), the second scope above is needed; Emilo asks you to sign in again once if your sign-in predates it.
- To remove Emilo's access: [myaccount.google.com/permissions](https://myaccount.google.com/permissions).
