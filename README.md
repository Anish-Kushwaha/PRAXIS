# PRAXIS

A static, local-first career-document studio. PRAXIS runs entirely in the browser: it uses IndexedDB for structured professional data and a service worker for offline application assets. No account, API, analytics, or backend is required.

## Deploy to GitHub Pages

1. Push this repository to GitHub.
2. In **Settings → Pages**, select **Deploy from a branch** and choose the branch and `/ (root)` directory.
3. Open the generated project URL. All application asset URLs are relative, so the app works under a GitHub Pages project path.

## Local data and backup

Use **Privacy & Data** to export a JSON backup before clearing browser data or changing devices. Backups are validated locally and limited to 10 MB on import.

## PDF and printing

The **Print / PDF** action uses the browser's native print engine, which provides genuinely client-side PDF saving and the best installed-font/print support. Select **Save to PDF** in the browser print dialog.

## Notes

PRAXIS is offline-first after its static app shell is cached. Native browser print-to-PDF is used instead of a heavyweight third-party PDF dependency. Fully automatic visual crop handles and a separately paginated PDF compositor are browser-dependent capabilities; users can still resize images with their system tools and create multi-page PDFs through native printing.
