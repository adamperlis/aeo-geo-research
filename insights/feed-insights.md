# Distilled AEO / SEO / GEO Insights

> **What this is:** durable AEO/SEO/GEO insights, auto-distilled each week from public
> SEO/marketing sources (vendor blogs, studies, official docs) and published automatically.
> Each entry cites its source so you can weigh it.
>
> **Trust level:** Lower than a hand-curated core. These come from vendor blogs (Semrush,
> Ahrefs, HubSpot, Search Engine Land, etc.) and may carry marketing bias. When an entry
> conflicts with a well-established study, treat the study as the stronger evidence.
>
> **Consumed by:** the open-source `seo-aeo-geo` Claude skill, which fetches `index.md`
> then the docs below. Newest entries on top.

---

<!-- ===== proposed 2026-11-09 (from 25 new article(s)) ===== -->
## Proposed 2026-11-09

#### Competitors Can Hijack Your Branded AI Overviews

- **21.7% of Google AI Overviews triggered by branded buying queries cite a competitor; when buyers ask AI to compare you to a rival, the AI builds its answer from whatever comparison evidence exists — which may be your competitor's own page**
  - Extends the core's "build comparison pages for competitors agents name" principle in a new direction: a competitor can actively shape what AI says about *your brand* when your brand is the query. Monitor branded AI Overviews weekly via GSC AI performance report + manual prompts. For every competitor running "X vs. [your brand]" pages, publish a counter-narrative on your own domain and ensure it ranks. In the ATS vertical example, Ashby's comparison page was cited when buyers searched for Greenhouse.
  - _Source: Foundation Marketing (The Lab Vol. 314, Writesonic data), 2026-10-19 — https://foundationinc.co/lab/vol-314; also Vol. 312, 2026-10-06 — https://foundationinc.co/lab/vol-312_

#### Technical Documentation Is the Dominant First-Party AI Citation Source for Developer/SaaS Products

- **For technical products, owned documentation beats owned blog content as a first-party AI citation source — Docker's data shows 54% of its AI citations come from docs, even during product-comparison queries**
  - The core's citation channel map (Reddit 20.8%, YouTube 13%, etc.) describes third-party sources. This finding adds the first-party picture: for developer/SaaS products, docs — not blog posts — are the highest-leverage owned asset. Treat documentation as a primary AEO surface: structure docs to answer buyer-intent questions (integrations, comparisons, use cases), ensure they're publicly crawlable (not behind auth), and apply the same H2/H3 extractability standards the core recommends for blog content.
  - _Source: Foundation Marketing (The Lab Vol. 311), 2026-09-28 — https://foundationinc.co/lab/vol-311_

#### Simple Original-Data Pages Outperform Comprehensive Reports for AI Citation

- **A short page built around a single original data finding is cited by AI more reliably than a large industry report covering the same topic**
  - AI engines favor extractability over comprehensiveness. A concise page with one clear, citable stat has high signal-to-noise; a 10,000-word annual report buries the finding. When building data assets for citation purposes, publish individual findings as dedicated, stand-alone pages — each finding gets its own URL and clean extractable structure — rather than consolidating everything into an omnibus report. Counterintuitive but consistent with the core's FSA "Structure" lens.
  - _Source: Brian Dean/Backlinko via Semrush, 2026-09-24 — https://www.youtube.com/watch?v=4a-W0liaIlU (vendor video, moderate trust)_

#### Vibe-Coded Sites Systematically Violate the Initial-HTML Requirement

- **AI-generated ("vibe-coded") websites introduce a recurring AEO failure mode: each iterative prompt can silently shift existing content from server-rendered HTML to client-side JS without the builder noticing**
  - The core already requires server-rendered HTML for AI crawlability. Vibe-coded sites add a new failure pattern: the site launches clean, then a later AI-assisted edit (adding an image gallery, a testimonials section, a data table) inadvertently wraps prior content in a JS component. Audit by viewing raw page source — not DevTools — after every significant AI-assisted change. If key headings and body text are absent from the raw HTML, they're invisible to AI crawlers.
  - _Source: Search Engine Land, 2026-11-03 — https://searchengineland.com/technical-seo-checks-vibe-coded-websites-500033_

