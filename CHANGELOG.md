# Changelog

## v2.1.1 — 2026-07-06
**Legal hardening.**
- Added Terms of Service (terms.html) and Privacy Policy (privacy.html), linked from signup, paywall, and profile.
- Signup consent line; 13+ age gate enforced in onboarding (COPPA).
- Paywall: automatic-renewal disclosure and cancellation info (FTC negative-option / state auto-renewal laws); removed unsubstantiated rating/social-proof claims (FTC advertising rules).
- AI-suggestion judgment disclaimer; copyright notice; 5 new legal-compliance tests (28 total).

## v2.1 — 2026-07-06
**Perfection pass: PWA, tests, and polish.**

### Added
- **Installable PWA** — web app manifest, app icons, and a service worker with offline support. "Add to Home Screen" now installs Squad Pick like a native app.
- **Automated test suite** (`tests.html`) — 20 integration tests that boot the real app and drive it end-to-end: auth, onboarding, squads, chat, XSS safety, polls, AI picks, taste memory, memories vault, paywall pricing, payment-link routing, Pro unlock, and localStorage persistence. Visitor data is snapshotted and restored around each run.
- **Squad options modal** — proper UI for add member (incl. from contacts), remove member, rename, and delete. Replaces the old text-prompt flow.
- **Social link previews** — Open Graph + Twitter card tags with a branded share image, so the app link looks professional when shared on socials.
- **Discover preview mode** — sample places now have "Poll the squad" buttons too.
- Escape key and backdrop-click close any modal. Enter submits the sign-in form.
- Accessibility labels on icon-only buttons.

### Fixed
- Signing up on a device that already has data now warns before overwriting (with a pointer to Settings → Backup).
- Logging in with a non-matching email no longer silently creates a new account.
- Boot sequence is fault-tolerant — a corrupted theme/streak can't blank the app.

## v2.0 — 2026-07-03
- Full rebuild: multi-squad group chats, polls, AI hangout picker with taste memory, @ai chat, personalization profile, memories vault, Squad Wrapped, Discover (Google Maps), contact linking, paywall ($4.99/mo · $39.99/yr) with Apple Pay / Google Pay / PayPal / Cash App checkout via payment links, backup/restore, themes.
- Published to GitHub Pages; Claude AI maintainer workflow added.
