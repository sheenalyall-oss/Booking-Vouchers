# Southern Cross Safaris — Booking Voucher Automation

A single-file web app for creating, storing, printing and emailing SCS booking vouchers. Mirrors the design and workflow of the Park Fees Voucher Automation app.

## Features

- **Auto-numbered BV numbers** starting at 158215 (continues from the last handwritten voucher)
- **301-lodge property autocomplete** with region & country context
- **Live voucher preview** — see the printed layout as you type
- **Print / Save as PDF** — native browser print
- **Email button** — opens your default mail client with subject & body pre-filled
- **Voucher history** — search, reopen, reprint, delete
- **Property master list** — browsable list of all 301 lodges (Kenya, Tanzania, Zanzibar, Uganda)
- **Dashboard** — total bookings, guests, nights, bednights; top properties & top agents
- **Backup / Restore** — export JSON or CSV; re-import to restore
- **Internal Voucher Notes** — captured in history but NEVER printed on the voucher
- **Works offline** — all data in browser localStorage, no login, no server, no fees

## Live URL

After deploying via GitHub Pages, the app is available at:

`https://<your-github-username>.github.io/booking-vouchers/`

## Files

| File | Purpose |
|---|---|
| `index.html` | The complete web app (all HTML / CSS / JS / 301 properties in one file) |
| `README.md` | This file |
| `.nojekyll` | Tells GitHub Pages to serve as-is (no Jekyll processing) |

## Deploy

1. Create a new GitHub repo (e.g. `booking-vouchers`)
2. Upload `index.html`, `README.md`, `.nojekyll`
3. Settings → Pages → Source: `main` branch → `/ (root)` → Save
4. Visit `https://<your-github-username>.github.io/booking-vouchers/`

## Local use

Download `index.html`, double-click to open in Chrome / Edge / Safari — full functionality, no install.

## Data storage

- Everything stored in browser `localStorage` (keys: `scs_bv_vouchers`, `scs_bv_counter`).
- No cross-browser or cross-device sync. Use Backup / Restore to move data between machines.
- Clearing browser data will erase vouchers — export a JSON backup regularly.

## Sibling app

Designed as a sibling to the SCS Park Fees Voucher Automation app — same stack, same colour language (adapted to SCS brand navy `#0F426D` on black), same tab pattern.

Prepared for Southern Cross Safaris — September 2026.