#### Price-Modifier Keywords Are Structurally Undercompeted

- **Keywords using "cheap," "affordable," "budget," or "low-cost" are systematically underserved because brands avoid price-qualifier language — but users search those terms heavily, and ranking for them also drives ranking for "best" variants**
  - Brands self-censor price qualifiers to protect premium positioning, creating a keyword gap searchers exploit. Placing a price modifier in the page title (the most visible element for clicks) captures high-intent, conversion-ready traffic with minimal competition. Applies to informational and commercial pages alike. Practical: add one dedicated page per price-modifier variant of your top commercial keyword where conversion intent is high.
  - _Source: Edward Sturm (via James Dooley), 2026-08-11 — https://edwardsturm.com/articles/2-easy-seo-tricks-cheap-modifier-micro-influencers/_


<!-- ===== proposed 2026-06-22 (from 25 new article(s)) ===== -->
## Proposed 2026-06-22

#### Schema as Agentic Infrastructure

- **Schema markup now serves dual roles: entity identification for AI Overviews AND enabling AI agents to act on content; structured data also reduces inference cost for LLMs operating within finite context windows**
  - As AI agents complete tasks on behalf of users (compare, recommend, book), they need schema not just to *understand* content but to *act on it* — relationships, trustworthiness, and actionability signals. Separately, parsing unstructured HTML is computationally expensive; clean structured data lowers inference cost per page, making schema-rich sites more likely to be fully processed at scale. This is a new efficiency-based argument for schema investment that complements the entity/crawl arguments already in the core. Note: Google's official guide says schema is "not required for AI features" (meaning ranking signals for Overviews) — this is a separate use case for agentic AI interactions beyond Overviews.
  - _Source: Search Engine Land, 2026-06-01 — https://searchengineland.com/schema-markup-optimize-agentic-web-479080_

#### AI Citation Tracking Requires Statistical Rigor

- **Because LLMs give probabilistic answers, a single prompt run is near-meaningless for tracking; run repeated queries with fixed sampling rules and calculate confidence intervals to produce defensible citation-rate numbers**
  - "AI mentioned us 3 out of 5 times" is noise; "we have a 60% ± N% citation rate across 30 consistent runs" is a trackable metric that can detect real improvement vs. variance. This is the measurement standard needed before reporting AEO progress to stakeholders. Complements the existing GSC AI performance insight (which is Google-only) by extending rigorous measurement to ChatGPT, Perplexity, and other engines where you track manually.
  - _Source: Growth Memo (Kevin Indig), 2026-06-08 — https://www.growth-memo.com/p/how-to-make-prompt-tracking-much_

#### Engine-Specific Citation Domain Fingerprints

- **Each major AI engine (Copilot, Gemini, AI Overviews, Grok, Perplexity) has a structurally distinct and stable top-cited domain set — off-site channel strategy must be engine-specific, not engine-agnostic**
  - Ahrefs' June 2026 "50 Most-Cited Domains" series across five engines documents that the sources each engine preferentially cites differ in consistent patterns. The core's existing "citation fingerprint is vertical-specific" principle extends further: it is *also* engine-specific in structural ways. Before investing in an off-site channel, run target-engine citation analysis for your specific vertical to verify that channel actually gets cited by *that* engine — not just by "AI" broadly. A channel that dominates Perplexity citations may be nearly absent from Gemini's top sources.
  - _Source: Ahrefs (five-engine citation series), 2026-06-01 — https://ahrefs.com/blog/most-cited-domains-perplexity/ (see also /copilot/, /gemini/, /most-cited-domains-ai-overviews/, /most-cited-domains-grok/)_


<!-- ===== proposed 2026-06-29 (from 13 new article(s)) ===== -->
## Proposed 2026-06-29

#### Measurement: AI "Share of Voice" Scores Are Unfalsifiable

