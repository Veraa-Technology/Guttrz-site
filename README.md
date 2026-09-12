# Guttrz site

Flat HTML. No build step.

## Deploy (Cloudflare Pages)
1. Push this repo to GitHub.
2. Cloudflare dashboard > Workers & Pages > Create > Pages > Connect to Git > pick this repo.
3. Build command: leave blank. Build output directory: `/`
4. Custom domains > add `getguttrz.com` and `www.getguttrz.com`. Cloudflare sets DNS and SSL.

## Update
Edit `index.html`, commit, push. Live in about 30 seconds.

## Before first deploy
- Add `og.jpg` (1200x630) to the repo root. Referenced in the head and schema.
- Confirm the GHL webhook URL in the form `data-endpoint`.
- After GBP is verified, add the Google Maps profile URL and Facebook page to `sameAs` in the schema.
- Submit `https://getguttrz.com/sitemap.xml` in Google Search Console (Domain property).

## Adding city pages later
Create `/canton-gutter-guards/index.html`, `/akron-gutter-guards/index.html`, etc. Each needs 600+ words of real local copy, its own title and H1, and a line in `sitemap.xml`.
