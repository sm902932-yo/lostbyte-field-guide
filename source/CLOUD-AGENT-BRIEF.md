# LostByte AI Field Guide v1 — cloud agent brief

Target repo (once it exists): https://github.com/sm902932-yo/lostbyte-field-guide (public)
Host: GitHub Pages (Actions), free. No paid domain. No backend.
Stack: Astro + Markdown content. Do not build on the shared box.

## Goal
Ship a static companion site for the LostByte YouTube channel before Sun Oct 18 2026 5:30 PM CT (Ep02 upload). QC every page against the script SOURCES before publish.

## Source materials on the box (copy into the repo)
- /workspace/lostbyte/field-guide/launch/PLAN.md
- /workspace/lostbyte/field-guide/launch/ep01-SCRIPT.md
- /workspace/lostbyte/field-guide/launch/ep01-SOURCES.md
- /workspace/lostbyte/field-guide/launch/ep02-SCRIPT.md
- /workspace/lostbyte/field-guide/launch/ep02-SOURCES.md

## Site structure
/, /terms/, /explainers/, /episodes/epNN/, /tools/, /about/ (AI disclosure), /newsletter/
Page template: plain answer (2-3 sentences) -> Byte & Bit analogy -> key terms -> sources (same S# as script) -> watch embed + timestamp -> related pages
Short redirects: /ep01 and /ep02 -> hubs

## First 15 pages (build order)
1. Ep01 hub + explainers/terms for hallucinations, why chatbots guess, spot fabrications, reduce hallucinations
2. Then Ep02 hub + token, next-token, embeddings, attention, training, RLHF, temperature, OpenAI Tokenizer tool page
Full table is in PLAN.md

## Constraints
- Facts and numbers only from SOURCES files. No unsourced claims.
- $0: no paid services, no custom domain unless Samuel OKs later
- Newsletter signup form can be a placeholder that posts nowhere until a free provider is wired
- Sponsor slots on /tools/ reserved but empty in v1
- Samuel approves every outgoing email and sponsor deal (do not send anything)

## Done when
- Pages Actions deploys to https://sm902932-yo.github.io/lostbyte-field-guide
- Homepage returns 200
- Ep01 and Ep02 hubs live with linked concept pages from the first batch
- README explains local build and Pages setup