- **Vendor AI visibility platforms present precise-looking percentages that have no valid denominator — the AI prompt universe is infinite and personalized, so no cross-platform SOV score can be audited or validated**
  - Unlike keyword-set SOV (fixed list, transparent assumptions), AI prompt space is unbounded and varies by session, user, and context. A single percentage obscures what was and wasn't tested. In AEO audits, replace vendor SOV scores with auditable proxies: GSC AI performance report data, manual prompt panels targeting real buyer queries, and brand-mention tracking separated from URL citation counts.
  - _Source: Search Engine Land, 2026-06-08 — https://searchengineland.com/ai-share-of-voice-metrics-that-matter-more-479611_

#### Technical: Server Logs Are Now the Authoritative AI Crawler Audit Tool

- **Server logs capture every GPTBot, Applebot, and AI crawler request that GSC, analytics, and third-party crawlers miss — on large sites, they reveal AI crawl access problems before they show up in any ranking signal**
  - Every bot request logs URL, response code, user agent, and timestamp. GSC and crawl simulators operate on samples or delayed data; logs are the ground truth. For sites with complex JS routing, paywalls, or aggressive caching, analyzing GPTBot/Applebot behavior in logs is now a distinct audit step — not covered by a standard Screaming Frog crawl.
  - _Source: Search Engine Land, 2026-06-09 — https://searchengineland.com/server-logs-reveal-what-seo-tools-miss-479650_

#### Ghost Citations: AI Engines Cite Domains Without Mentioning the Brand

- **In a 4-engine study (ChatGPT, Gemini, Google AI Overviews, AI Mode, n=3,981 domain appearances), 62% of AI citations were "ghost citations" — the URL was cited but the brand name never appeared in the response text**
  - URL citation and brand mention are distinct AEO outcomes with different business value. A ghost citation influences nothing the reader sees. To convert citations into brand mentions: strengthen entity signals (consistent Organization schema sitewide, `sameAs` cross-links, repeated brand-name attribution in third-party sources) and write content that names the brand explicitly in extractable summary positions — not just in body copy.
  - _Source: Semrush / Kevin Indig, 2026-06-09 — https://www.semrush.com/blog/the-ghost-citations-study/ (vendor study, moderate trust — methodology disclosed)_


<!-- ===== proposed 2026-06-17 (deduped, 25 new articles) ===== -->
## Proposed 2026-06-17 — backlog catch-up (deduped)

#### Zero-Click Is Now the Default — Hard Numbers  ✅ Safe

- **68% of U.S. Google searches ended without a click in early 2026 (up from 60.45% in 2024); AI Overviews cut CTR ~60% when present, and now appear on 20%+ of queries**
  - SparkToro/Similarweb clickstream data (Jan–Apr 2026) quantifies what the core's mental model describes qualitatively. Reframe audit KPIs: traffic ≠ visibility, and citation-in-answer is the primary objective, not clicks. Zero-click is structural, not a temporary dip.
  - _Source: Search Engine Land (SparkToro/Similarweb), 2026-06-09 — https://searchengineland.com/google-zero-click-searches-2026-study-479717_

#### ChatGPT Fetches Reddit at Query Time (mechanism refinement)  ✅ Safe (moderate trust)

- **ChatGPT issues retrieval queries *naming Reddit* before it answers — Reddit influence is active, query-time grounding, not just training-data exposure**
  - Refines the existing insight "Reddit shapes ChatGPT's understanding but rarely gets the citation": the shaping happens through live, upstream retrieval at inference, then ChatGPT attributes the answer to an institutional source. Tactical implication: Reddit presence must be *findable by a search query*, not just crawlable — and it's a real-time signal, not only a slow brand-building play.
  - _Source: Foundation Marketing (The Lab Vol. 295, Profound data), 2026-06-04 — https://foundationinc.co/lab/vol-295/_

#### GSC Now Has AI Visibility Measurement + Control  ✅ Safe

- **Google Search Console added a dedicated AI performance report (AI Overview impressions/clicks/CTR) and a per-page toggle to block content from AI-generated responses**
  - These are now the authoritative first-party tools for measuring and controlling AI Overview visibility — more direct than inferring from organic CTR drops. Make "GSC → AI performance report" the primary measurement step in any AEO audit. The block toggle is a new publisher lever for content where uncontextualized citation creates risk (paywalled/exclusive/thin pages).
  - _Source: Semrush blog (Google announcement), 2026-06-03 — https://www.semrush.com/blog/google-adds-ai-performance-reports/_

