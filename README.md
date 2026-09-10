# aeo-geo-research

Auto-published, weekly-refreshed research feed for **AEO** (Answer Engine Optimization),
**SEO**, and **GEO** (Generative Engine Optimization).

Each week a distiller reads fresh public sources — vendor studies, SEO/marketing blogs,
official search docs — and summarizes the genuinely new, durable findings into cited,
trust-labeled insights. The result is published here automatically. No editorializing beyond
"is this new, durable, and sourced."

## What's here

- **[`index.md`](index.md)** — machine-readable manifest. Start here: it lists every research
  doc with its raw URL and a one-line summary.
- **[`insights/feed-insights.md`](insights/feed-insights.md)** — the distilled insights,
  newest on top, each with a `Source:` line so you can weigh it.

## Who consumes it

The open-source [`seo-aeo-geo`](https://github.com/adamperlis/claude-skill-seo-aeo-geo) Claude
skill fetches `index.md` (raw) as its first step, then pulls the doc(s) most relevant to the
question. Anything that can fetch a raw Markdown URL can use it — an agent's web-fetch tool,
`curl`, a script:

```bash
curl -s https://raw.githubusercontent.com/adamperlis/aeo-geo-research/main/index.md
```

## Trust & caveats

- These are **distilled summaries of third-party sources**, not original text — every entry
  cites where it came from. When an insight conflicts with a well-established study, treat the
  study as the stronger evidence.
- Sources skew toward vendor blogs (Semrush, Ahrefs, HubSpot, Search Engine Land, etc.) and
  may carry marketing bias. The distiller filters out obvious product pitches, but weigh each
  entry on its source.
- Published automatically on a weekly cadence. Content reflects what was true when distilled.

## License

MIT © Adam Perlis. See [LICENSE](LICENSE). Distilled insights link to their original sources,
which remain the property of their respective publishers.
