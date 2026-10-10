# Cloud Service Site Template

[English](README.md) | [简体中文](README.zh-CN.md)

> A lightweight multi-page product site — 31 static HTML pages, no framework, no build step.

> **Note.** This repository contains company-specific content — brand copy, logos and asset paths. The layout, effects and code are what is worth taking. Replace the content before publishing.


## What this is

This is not a framework starter. There is no React, no Tailwind, no bundler.

It is the other approach: plain HTML pages with plain CSS, plus a news archive. The whole thing is small enough to read end to end, which is the point — some product sites do not need a build pipeline, and this shows what that looks like when it is done properly.

## Why we open-sourced it

We run this site for one of our own services. The structure turned out to be reusable, so we separated it from the content.

What is portable is the page organisation, the shared layout approach and the news archive pattern. Replace the copy and it is a starting point for something else.

## What's in it

- **31 HTML pages** including a landing page, about, company, contact, a 404 and a dated news archive.
- **No dependencies.** Nothing to install, nothing to update, nothing that breaks on a version bump.
- **Small by measurement.** Roughly 420 KB across 35 files.
- **A dated news pattern.** Articles are individual pages named by date, which makes the archive navigable without a CMS.

## Requirements

Any static file server.

## Getting started

Serve the folder and open it:

```bash
python -m http.server 8000
# then visit http://localhost:8000
```

Or open `index.html` directly.

## Structure

```
├── 404.html
├── about.html
├── assets/
│   └── style.css
├── company.html
├── contact.html
├── index.html
├── news-20250618.html
├── news-20250710.html
├── news-20250812.html
├── news-20250828.html
├── news-20250915.html
├── news-20251020.html
├── news-20251108.html
├── news-20251128.html
├── news-20251220.html
├── news-20260112.html
├── news-20260128.html
├── news-20260214.html
├── news-20260310.html
├── news-20260326.html
├── news-20260416.html
├── news-20260507.html
├── news-20260526.html
├── news-20260616.html
├── news-20260630.html
├── news-20260720.html
├── news-20260806.html
├── news-20260825.html
├── news-20260910.html
├── news-20260928.html
├── news.html
├── products.html
├── robots.txt
└── sitemap.xml
```

## Notes and limits

1. **Shared markup is duplicated, not templated.** With no build step there is no include mechanism, so a header change means editing every page. That is the trade for having no toolchain.
2. **A build output folder is present in the original and should be removed.** The `_build` directory is an artifact, not source.
3. **Content is company-specific.** Replace the copy, company details and contact information.
4. **News pages are dated in the past.** Kept as structure examples; they are not live.

## License

MIT