#### Lighthouse Now Audits "Agentic Browsing" Readiness  ✅ Safe

- **Google added an Agentic Browsing audit category to Lighthouse — sites are now formally scored on whether AI agents can navigate and act on them**
  - A new technical axis beyond crawlability: agents must be able to follow links, reach key content, and interact with forms without hitting JS-rendering walls. Overlaps existing AEO foundations (server-side rendering, semantic HTML, no JS-only critical paths) but extends into interactive surfaces. Run a Lighthouse Agentic Browsing audit alongside Core Web Vitals on complex sites (SPAs, gated content, heavy client-side routing).
  - _Source: Semrush blog (Google announcement), 2026-06-03 — https://www.semrush.com/blog/google-adds-agentic-browsing-category-to-lighthouse/_

#### Google AI Mode Queries Are ~3× Longer (extends fan-out)  ✅ Safe

- **AI Mode (1B+ monthly users) queries average ~3× the length of traditional searches — content tuned to short-tail keywords is mismatched to compound, conversational intent**
  - Extends the existing fan-out title-relevance principle to Google's own AI surface. Practical: structure H1/H2 headings and opening paragraphs to mirror how someone describes a full problem in a sentence, not a two-word keyword.
  - _Source: Search Engine Land (Google Marketing Live 2026), 2026-06-08 — https://searchengineland.com/google-ai-brief-replacement-keywords-479576_

#### UCD Brand-Signal Framework (complements FSA)  ✅ Safe

- **AI forms brand opinions through three filters — Understandability, Credibility, Deliverability (UCD) — and the operational expertise that makes a business valuable is rarely published where AI can see it**
  - Understandability: clear about/product pages + structured data. Credibility: experience/expertise/authority/trust signals. Deliverability: surfaced for the right queries at the right moment. UCD complements FSA — FSA is about *content to produce*, UCD is about *signals AI infers from your footprint*. The high-leverage gap: convert internal/operational knowledge (methodology, process docs, expert-attributed case studies) into crawlable content. Apply both lenses in a brand AEO audit.
  - _Source: Search Engine Land, 2026-06-09 — https://searchengineland.com/how-ai-forms-opinions-about-your-brand-479671_

#### Google Officially Flags "AEO/GEO Tool" Claims as Skepticism-Worthy  ✅ Safe (validates core)

- **Google's third-party guidance doc now lists tools "promising improvements for AI experiences and search formats (AEO/GEO tools)" alongside other claims to evaluate critically — no tool has privileged access to AI feature signals**
  - Google-official validation of the skill's anti-snake-oil stance: core quality signals remain the primary lever. When advising clients evaluating third-party AEO tools, cite this doc — it shifts the burden of proof onto the vendor.
  - _Source: Search Engine Land (Google docs update), 2026-06-07 — https://searchengineland.com/google-adds-guidance-on-third-party-seo-tools-services-advice-and-updates-hiring-an-seo-doc-479637_

#### AI Search Is the Top Purchase-Intent Signal in B2B Discovery  ✅ Safe (moderate trust)

