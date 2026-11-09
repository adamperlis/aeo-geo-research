# AEO / SEO / GEO Research Index

Machine-readable index of the research documents in this repo. The open-source
`seo-aeo-geo` Claude skill fetches this file first, then the doc(s) most relevant to the
user's question.

_Last updated: 2026-11-09 (auto-published)._

## Documents

- **insights/feed-insights.md** — Weekly-distilled AEO/SEO/GEO insights from public
  sources (vendor blogs, studies, official docs), each entry cited. Lower-trust than
  well-established studies; newest on top.
  - raw: https://raw.githubusercontent.com/adamperlis/aeo-geo-research/main/insights/feed-insights.md

## How to use

Fetch a doc's `raw:` URL over HTTP (or via an agent's WebFetch). Files are plain Markdown.
Content is auto-published weekly; weigh each entry on the source it cites.
