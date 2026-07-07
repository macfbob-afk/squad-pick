# 🎯 Squad Pick

**The app that ends the "idk, what do you wanna do?" group-chat loop.** AI picks the perfect hangout for your crew — tuned to everyone's tastes, budget, and city.

**▶ Use it now:** https://macfbob-afk.github.io/squad-pick/

## Features
- **Squads** — a separate group chat for every friend group, with polls and votes
- **AI Hangout Picker** — blends the squad's interests, budget, energy, and past favorites into 3 perfect picks; learns from every 🔥 and 👎
- **@ai in chat** — ask the AI to settle any debate, right in the group chat
- **Discover** — live Google Map of restaurants, cafés, parks, and fun near you
- **Memories vault** — log past hangouts with photos, ratings, and notes, organized by month
- **Squad Wrapped** — shareable monthly recap of your crew's stats
- **Contact linking** — invites friends through the contacts already on your phone (permission-based, nothing stored)
- **Pro** — $4.99/mo or $39.99/yr with 7-day free trial · Apple Pay, Google Pay, PayPal, Cash App

## Power it up (Settings ⚙️ inside the app)
| Key | What it unlocks | Where to get it |
|---|---|---|
| Claude AI key | Real AI picks + @ai chat | console.anthropic.com |
| Google Maps key | Live map + real places | console.cloud.google.com (Maps JavaScript API + Places API) |
| Stripe Payment Links | Real Apple Pay / Google Pay / Cash App / card checkout | stripe.com → Payment Links |
| PayPal.Me / $cashtag | PayPal & Cash App buttons | paypal.me · cash.app |

Keys are stored only in the user's own browser — never in this repo.

## AI maintainer 🤖
This repo includes a Claude GitHub Action (`.github/workflows/claude.yml`). Add your `ANTHROPIC_API_KEY` as a repo secret, then mention **@claude** in any issue — Claude reads the code, writes the fix, and opens a pull request.

## Install it like a real app 📱
Open the link on your phone → browser menu → **Add to Home Screen**. Squad Pick installs with its own icon, runs full-screen, and works offline (service worker + manifest included).

## Tests ✅
Open [`tests.html`](https://macfbob-afk.github.io/squad-pick/tests.html) — 20 automated integration tests boot the real app in a hidden iframe and drive it end-to-end (auth, squads, chat, XSS safety, polls, picks, memories, paywall math, payment routing, persistence). Your own data is snapshotted and restored around the run. Green summary = healthy build. Run it after every change.

## Tech
Single-file web app (HTML/CSS/JS, zero dependencies) · installable PWA with offline support · localStorage persistence · Claude API · Google Maps Places · W3C Contact Picker · hosted on GitHub Pages. See [CHANGELOG.md](CHANGELOG.md).

*Built with Claude Fable 5.*
