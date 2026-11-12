# Chemistry 360 — MVP prototype

A responsive, installable web app prototype for Chemistry 360.

## Included
- Responsive homepage and navigation
- Six starter Chemistry lessons
- Lesson comprehension checks
- Five-question interactive quiz
- Local learning progress (saved in the browser)
- Premium membership preview (demo only)
- Creator/admin preview (not secured)
- PWA manifest, service worker and app icon

## Run locally
The simplest option is to use a static web server:
1. Extract the ZIP.
2. Open a terminal in this folder.
3. Run `python -m http.server 8000`
4. Open `http://localhost:8000` in your browser.

Opening `index.html` directly also works for the main website, but PWA installation/offline caching requires HTTPS or localhost.

## Publish online
1. Create a GitHub account and a new repository, e.g. `chemistry360`.
2. Upload `index.html`, `manifest.json`, `service-worker.js`, and `icon.svg`.
3. In repository Settings → Pages, enable deployment from the main branch and root folder.
4. Wait for the published HTTPS URL, then open it on your phone.
5. In Chrome on Android, use the browser menu → Install app or Add to Home screen (wording may vary).

Alternative: upload the extracted files to a static hosting provider that supports HTTPS.

## Important before commercial launch
This is a front-end MVP prototype, not a production commerce platform. It does NOT include:
- Secure registration/login or server-side user accounts
- A real database or cloud sync
- Real Mobile Money/card payment processing
- Protected premium content
- Secure administrator authentication
- Production analytics, backups or customer support workflows

Do not collect customer information or accept payments through this prototype. Before charging customers, add a secure backend, database, authentication, payment provider integration, privacy policy, terms, refund policy and content review process. Test payment flows in the provider's sandbox first.

## Suggested next production stack
- Frontend: this responsive PWA
- Backend/database/authentication: Supabase or Firebase
- Payments: a supported Ugandan payment gateway / Mobile Money aggregator, subject to merchant onboarding and current fees
- Android: launch the PWA first; later package it as a Trusted Web Activity or build a native app if there is a clear need.