- **AI search was the #1 predictor of purchase intent for CRM software buyers; AI-referred traffic converts higher despite lower volume — the zero-click trade-off is leads-quality-positive for B2B**
  - AI-briefed visitors arrive further down the consideration funnel. For B2B SaaS, appearing in AI consideration-phase answers can matter more than organic traffic volume. Map content to the queries buyers run during *shortlist formation* (reinforces the core's shortlist-position insight), not just awareness queries.
  - _Source: HubSpot State of AEO 2026, 2026-06-01 — https://blog.hubspot.com/marketing/ai-search-behavior — (moderate trust — vendor report)_


<!-- ===== proposed 2026-06-01 web (Perplexity source selection) ===== -->
## Proposed 2026-06-01 — Perplexity engine (web research)

#### Perplexity Rewards Freshness + Niche Topical Authority  ✅ Safe (moderate trust)

- **Perplexity is a RAG engine with a strong recency bias and a preference for niche topical authority over generic domain strength**
  - Two-stage pipeline: retrieve (query match + authority signals) → rank for the most specific, accurate, well-structured answer. Averages ~5.3 cited sources per answer with a strong skew toward content published in the last ~12 months. A niche site with deep vertical expertise can out-cite a high-DA generalist. Practical: keep target pages genuinely fresh (real updates + `dateModified`) and build demonstrable topical depth in your vertical rather than chasing broad domain authority.
  - _Source: synthesized from multiple 2026 Perplexity citation analyses (AuthorityTech, SearchPilot, Stackmatix) — moderate trust; cross-source synthesis, not a single hard-data study_

#### Perplexity Favors Unique, Well-Structured, News-Style Content  ✅ Safe (moderate trust)

- **When sources overlap, Perplexity cites the one with unique information and clean structure; news/journalism content dominates its citations**
  - It preferentially cites original research, proprietary data, case studies, expert interviews, or novel frameworks over commodity rehashes, and clear heading hierarchy / extractable structure raises citation odds. Practical: lead pages with a distinct original angle and structure for extractability — this is the FSA "Structure" + "Freshness" lenses applied specifically to Perplexity.
  - _Source: synthesized from multiple 2026 Perplexity citation analyses — moderate trust_


<!-- ===== proposed 2026-06-01 backlog (ChatGPT citation study) ===== -->
## Proposed 2026-06-01 — backlog deep-read (LLM-assistant engines)

#### ChatGPT Citation Requires Ranking in Classic Search  ✅ Safe

- **To be cited by ChatGPT, you generally must first rank in traditional web search — it's the dominant supply channel**
  - In a 1.4M-prompt study, 88% of ChatGPT's actual citations came from the "search" retrieval channel (88.46% citation rate). Reddit/YouTube/academia are pulled in at scale but cited <2% of the time, and ChatGPT cites only ~50% of the URLs it retrieves. Practical: classic SEO ranking is the price of entry for ChatGPT visibility.
  - _Source: Ahrefs (Louise Linehan), 2026-04-15 — https://ahrefs.com/blog/why-chatgpt-cites-pages/_

#### Reddit Shapes ChatGPT's Understanding but Rarely Gets the Citation  ❗ Nuances core

- **Per-engine split: Reddit drives AI *consensus/context*, but owned/institutional ranked pages earn the actual ChatGPT *citation***
  - Reddit has its own retrieval channel (16M+ data points) yet is cited only 1.93% of the time; 67.8% of all non-cited URLs are Reddit. ChatGPT "learns from the crowd, then cites another institution." This nuances the core's 57M-citation study (where Reddit is the top channel): the two measure different things — overall AI citations across engines vs. ChatGPT-specific cited sources. Treat Reddit as an *influence* play, not a *citation* play, for ChatGPT.
  - _Source: Ahrefs (Louise Linehan), 2026-04-15 — https://ahrefs.com/blog/why-chatgpt-cites-pages/_

#### Title–Fan-out Relevance Drives ChatGPT Selection  ✅ Safe

- **Match titles/headings to ChatGPT's internal fan-out sub-questions, not just the head keyword**
  - Cited pages showed much higher cosine similarity between their title and the query's fan-out sub-questions (max-match 0.656) than non-cited pages (~0.48). A pre-fetch gatekeeping layer uses title + URL + snippet to decide which retrieved URLs to even open. Practical: phrase H1/title and section headings to mirror the specific sub-questions a topic fans out into.
  - _Source: Ahrefs (Louise Linehan), 2026-04-15 — https://ahrefs.com/blog/why-chatgpt-cites-pages/_


<!-- ===== proposed 2026-06-01 (from 5 new article(s)) ===== -->
## Proposed 2026-06-01

#### LLM Query Classification Determines Retrieval Strategy

- **Segment content by query type: "what's true now" triggers live search; "how things work" relies on training data**
  - LLMs fire real-time web searches for time-sensitive queries (prices, rankings, comparisons, current events) but answer conceptual/definitional queries from training data alone. This means freshness infrastructure (`dateModified`, frequent updates, crawlability) matters most for transactional/comparative content, while depth and entity consistency matter more for evergreen how-to content.
  - _Source: Edward Sturm, March 21, 2026 — (no URL in article)_
