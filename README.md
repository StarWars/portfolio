# Product & engineering portfolio of Michał Stawarz

Public portfolio site, served by GitHub Pages at <https://starwars.github.io/portfolio/>.
It is public and indexable by search engines (since 22 November 2026), positioned for "Michał Stawarz, Engineering Manager".

## Files

| File | Purpose |
| --- | --- |
| `index.html` | Generated web edition with inline case studies. Dusk styles live in tokens.css. |
| `Michal_Stawarz_Portfolio_Case_Studies_EN.pdf` | The 16-page case-study portfolio. Generated, do not edit by hand. |
| `cover.png` | First page of the PDF as an image. The site uses mobile-work.webp for its hero and social preview. |
| `robots.txt`, `sitemap.xml`, `.nojekyll` | Crawler permissions, sitemap and Pages setting. |

## How it is maintained

This repository is a published copy. The source of truth is a private career knowledge-base project
(`ms-career-knowledge-base`, folder `output/portfolio-site/`, notes in `notes/job-search/public-portfolio.md`):

- The PDF is generated from that knowledge base with `scripts/portfolio/build_case_study_portfolio.py --public`.
- `scripts/portfolio/publish_public_site.sh` rebuilds the HTML, project images, PDF and cover, checks them and pushes here
  (it needs `gh` logged in as `StarWars`).

The HTML builder is `scripts/portfolio/build_portfolio_page.py`. Edit the page structure in `scripts/portfolio/portfolio_page.html` and the shared project records in the PDF builder.
To change the case studies, change the knowledge base or the build script, then run the publish script.

## Public-version rules

- No phone number and no email address, in the page or in the PDF.
- BIEK is public. Its case study covers the national launch after the mobile engagement ended.
- Store screenshots belong to their publishers.
- The private version of the PDF (with phone and email) is never published here.
