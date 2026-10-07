# Portfolio Site Plan

## Goal
Create a publish-ready Jekyll personal portfolio for Charles Gao at
`charlesgao721.github.io`, with GitHub Pages publishing from `main` and `/`.

## Pages and content
- **Home:** name and a short introduction based only on the supplied bio.
- **About:** the supplied MBA and career summary, plus education.
- **Work Experience:** list the two supplied roles and descriptions without adding claims.
- **Contact:** link to the supplied LinkedIn profile. Do not publish an email address or phone number.

## Design
Use a light, text-forward, single-column layout with generous whitespace, a system
sans-serif font stack, readable line length, and responsive semantic HTML. Include
shared navigation and footer; no hero image, animation, carousel, or external font.

## Implementation
Keep the complete site at the repository root: Markdown pages with YAML front
matter, reusable Jekyll layouts and includes, CSS/favicon assets, SEO metadata,
sitemap, `_config.yml`, and a README with update, local-preview, and Lighthouse
instructions. Set `url` to `https://charlesgao721.github.io` and `baseurl` to an
empty string; use Jekyll URL filters for internal links. Exclude this plan from
the generated site.

## Verification
Check the Jekyll/GitHub Pages configuration, page/navigation links, and responsive
layout at 375px and 1280px. Run Lighthouse and target at least 90 in Performance,
Accessibility, Best Practices, and SEO.

## Assumptions
- The supplied LinkedIn URL is the only public contact method.
- The provided role, education, dates, and descriptions are the complete first-version content; unsupplied details will not be invented.
- Approval authorizes replacing the existing starter API, mockup, and workspace scaffolding so the repository contains only the static Jekyll site.
