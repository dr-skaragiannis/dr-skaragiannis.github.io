# S\KARAGIANNIS — Personal Research Website

**Play . Learn . Defend**  
**Παίζω . Μαθαίνω . Αμύνομαι**

Official personal and academic website of **Dr. Stylianos Karagiannis**, Postdoctoral Researcher in Cybersecurity at the Department of Informatics, Ionian University (NMSLab, Corfu, Greece).

---

## Overview

This repository contains the source code for a bilingual (English / Greek), theme-aware scientific personal website presenting:

- Research profile, biography, and academic path  
- Research areas (CTF, Game-Based Learning, Cyber Ranges, Adversary Emulation, Healthcare/IoMT Security, Privacy Pedagogy)  
- Publications and scholarly metrics  
- Research projects and prototypes (including **ZeroCrowd PhishGame**, PocketCTF, NITRO, Chidroid, and others)  
- Teaching portfolio  
- Contact and professional profiles  

The site is designed as a long-lived public presence and as a foundation for future **SaaS** educational and cybersecurity-training products under the Licensor’s Intellectual Property (see [LICENSE.md](./LICENSE.md)).

---

## Features

| Feature | Description |
|--------|-------------|
| **Bilingual UI** | Full English and Greek (Ελληνικά) interface with scientific terminology; `EN \| ΕΛ` toggle |
| **Light / Dark theme** | Body sections adapt; **header, hero, and footer remain always dark** |
| **Brand lockup** | Single-line `S\KARAGIANNIS` wordmark with tagline |
| **Research catalogue** | Filterable publications, project cards, EU Horizon programme list |
| **Featured product** | ZeroCrowd PhishGame live demo and repository links |
| **Responsive layout** | Content shell at ~85% viewport width; elevated type scale (~115%) |
| **SEO** | Open Graph / Twitter cards, JSON-LD, `sitemap.xml`, `robots.txt`, web app manifest |
| **Accessibility** | Semantic structure, ARIA labels on controls, keyboard-friendly toggles |

---

## Technology stack

- **React 19** + **TypeScript**  
- **Vite 7** (single-file production build via `vite-plugin-singlefile`)  
- **Tailwind CSS 4**  
- **React Router** (HashRouter for portable static hosting)  
- Custom design tokens (ink / cream / bronze accent), Instrument Serif + Inter + JetBrains Mono  

---

## Getting started

### Prerequisites

- Node.js 20+ (recommended)  
- npm 10+

### Install

```bash
npm install
```

### Development

```bash
npm run dev
```

### Production build

```bash
npm run build
```

Output is written to `dist/` (typically a single self-contained `index.html` suitable for static hosting or GitHub Pages).

### Preview

```bash
npm run preview
```

---

## Project structure

```
├── index.html                 # HTML shell, SEO meta, theme/lang boot script
├── LICENSE.md                 # All Rights Reserved — proprietary licence
├── README.md                  # This file
├── public/
│   ├── logo-dark.svg          # Wordmark for light backgrounds
│   ├── logo-light.svg         # Wordmark for dark backgrounds
│   ├── og-image.png           # Open Graph / social share image
│   ├── robots.txt
│   ├── sitemap.xml
│   └── site.webmanifest
└── src/
    ├── App.tsx                # Router
    ├── main.tsx               # Providers (theme, language)
    ├── index.css              # Design tokens, surfaces, zone-dark
    ├── components/            # Layout, Logo, toggles, Section, PageHeader
    ├── context/               # ThemeContext, LanguageContext
    ├── data/content.ts        # Canonical research data (pubs, projects, links)
    ├── i18n/translations.ts   # EN / EL copy
    └── pages/                 # Home, Research, Publications, Projects, Teaching, About, Contact
```

---

## Configuration notes

- **Theme** preference: `localStorage` key `sk-theme` (`dark` \| `light`)  
- **Language** preference: `localStorage` key `sk-lang` (`en` \| `el`)  
- **Routing**: Hash-based (`#/research`, etc.) for maximum compatibility with static hosts  
- **Canonical identity links**: ORCID, Google Scholar, ResearchGate, GitHub, Ionian University staff page — see `src/data/content.ts`

Update `public/sitemap.xml` and Open Graph URLs in `index.html` when the production domain is finalised.

---

## Intellectual property and commercial status

**© 2026 Dr. Stylianos Karagiannis. All rights reserved.**

This project is **proprietary software**. Full Intellectual Property rights are claimed by **Dr. Stylianos Karagiannis**.

- The Work is intended for **SaaS** and other commercial or institutional deployments; plans remain under discussion and will be governed by separate written agreements.  
- **Collaborations and investments** are welcome for branch products and related ventures, subject to written agreement.  
- **Ionian University** retains **shared benefits and exploitability options** through academic affiliation and project participation, as defined by institutional policy, grant instruments, and separate written agreements — without diminishing the Licensor’s full IP claim unless expressly agreed in writing.

See **[LICENSE.md](./LICENSE.md)** for the complete legal notice.  
Unauthorised copying, modification, distribution, hosting, or commercial exploitation is strictly prohibited.

---

## Contact

| | |
|--|--|
| **Email** | [skaragiannis@ionio.gr](mailto:skaragiannis@ionio.gr) |
| **ORCID** | [0000-0001-9571-4417](https://orcid.org/0000-0001-9571-4417) |
| **GitHub** | [github.com/dr-skaragiannis](https://github.com/dr-skaragiannis) |
| **Institution** | [Department of Informatics, Ionian University](https://di.ionio.gr/en/department/staff/1061-karagiannis/) |
| **Scholar** | [Google Scholar](https://scholar.google.com/citations?user=nldsDgQAAAAJ) |

For licensing, collaboration, investment, or deployment enquiries, please contact the Licensor directly.

---

## Acknowledgements

Academic affiliation: **Ionian University**, Department of Informatics — Networks, Multimedia and Security Systems Laboratory (**NMSLab**).  
Research contributions have been supported in part through European programmes (including Horizon initiatives such as AI4CYBER, DYNABIC, DAIS, CYBERSECPRO, SPHINX, AI4HEALTHSEC, MOORE4MEDICAL, NITRO, and related consortia), subject to their respective agreements.

---

**S\KARAGIANNIS** · Play . Learn . Defend  
Corfu, Greece
