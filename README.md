# Tools Hub

Internal tooling hub for Potsdam Media. An interconnected interface that links every tool
and holds the shared demo scheduler.

Live: https://tools.homeservicereply.com/

## Tools

- **Call Tracker** (live) -> https://potsdam-media.de/leads/
- **Scheduler** (live) -> Cal.com embed inside the hub
- Lead Finder, Pipeline, Demo Studio -> planned

## Connect the calendar

The scheduler embeds Cal.com (shared, time zones + reminders handled automatically).
To activate it, set the constant in `index.html`:

```js
const CAL_LINK = "homeservicereply/demo";  // your cal.com user/event
```

While `CAL_LINK` is empty, the hub shows setup instructions instead of the calendar.

## Add a tool

In `index.html`, add another `.card live` with a link inside `.grid`, or a `.card soon`
placeholder. Single file, no build, no backend.

## Deployment

GitHub Pages from `main`, root. Custom domain via the `CNAME` file
(`tools.homeservicereply.com`).

DNS at the registrar (Porkbun): a `CNAME` record, host `tools`, target
`karahanjustin.github.io`.
