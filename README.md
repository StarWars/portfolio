# Mobile portfolio of Michał Stawarz

Public portfolio site, served by GitHub Pages at <https://starwars.github.io/portfolio/>.
It is meant to be shared by direct link (job applications); search engines are asked not to index it.

## Files

| File | Purpose |
| --- | --- |
| `index.html` | The whole page: text, App Store links and styles. Edit it directly. |
| `Michal_Stawarz_Portfolio_Case_Studies_EN.pdf` | The 15-page case-study portfolio. Generated, do not edit by hand. |
| `cover.png` | First page of the PDF as an image (page preview and link preview). |
| `robots.txt`, `.nojekyll` | Crawler hint and Pages setting. Leave as they are. |

## How it is maintained

This repository is a published copy. The source of truth is a private career knowledge-base project
(`ms-career-knowledge-base`, folder `output/portfolio-site/`, notes in `notes/job-search/public-portfolio.md`):

- The PDF is generated from that knowledge base with `scripts/portfolio/build_case_study_portfolio.py --public`.
- `scripts/portfolio/publish_public_site.sh` rebuilds the PDF and cover, checks them and pushes here
  (it needs `gh` logged in as `StarWars`).

To change the page text, edit `index.html` in the private project (or here, then copy it back).
To change the case studies, change the knowledge base or the build script, then run the publish script.

## Public-version rules

- No phone number and no email address, in the page or in the PDF.
- The retail client is not named ("one of Poland's biggest retailers"); unreleased product details stay out.
- Store screenshots belong to their publishers.
- The private version of the PDF (with phone and email) is never published here.
