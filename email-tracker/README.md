# Email Tracker

A tiny, zero-backend tool for tracking cold-email outreach. Add leads, mark reply status, jot notes — everything stays on your own device.

**Live:** https://karahanjustin.github.io/email-tracker/

## Features

- Track leads with name, email, website, and site-quality tag
- Status workflow: Not sent → No reply / Not interested / Replied / Closed
- Per-lead notes and follow-up dates (auto-set on No-reply / Replied)
- Live stats: total, sent, replied, closed
- **CSV import** — drop a spreadsheet export, missing fields show as `???` and stay editable
- Export / Import as JSON for backup or moving between devices

## CSV format

Header row is auto-detected. Recognized columns (any subset, any order):

```
name, email, website, quality, notes
```

Quality values: `none`, `bad`, `ok` (anything else → `???`). Missing fields become `???` and can be edited inline later.

## Privacy

All data is stored in your browser's `localStorage`. It survives reboots, browser restarts, and shutdowns. It never leaves your device — there is no server.

Clearing your browser's site data for this domain will wipe your leads. Use **Export JSON** regularly if your list matters.

## Run locally

It's a single `index.html` — open it in any browser. No build, no install.

```sh
open index.html
```

## License

MIT
