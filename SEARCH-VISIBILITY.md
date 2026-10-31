# Search visibility and launch maintenance

Canonical product page: https://orpheane.github.io/cozy-aquarium/

## Deployment and submission status — 31 October 2026

- GitHub Pages is live. The canonical page, stylesheet, sitemap, and `llms.txt` returned HTTP 200.
- The controlling host-root `robots.txt` permits crawling and declares the product sitemap. The portfolio sitemap includes the product URL, and the portfolio's Cozy Aquarium entry links to it.
- The IndexNow verification file is publicly accessible and matches the submitted key. IndexNow returned **HTTP 202**: URL received, key validation pending. This is not confirmation that the page is indexed.
- Local browser checks passed at 1440, 390, and 320 pixels, including HTML access without application JavaScript, image decoding, internal links, and exact FAQ/schema agreement. The mobile layout has no horizontal overflow.
- Authenticated Google Search Console and Bing Webmaster Tools submissions have **not** been performed. No accessible dashboard session was available. Follow the steps below to submit the sitemap and inspect actual indexing.

## Implemented

- Static English HTML, available without application JavaScript, with descriptive headings, real screenshots, and an accessible mobile layout.
- Canonical URL, descriptive title and description, indexable robots metadata, favicon, Open Graph and social preview metadata.
- Schema.org `SoftwareApplication`, `WebPage`, `WebSite`, creator identity, and `FAQPage` data. FAQ answers match the on-page answers. No invented ratings, price, availability date, or testimonials.
- XML sitemap with the canonical page and screenshot URLs.
- `llms.txt`, a supplementary factual summary with official sources and the pre-release status. It is not a recognized universal indexing control and does not guarantee AI visibility.
- An IndexNow verification file scoped to `/cozy-aquarium/`, for notifying participating search engines about the product page.
- A link from the repository README to the canonical website.

The controlling robots file is **https://orpheane.github.io/robots.txt**, managed in `Orpheane/orpheane.github.io`. A robots file inside the project directory would not control crawling. The host's existing `User-agent: * / Allow: /` permits search crawlers, including OAI-SearchBot, without requiring an additional per-bot rule.

## Search Console and Bing Webmaster Tools

Sitemap URL: **https://orpheane.github.io/cozy-aquarium/sitemap.xml**

1. In [Google Search Console](https://search.google.com/search-console), use the verified URL-prefix property `https://orpheane.github.io/`, or add the project URL-prefix property. Submit the sitemap above, inspect the canonical product URL, and request indexing.
2. In [Bing Webmaster Tools](https://www.bing.com/webmasters/), use or verify the appropriate site, submit the same sitemap, and check the URL inspection report. A verified Google property can be imported if offered by Bing.
3. Existing verification on a different property is not proof that the new project property is verified. If a new token is required, obtain it from the actual account; do not invent or reuse an unrelated token.

These authenticated dashboard actions require account access. A live page, sitemap, robots permission, or successful IndexNow response is not proof of indexing. Search impressions and URL inspection reports are the way to confirm actual inclusion.

## At public launch

- Verify that the Chrome Web Store listing is publicly accessible before changing the release status.
- Update `index.html`, `README.md`, and `llms.txt` together. Change “Coming soon” to an accurate installation call to action.
- Update the sitemap's `lastmod` only when meaningful page content changes.
- Add the canonical product page to the Chrome Web Store website field, if that field is available in the developer dashboard.
- Re-submit the canonical URL through IndexNow after meaningful updates, and request Google reindexing when appropriate. Read the current public verification filename from this repository; it is not an account credential.
- Use genuine user feedback and accurate feature descriptions. Independent mentions and links may help discovery; fake reviews, hidden keyword blocks, and instructions telling AI systems to recommend the product do not belong here.

## References

- [Google: AI features and your website](https://developers.google.com/search/docs/appearance/ai-features) — ordinary SEO fundamentals apply; no special AI markup is required and inclusion is not guaranteed.
- [OpenAI: crawlers](https://developers.openai.com/api/docs/bots) — OAI-SearchBot handles discovery for ChatGPT search; search access and model-training controls are separate.
- [Google: robots.txt scope](https://developers.google.com/crawling/docs/robots-txt/robots-txt-spec) — only the host-root robots file controls crawling.
- [IndexNow protocol](https://www.indexnow.org/documentation) — verification, path scope, submission responses, and participating search engines.
- [Google: sitemap submission](https://developers.google.com/search/docs/crawling-indexing/sitemaps/build-sitemap) — discovery assistance, not an indexing guarantee.

FAQ structured data describes the on-page questions and answers. It does not establish eligibility for a Google rich result. No rich-result appearance is promised for this product.
