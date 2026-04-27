# andrew-andrada.github.io

Personal research portfolio for Andrew Andrada, PhD, MSPH — quantitative researcher pivoting from epidemiology into UX research.

**Live site:** [https://andrew-andrada.github.io/](https://andrew-andrada.github.io/)

The site presents three selected case studies framed around the methods most directly relevant to quantitative UX research:

- **Workflow & Journey Research** — a mixed-methods process evaluation of a pediatric care pathway in rural Zambia (~100+ semi-structured interviews, facility-readiness assessments, caregiver surveys). Manuscript submitted to *PLOS One*, March 2026.
- **Measurement Validation** — comparison of a national routine tracking system (DHIS2) against a gold-standard prospective cohort, using Bland-Altman analysis and negative-binomial mixed-effects regression to quantify instrumentation accuracy. Aim 1 of dissertation, Tulane (June 2025).
- **Product Analytics from Zero** — solo end-to-end build of a Filipino mahjong mobile game with embedded analytics across Firebase, AdMob, and BigQuery. Currently in Google Play closed testing.

## Repository contents

```
.
├── index.html      # the site itself, single-page, no build step
├── README.md       # this file
└── images/         # figures cited in the case studies
```

Figures embedded in Case Studies 1 and 2 are reproduced from work-in-progress and published research and are credited in figure captions on the site. Case Study 3 links externally to the [mahjong-filipino](https://github.com/andrew-andrada/mahjong-filipino) repository and the [Google Play closed-testing listing](https://play.google.com/store/apps/details?id=com.bayanihangames.filipinomj).

## Tech stack

Plain HTML and CSS — no build step, no JavaScript, no framework. Served by GitHub Pages from `main`. The page is intentionally simple so it loads instantly, ages well, and stays accessible.

## Local preview

Open `index.html` in any browser. That's it.

## Publishing

This repo is named exactly `andrew-andrada.github.io`, which is what tells GitHub Pages to host it as a user site at the root domain. Push to `main` and the site rebuilds within ~60 seconds.

```bash
git add .
git commit -m "Update portfolio"
git push origin main
```

## Adding a case study

Each case study lives inside an `<article class="case">` block in `index.html`. Copy an existing one and edit:

- `<h3>` — case study title
- `.meta` — context line (role, organization, year)
- `.tags` — short keyword chips
- `<figure>` — embedded figure with caption (optional but encouraged)
- `<dl>` — Question, Approach, Findings, Outputs / Stack
- `.takeaway` — the UXR-translation paragraph
- `.case-links` — external links to source / live demos / publications (optional)

Place new figures in `images/` and reference them with URL-encoded paths (e.g. `images/Fig%201.png` if the filename has a space).

## Contact

[andrew.p.andrada@gmail.com](mailto:andrew.p.andrada@gmail.com) · [LinkedIn](https://www.linkedin.com/in/andrew-andrada/) · [Google Scholar](https://scholar.google.com/citations?user=isQdJ2UAAAAJ&hl=en&oi=sra)
