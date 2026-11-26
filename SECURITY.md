# Security policy

Thank you for helping keep MJSMonitor and its users safe.

## Supported versions

Only the **latest release** of MJSMonitor receives security fixes. **Help → Check for
Updates…** in the app installs it, as do `dnf` and `apt` for the Linux packages. The
newest downloads are always at <https://mjsapps.net/mjsmonitor/>.

| Version | Supported |
|---|---|
| Latest release | ✅ |
| Older releases | ❌ — please update |

## Reporting a vulnerability

**Please don't report security problems in a public issue, discussion or post.** Report
them privately in either of these ways:

- **GitHub:** open the **Security** tab of this repository and click
  **Report a vulnerability**. Only you and the maintainer can see the report.
- **Email:** <support@mjsapps.net>, with "Security" in the subject.

Please include:

- the MJSMonitor version and build — shown in **Help → About MJSMonitor** (for example
  *1.0.0, macOS · Apple silicon (arm64)*), or which download or page it affects;
- your operating system and version;
- what the problem is and the steps to reproduce it, and what an attacker could do with it.

## What happens next

- You'll get a reply **within 3 business days** confirming the report was received.
- We'll keep you updated while we investigate, and tell you whether the report is
  accepted or declined and why.
- Fixes are released as a new version, delivered through Check for Updates, `dnf` and
  `apt`. With your permission, we're glad to credit you in the release notes.
- Please give us a reasonable time to release a fix before sharing details publicly.

## Scope

- The MJSMonitor apps for macOS, Windows and Linux, and their installers and packages.
- The update information MJSMonitor downloads (`update-*.json`) and the signed `dnf` and
  `apt` repositories at <https://msanty573.github.io/OmniMonitor-Downloads/>.

## How MJSMonitor handles your data

MJSMonitor works on your computer. What you watch, every check result, incidents and the
devices found by Discover are stored locally (on a Mac in
`~/Library/Application Support/MJSMonitor`) and are never sent to MJS Applications.
Passwords and webhook links (mail server, Teams, Slack, Discord, router) are kept in the
system keychain.

MJSMonitor talks to the internet only for these:

- **The checks you set up** — the websites and services you choose to watch.
- **Alerts and summary emails you turn on** — sent to the mail server, Teams, Slack,
  Discord or ntfy server you enter, containing the name, address and status of the item.
- **Check for Updates** — MJSMonitor's update information and, when you choose to update,
  the new version from GitHub, checked against a SHA-256 checksum before use. The daily
  automatic check can be turned off in the **Help** menu.
- **Maker names** — once a month, the latest list of device makers (no information about
  your network is sent).

Discover's scan stays on your network: MJSMonitor only connects to devices the way any app
does and never tries to log in or break in.
