# Chemistry 360 – Learning Library v1

A free, static, mobile-friendly Chemistry learning library for Ugandan secondary learners (S1–S6).

## Included in this first release
- Class filters for S1, S2, S3, S4, S5 and S6
- One starter lesson for each class
- Learning outcomes, explanatory notes and worked applications
- Original schematic diagrams
- Topic-specific YouTube search links for supplementary video learning (these are search links, not individually reviewed videos)
- Two interactive comprehension questions per lesson with instant feedback
- Local lesson-completion tracking on the learner's device
- Basic PWA manifest and offline cache

## Publish on GitHub Pages
1. Download and extract the project ZIP.
2. Open your existing Chemistry 360 GitHub repository.
3. Upload/replace `index.html`, `manifest.json`, `service-worker.js`, `icon.svg`, and `README.md` in the repository root.
4. Commit the changes to your `main` branch.
5. Open the published GitHub Pages website and refresh. If an old version remains, wait a few minutes and refresh; the service worker may cache the previous version.

## Important limitations
- This is a front-end learning library. Progress is stored only in the current browser/device using localStorage; it does not sync between devices.
- There are no student accounts, teacher dashboard, cloud database, protected paid content or payment processing.
- Video links open YouTube search results rather than a selected/endorsed video.
- This is a starter set of six sample lessons, not complete S1–S6 syllabus coverage. Review content against the current NCDC/UNEB requirements before formal use or sale.
- Chemistry practicals must be performed only under qualified teacher supervision and with appropriate safety controls.

## Run locally
Open `index.html` in a browser for a basic preview. For PWA/service-worker testing, serve the folder over localhost, for example:

```bash
python -m http.server 8000
```

Then visit `http://localhost:8000`.
