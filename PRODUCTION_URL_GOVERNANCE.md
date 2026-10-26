# Melody Website — Production URL Governance

## Single public origin
The only intended indexable production origin is:
https://melody-brand-website.vercel.app/

GitHub is source/version control. Preview and development artifacts must not be published as indexable production pages.

## Release flow
1. Develop on a non-production branch / protected preview.
2. QA content, layout, links, metadata and analytics.
3. Confirm preview is not intended for search indexing.
4. Merge approved work to `main`.
5. Deploy production on Vercel.
6. Verify canonical, sitemap, robots, internal links and HTTP status.
7. Only production URLs are submitted or promoted to Google.

## URL stability
- Existing production URLs should remain stable when content/design changes.
- Do not create `*-preview.html` files on `main`.
- Do not publish a second public copy of the site on GitHub Pages.
- If a production URL must change, map the old URL to the closest new URL with a permanent redirect where the host is controllable.
- Do not redirect unrelated/dead URLs indiscriminately to the homepage.

## SEO checks for every new page
- One production URL.
- Self-referencing canonical using the production Vercel origin.
- Correct title and description.
- Added to sitemap only when intended to be indexed.
- Internal links use production page paths.
- Preview/staging copies are not indexable.
- Verify production returns the intended HTTP status after deployment.
- Preserve existing analytics unless a deliberate tracking change is approved.

## Current canonical production pages
- `/`
- `/about.html`
- `/gyrotonic.html`
- `/learning-map.html`

This document is the standing release rule for future Melody website development, including Overseas Training and Trainer Identity work.
