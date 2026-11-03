# CPA Firm Simulator

A browser game where you build an accounting firm from a one-person practice toward the IPA 500: win clients, price services, hire staff, open offices, and acquire other firms month by month.

Version 2.12.1: version 2 (phases 1–10 of the build plan), the November 3, 2026 update, staff levels, the integration pause, smaller saves and partners.

## Play

Open `index.html` in any modern browser. There's no build step and no server.

To host it online, enable **GitHub Pages** (Settings → Pages → Deploy from a branch → `main` / root). The game will be at `https://<username>.github.io/cpa-firm-simulator/`.

## What's new in 2.12.1

- **Fewer firms for sale while you're small.** Offers per year are about the square root of your revenue ÷ $100,000: 1 a year under $100K, 2 at $400K, about 3 at $1M, 5 at $2.5M, 10 at $10M, and at most 12. It was 6 a year at any size. Adjustable in Settings.
- **Fewer hours for everyday services.** CAS Tier 1 takes 40 hours a client a year (was 60), CAS Tier 2 60 (was 84), personal returns 1.5 (was 2) and business returns 8 (was 10). Existing saves convert on load.
- **Safer account saves.** A save that's cut off halfway (the app closed or lost signal) no longer leaves a broken copy in your claude.ai account; the last complete save stays in place.

## What's new in 2.12.0

- **Partners.** Directors are now partners, and you are the managing partner. Each month the firm keeps 75% of its profit before partner pay and pays 25% to its partners, split evenly. Every partner gets at least $150,000 a year; yours starts once yearly revenue passes $1M. A month that loses money pays no share, and the loss is made up from the next good months before partners share profit again. The People tab shows each partner's pay over their last 12 months as a partner.
- **Partner leads.** Each partner other than you brings about 2 extra leads a month to their department's services.
- **CAS Tiers 3–6 take 50% more hours per client** (540, 720, 1,080 and 1,350 hours a year).

Every number is in Settings under Partners.

## What's new in 2.11.0

- **Hours by staff level.** Every service splits its hours across associates, seniors, managers and directors. Bookkeeping and simple returns are mostly associate work; fractional CFO work is mostly managers and directors. Work flows down only: a director can do manager work, never the reverse. Staff work in their own department, and you count as a director anywhere. When a level runs short, services that need it stop winning clients and lose more of them. The Hiring desk shows load by level, and the Clients tab shows each service's mix and what's holding it back. You can turn this off in Settings.
- **Integration pause.** Buying a firm bigger than 90% of your revenue pauses acquisitions for about 12 months per 1× your revenue (12–36 months). Smaller deals don't pause. You can still Hold firms during a pause.
- **Smaller saves.** The mergers log keeps the last 3 years of every deal and the last 10 years of top 500 deals. If this device ever fails to save, a warning appears on every screen.

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
