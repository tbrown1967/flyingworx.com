# Flying Worx Hugo Site Skeleton

This is a minimal Hugo skeleton ready for local development.

## Prerequisites

Install Hugo Extended (needed for SCSS if you add it later).

Windows (Chocolatey):
    choco install hugo-extended

Or download from: https://github.com/gohugoio/hugo/releases

Verify:
    hugo version

## Run the Development Server

    hugo server -D

Flags:
- -D includes draft content.
- -F would include future-dated posts.

Open http://localhost:1313/

## Create a New Post

    hugo new posts/my-new-post.md

Then edit the generated file (it will be a draft until you set draft: false).

## Build for Production

    hugo

Output goes to public/ (ignored by git).

## Customization Next Steps

1. Update hugo.toml (baseURL, title, params, menus, pagination.pagerSize).
2. Add more partials (e.g., analytics, favicon links) under layouts/partials.
3. Introduce SCSS or a utility framework (Tailwind) via the Hugo asset pipeline.
4. Add Open Graph / Twitter meta tags in head.html.
5. Configure deployment (GitHub Pages, Netlify, Cloudflare Pages, etc.).

## Deploy (Example: GitHub Pages)

Basic idea:
1. Run "hugo --minify".
2. Push public/ folder to the gh-pages branch (or let an action do it).

Add a GitHub Action later for automatic builds.

---
Enjoy building with Hugo!
