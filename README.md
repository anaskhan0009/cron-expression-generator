# Cron Expression Generator — Visual Crontab Builder, Translator & Next Run Times

Nobody memorizes cron syntax — they copy an expression from an old server and pray. This tool ends the guessing: build the schedule **visually** with pickers for all five fields, read it back in **plain English**, and see the **next 5 actual run times** computed for your own timezone before you deploy it anywhere.

**Live Demo:** https://anaskhan0009.github.io/cron-expression-generator/

## Features

- **Local account system** — sign up / log in on this device (passwords stored only as salted SHA-256 hashes, never plain text), continue as guest, per-account data separation, account deletion, and Export / Import of your records as JSON
- **Full record manager (CRUD)** — create, view, edit and delete your own saved, labelled cron expressions; the core tool works fully without an account, signing in unlocks saving
- **Visual builder** — per-field modes: Every, Every-N step, Range, or Specific values with checkbox pickers for minutes, hours, days, months and weekdays
- **Plain-English translation** — every expression explained in a sentence a human can verify
- **Next-5-runs preview** — real run times computed live, with full cron day-matching semantics (including the day-of-month OR day-of-week rule)
- **Presets & manual mode** — common schedules in one click, or paste any expression to translate and preview it

## How to Use

1. Set each field with the pickers — or click a preset, or paste an expression.
2. Read the plain-English translation and check the next 5 run times.
3. Copy the expression into your crontab.
4. Label it and save it to your collection with a note about which server it lives on.

## Why It Matters

Cron failures are silent and expensive: the backup that ran at 16:45 UTC instead of 21:45 local, the job that fired on Saturdays because of the day-of-month/day-of-week OR rule. A builder that shows the translation and the actual next runs — in a named timezone — catches both before they cost you a weekend.

## Ethical Use

This is a **developer productivity tool** — it builds and explains schedules for your own systems, entirely inside your browser. Nothing is uploaded, logged or shared.

## Tech

Single self-contained `index.html` — HTML, CSS, vanilla JavaScript, WebCrypto (salted SHA-256 password hashing), localStorage persistence. No servers, no tracking, no external requests.

---

Built by **Dinal Studios** — free developer & cyber security tools and web apps.
GitHub: https://github.com/anaskhan0009
