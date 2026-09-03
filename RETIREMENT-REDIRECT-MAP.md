# gvancouverhomes.com Retirement Redirect Map

Status: staging only on `gvancouverhomes-retirement`. Do not merge to `main` until domain-level redirects are configured and tested.

## Primary permanent redirects

- `/` -> `https://tanvirbhupal.com/`
- `/about/` -> `https://tanvirbhupal.com/about/`
- `/contact/` -> `https://tanvirbhupal.com/contact/`
- `/blog/` -> `https://tanvirbhupal.com/articles/`
- `/search/` -> `https://tanvirbhupal.com/buying/`
- `/thanks/` -> `https://tanvirbhupal.com/contact/`

## Old posts

- `/2025/08/11/it-starts-here/` -> `https://tanvirbhupal.com/about/`
- `/2026/01/19/surrey-detached-price-floor-2026/` -> `https://tanvirbhupal.com/buying/`
- `/2026/01/16/south-surrey-land-value-shift/` -> `https://tanvirbhupal.com/articles/`

## Legacy utility/legal pages

These do not have true one-to-one equivalents on the new site and should not be treated as priority SEO transfers:

- `/privacy/`
- `/terms/`
- `/accessibility/`

If the retirement is implemented with a domain-wide fallback redirect, these may fall back to `https://tanvirbhupal.com/`. If a 410/explicit retirement response is available at the edge, that is cleaner for non-equivalent low-value URLs.

## Implementation rule

Use real HTTP permanent redirects at the domain edge rather than replacing the old GitHub Pages content with JavaScript or meta-refresh redirects.

Keep the old GitHub repository intact as the historical backup until the redirect migration is verified.
