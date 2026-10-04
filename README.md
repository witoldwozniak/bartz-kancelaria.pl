**English** · [Polski](README.pl.md)

# bartz-kancelaria.pl

Website of Kancelaria Radcy Prawnego Justyna Bartz, a one-person law practice
in Płock, Poland. Design, development and maintenance: Witold Woźniak.

**[bartz-kancelaria.pl →](https://bartz-kancelaria.pl)**

| June 2025 | October 2026 |
| --- | --- |
| ![The site in June 2025](screenshots/before-desktop.jpg) | ![The site in October 2026](screenshots/after-desktop.jpg) |

## The brief

The client is my mother, Justyna Bartz: a radca prawny (Polish legal counsel)
and a permanent mediator on the list of the President of the Regional Court in
Płock. She served as a judge for ten years and has run her own practice since
2008.

The site serves two readers:

- **A private client**, often seeing a lawyer for the first time about a
  divorce, an inheritance or a dispute, and usually reading on a phone. The
  site's purpose is to make it easy for them to call or write.
- **An institution** verifying the practice before signing a contract. For
  them, the site has to present a credible, professional practice.

Every statement on the site must be verifiable. The site makes no promises of
outcome and uses no slogans, in line with the professional ethics rules for
legal counsel.

## Results

- **No JavaScript.** Twenty pages of static HTML and one stylesheet.
- **Accessibility.** Text contrast meets WCAG AAA (7:1).
- **Mediation documents.** The eight documents used in her mediations, each
  published as a web page with a completed example and as a print-ready PDF
  generated from the same source. Four of the PDFs are fillable forms.
- **Privacy.** No cookies and no tracking. Fonts are served with the site, and
  the map is drawn from OpenStreetMap data and served as a static image. Pages
  load nothing from other domains.
- **Page weight.** About 300 kB per page, most of it fonts.
- **Testing.** An end-to-end test suite runs on every push and checks all
  twenty pages for accessibility, content, navigation, SEO metadata and the
  PDFs.
- **Maintenance.** The client chose not to manage the site herself, so there
  is no admin panel; I maintain it. Content changes do not require opening the
  code: an AI agent makes the edit and the test suite verifies it. Updating a
  phone number or a sentence takes seconds.

## Process

- **Starting point.** The previous site, shown above as June 2025, was built by
  another company and came with a hosting and maintenance plan that cost more
  than the site needed. I offered to redesign it and move her off that plan.
- **Brief.** A design interview in July 2026 set the two readers, the tone, and
  a list of things the site must never contain: no Lady Justice, gavels or
  stock photos, no promises of results, no pop-ups.
- **Design and copy.** The client gave me full control over the design and
  most of the copy. Her own texts from the old site were kept with only
  typographic corrections.
- **Approval.** New copy was reviewed with her sentence by sentence. She
  approved the final wording, with her own corrections, in September 2026.
  Until then, the preview was behind a login.
- **Hosting.** The site is on Cloudflare Pages for now, at no cost. The
  domain, hosting and e-mail are moving to a single provider that costs less
  and offers better support.

## Engineering decisions

- **Astro instead of Nuxt.** The first version I built ran on Nuxt. Measured on
  its build output, it sent 320 kB of JavaScript (gzipped) on every page load.
  The only interactive element was a mobile menu, and the redesign removed even
  that. The first plan was to keep Nuxt; the measurements reversed it. The
  Astro rebuild sends no JavaScript, has 5 runtime dependencies instead of 17,
  and builds in under a second.
- **A written design system.** Every colour, size and spacing value comes from
  one token sheet. Text colours were chosen to clear 7:1 against the site's
  single background, so contrast cannot pass on one surface and fail on
  another.
- **One source per document.** Each mediation document is a Markdown file with
  custom form tokens (blank, checkbox, signature), rendered by a small Markdown
  plugin. Headless Chromium prints the PDF from the page. For fillable forms, a
  script measures where each blank landed in the printed PDF and places a form
  field exactly there. Each PDF records a hash of its source, and CI fails if a
  document changed but its PDF was not regenerated.
- **Tests that can fail.** axe-core scans every page. Touch targets are
  measured against a 48 px minimum. The PDF check confirms under print
  emulation that no sample text reaches paper. The route list is written by
  hand, so a page that stops rendering cannot quietly drop out of the tests.
  After any change to the accessibility gate, it is broken on purpose to prove
  it still goes red.
- **Privacy by construction.** Fonts are self-hosted. The map is drawn by a
  Python script from OpenStreetMap data into an SVG of 14 kB gzipped, with
  labels as real HTML text. The Content Security Policy is `default-src
  'none'` with no script source at all. A Google static map was ruled out
  because its terms require loading it from Google in the visitor's browser.
- **A repository an AI agent can work in.** Conventions are documented for the
  agent. Changeable facts sit in one data file and prose in Markdown, so
  routine edits land in predictable places and the tests catch mistakes.

**Stack:** Astro 7 · Tailwind CSS v4 · TypeScript · Playwright + axe-core ·
Biome · Bun · GitHub Actions · Cloudflare Pages

The source code is private.

## Contact

Witold Woźniak

- E-mail: [witold@witoldwozniak.dev](mailto:witold@witoldwozniak.dev)
- LinkedIn: [linkedin.com/in/witold-wozniak](https://www.linkedin.com/in/witold-wozniak/)
