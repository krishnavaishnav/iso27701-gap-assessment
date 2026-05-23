# ISO 27701:2025 Gap Assessment Tool

A free, open-source gap assessment tool for **ISO/IEC 27701:2025** — the Privacy Information Management System (PIMS) standard. Built as a single HTML file with no dependencies, no backend, and no data leaving your browser.

🔗 **[Live demo →](https://YOUR-PROJECT.vercel.app)**

![ISO 27701:2025 Gap Assessment Tool](https://img.shields.io/badge/ISO%2027701-2025-blue) ![License: MIT](https://img.shields.io/badge/License-MIT-green) ![No dependencies](https://img.shields.io/badge/dependencies-none-brightgreen)

---

## Features

- **All 78 controls** across three Annex A sections:
  - A.1 — 31 PII Controller controls
  - A.2 — 18 PII Processor controls
  - A.3 — 29 Shared information security controls
- **Role-based filtering** — select Controller, Processor, or Both
- **Live compliance score** — weighted score (partial = 50%) with colour-coded progress
- **Common gap hints** — shown when a control is marked ❌ Not implemented
- **Filter views** — show all, gaps only, partial, or unrated controls
- **Export to CSV** — download a full report ready for your SoA or audit evidence pack
- **Auto-saves to localStorage** — progress survives browser refresh
- **Dark mode** — respects system preference
- **No backend, no tracking, no cookies** — everything runs in your browser

---

## Deploying to Vercel

### Option 1 — Deploy from GitHub (recommended)

1. Fork or clone this repo to your GitHub account
2. Go to [vercel.com](https://vercel.com) → New Project
3. Import your GitHub repo
4. Vercel auto-detects it as a static site — click **Deploy**
5. Done. Your tool is live at `https://your-project.vercel.app`

No build step, no configuration required.

### Option 2 — Deploy with Vercel CLI

```bash
npm i -g vercel
cd iso27701-gap-assessment
vercel
```

---

## Running locally

Just open `index.html` in any browser — no server required:

```bash
# macOS
open index.html

# Linux
xdg-open index.html

# Or use any static server
npx serve .
python3 -m http.server 8080
```

---

## Project structure

```
iso27701-gap-assessment/
├── index.html        # The entire tool — self-contained
├── vercel.json       # Vercel deployment config (optional)
├── README.md
└── LICENSE
```

---

## About ISO 27701:2025

ISO/IEC 27701:2025 is the second edition of the Privacy Information Management System standard, published in October 2025. Key changes from the 2019 edition:

- **Standalone standard** — ISO 27001 is no longer a prerequisite
- **Own HLS clauses 4–10** — full management system in one document
- **78 controls** across A.1 (controller), A.2 (processor), A.3 (shared security)
- **New Annex B** — implementation guidance
- **Updated GDPR mapping** annex
- **Transition deadline** — October 2028 for organisations certified under 2019 edition

> **Note:** ISO 27701 certification does not constitute a GDPR safe harbour. It provides strong evidence of technical and organisational measures (TOMs) under GDPR Articles 24 and 32, but does not guarantee compliance or shield organisations from regulatory enforcement.

---

## Contributing

Contributions welcome. Please open an issue or PR for:
- Control description corrections
- New features (notes per control, GDPR mapping view, SoA export)
- Translations
- Accessibility improvements

---

## License

MIT — free to use, modify, and distribute.

---

## Disclaimer

This tool is for self-assessment purposes only. It does not constitute legal advice and does not guarantee ISO 27701 certification readiness. Always engage a qualified auditor or privacy professional for formal assessments.
