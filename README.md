# LostByte AI Field Guide

Plain static HTML/CSS companion site for the [LostByte YouTube channel](https://www.youtube.com/@lostbyte2). No build step: GitHub Pages serves the files as-is.

Live (once Pages is on): https://sm902932-yo.github.io/lostbyte-field-guide/

## Layout
- `index.html`: home (latest episode + start here)
- `episodes/ep01/`, `episodes/ep02/`: episode hubs (chapter → page table + full source list)
- `terms/<slug>/`: glossary pages (hallucination, retrieval, token, next-token-prediction, embeddings, attention, rlhf, temperature)
- `explainers/<slug>/`: question pages (why-chatbots-guess, spot-fabrications, reduce-hallucinations, how-chatgpt-is-trained)
- `tools/`: free tools (openai-tokenizer); sponsor slots reserved, empty
- `about/`: about + AI disclosure; `newsletter/`: placeholder form (posts nowhere)
- `ep01/`, `ep02/`: short redirects to the hubs
- `style.css`: the single shared stylesheet
- `sitemap.xml`, `robots.txt`, `.nojekyll`
- `source/`: episode scripts and SOURCES files the pages are checked against

## Page template
Plain answer → Byte & Bit analogy → key terms → sources → watch the video (timestamps) → related pages.

## Rules
Every fact or number must come from `source/epNN-SOURCES.md` and is cited as `[EpNN S#]`, linking to the page's source list. All links are relative so the site works under `/lostbyte-field-guide/`.

## Local preview
Open `index.html` in a browser, or run `python3 -m http.server` in the repo root.

## Pages setup
Settings → Pages → Source: Deploy from a branch → `main` / `(root)`.
