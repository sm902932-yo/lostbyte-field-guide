# LostByte AI Field Guide — Plan v1 (2026-10-15)

## 1. Site plan
**Structure:** `/` home (latest episode + "start here") · `/terms/` glossary · `/explainers/` one page per question · `/episodes/epNN/` hubs · `/tools/` free-tools directory (sponsor slots reserved, empty in v1) · `/about/` (incl. AI disclosure) + `/newsletter/` (signup form).

**Page template:** Plain answer (2–3 sentences) → Byte & Bit analogy → Key terms (links into /terms/) → Sources (same S# list the script uses) → Watch the video (embed + timestamp) → Related pages.

**First 15 pages:**
| # | Title | Slug | Ep |
|---|---|---|---|
| 1 | Ep01 hub: Why Does ChatGPT Make Things Up? | /episodes/ep01/ | 01 |
| 2 | Ep02 hub: How Does ChatGPT Actually Work? | /episodes/ep02/ | 02 |
| 3 | What is an AI hallucination? | /terms/hallucination/ | 01 |
| 4 | Why do chatbots guess instead of saying "I don't know"? | /explainers/why-chatbots-guess/ | 01 |
| 5 | How to spot a made-up AI answer (fake citations) | /explainers/spot-fabrications/ | 01 |
| 6 | Free prompt fixes that reduce made-up answers | /explainers/reduce-hallucinations/ | 01 |
| 7 | What is retrieval (RAG)? | /terms/retrieval/ | 01 |
| 8 | What is a token? | /terms/token/ | 01+02 |
| 9 | Next-token prediction, explained | /terms/next-token-prediction/ | 01+02 |
| 10 | Word maps (embeddings): king − man + woman | /terms/embeddings/ | 02 |
| 11 | Attention: the highlighter | /terms/attention/ | 02 |
| 12 | How ChatGPT is trained (fill-in-the-blank + parameters) | /explainers/how-chatgpt-is-trained/ | 02 |
| 13 | Human feedback coaching (RLHF) | /terms/rlhf/ | 01+02 |
| 14 | Why ChatGPT gives different answers (temperature) | /terms/temperature/ | 02 |
| 15 | Tools: OpenAI Tokenizer (free, no login) | /tools/openai-tokenizer/ | 02 |

**Video linking:** description gets hub link + 2–3 concept links; pinned comment links the hub; each chapter maps to a page (hub lists chapter → page); end-screen/outro CTA "full guide at [site]/epNN"; short, UTM-free paths (`/ep01`, `/ep02` redirect to hubs).

## 2. Hosting / build
Static site (Astro preferred; Eleventy fine), Markdown content, no backend. New GitHub repo built by a Cursor cloud agent (nothing built on the box — disk 96% full). Host on **GitHub Pages (free)** → `<username>.github.io/lostbyte-field-guide` (custom domain later). Vercel free (`*.vercel.app`) works too but needs a new account connection; GitHub is already connected, so Pages wins.
**Samuel must approve:** (a) repo owner account + name (proposed `lostbyte-field-guide`), (b) making it public, (c) enabling Pages (Actions deploy), (d) any later custom domain/DNS.

## 3. Lean routines
- **Daily (1 check):** new episode script drafted/locked? → queue its page drafts via Head of Content; site uptime check (homepage 200).
- **Weekly (Mon):** page backlog + QC status, traffic note if analytics exist, sponsor pipeline summary to Jessica.

## 4. Newsletter & sponsors
Free tier (Buttondown, Beehiiv, or Kit). Signup form live from v1; first issue after ~5 episodes or 100 signups. Sponsors: directory listing slots on /tools/, "Tool of the week" in newsletter + site, rate card once traffic exists. All outreach drafted → Jessica → Samuel approves before anything is sent. Sponsored items clearly labeled.

## 5. ETA
v1 live ~24h after repo/Pages approval. Every page passes QC (facts match script SOURCES, no unsourced numbers) before publishing. Order: Ep01 hub + pages 3–6 first, then Ep02 set before Sun Oct 18 upload.
