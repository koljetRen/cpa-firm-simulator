# CPA Firm Simulator

A browser game where you build an accounting firm from a one-person practice toward the IPA 500: win clients, price services, hire staff, open offices, and acquire other firms month by month.

Version 2.10.0 completes version 2 (phases 1–10 of the build plan) plus the November 3, 2026 update.

## Play

Open `index.html` in any modern browser. There's no build step and no server.

To host it online, enable **GitHub Pages** (Settings → Pages → Deploy from a branch → `main` / root). The game will be at `https://<username>.github.io/cpa-firm-simulator/`.

## What's new in 2.10.0

- **Tutorial.** Every New Game asks whether you want a guided tutorial or to skip it. The tutorial starts a preset firm and walks you through each screen, and you can replay it from Settings.
- **IPA 500 tab.** The IPA 500 list replaces the Turn Log tab, so you no longer scroll through Growth to find it.
- **Launch several services at once.** The year-end pop-up lets you tick several services. On the Clients tab, pick services and launch them from a bar that stays on screen.
- **Acquired staff follow version 1.** A firm comes with round(revenue ÷ $200,000) staff, so small practices (under about $100K) bring their client list but no staff.
- **Technology tiers (phase 9).** Basic, Cloud and AI-assisted tiers have a monthly cost per person, more client output, and a learning curve after you upgrade.
- **CPE (phase 9).** Licensed staff (CPA, EA, CPB) spend yearly CPE hours and pay a training cost. If you skip CPE, licenses can lapse at year end.
- **Balancing (phase 10).**
  - After the hiring hand-off, directors hire interns and make full-time offers only where a department is busy. They used to fill every seat and over-hire large firms.
  - Negative cash now costs 10% a year in interest.
  - Office placement is much faster for large firms.

Every number is in Settings.

## Saving

Progress is saved in your browser's local storage on the device you play on. The claude.ai-hosted version also syncs saves to your claude.ai account, which isn't available on other hosts. Settings → Copy save code makes a backup you can paste into either version.

## Notes

- It's a single self-contained HTML file. Fonts load from Google Fonts.
- Firm rankings start from the 2026 IPA 500 revenue list.
