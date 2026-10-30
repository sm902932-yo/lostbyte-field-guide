# LostByte Ep02 — Sources
URLs checked 2026-10-13 ~19:10 CT: arXiv pages HTTP 200 via curl; S1 and S12 (help.openai.com, 403 to curl) verified via WebFetch. Quoted facts were checked against the paper text/abstract.

| id | Title | Publisher / Author | Year | URL | Used for |
|---|---|---|---|---|---|
| S1 | Understanding and counting tokens | OpenAI Help Center | living doc (checked 2026-10-13) | https://help.openai.com/en/articles/4936856-what-are-tokens-and-how-to-count-them | Tokens = pieces of words; 1 token ≈ ¾ word, 100 tokens ≈ 75 words (rough English estimate); free Tokenizer page |
| S2 | Neural Machine Translation of Rare Words with Subword Units | Sennrich, Haddow, Birch, ACL | 2016 | https://arxiv.org/abs/1508.07909 | Rare/long words split into sub-word pieces |
| S3 | Efficient Estimation of Word Representations in Vector Space | Mikolov, Chen, Corrado, Dean (Google) | 2013 | https://arxiv.org/abs/1301.3781 | Words as points in a meaning space; king − man + woman ≈ queen |
| S4 | Attention Is All You Need | Vaswani et al. (Google), NeurIPS | 2017 | https://arxiv.org/abs/1706.03762 | Attention ("highlighter"); Transformer design |
| S5 | Language Models are Few-Shot Learners (GPT-3) | Brown et al., OpenAI, NeurIPS | 2020 | https://arxiv.org/abs/2005.14165 | Next-word prediction training on large text; GPT-3 = 175 billion parameters |
| S6 | Scaling Laws for Neural Language Models | Kaplan et al., OpenAI | 2020 | https://arxiv.org/abs/2001.08361 | Performance improves predictably (power law) with model size, data and compute |
| S7 | The Curious Case of Neural Text Degeneration | Holtzman et al., ICLR | 2020 | https://arxiv.org/abs/1904.09751 | Always picking the most likely word gives bland/repetitive text → sampling randomness |
| S8 | Deep Reinforcement Learning from Human Preferences | Christiano et al., NeurIPS | 2017 | https://arxiv.org/abs/1706.03741 | Learning from human comparisons of outputs |
| S9 | Training language models to follow instructions with human feedback (InstructGPT) | Ouyang et al., OpenAI, NeurIPS | 2022 | https://arxiv.org/abs/2203.02155 | Human-feedback coaching; 1.3B InstructGPT preferred over 175B GPT-3 ("100x fewer parameters") |
| S10 | Why Language Models Hallucinate | Kalai, Nachum, Vempala, Zhang, arXiv | 2025 | https://arxiv.org/abs/2509.04664 | One-line Ep01 callback in beat 11 |
| S11 | Toolformer: Language Models Can Teach Themselves to Use Tools | Schick et al. (Meta AI), NeurIPS | 2023 | https://arxiv.org/abs/2302.04761 | Models learning to call tools such as a calculator and search engines (beat 15) |
| S12 | Searching the web with ChatGPT | OpenAI Help Center | living doc (checked 2026-10-13) | https://help.openai.com/en/articles/9237897-chatgpt-search | ChatGPT can search the web and cite sources with links (beats 8, 15) |
| S13 | Tokenizer (interactive tool) | OpenAI Platform | live tool (checked 2026-10-13) | https://platform.openai.com/tokenizer | Public, no login; "Why does ChatGPT make things up?" = 8 tokens / 32 characters, split Why\| does\| Chat\|GPT\| make\| things\| up\|? ; page text: "one token generally corresponds to ~4 characters of text for common English text. This translates to roughly ¾ of a word (so 100 tokens ~= 75 words)." Verified by HoP in a real browser 2026-10-13 (curl/WebFetch blocked by bot check); screenshot: /workspace/lostbyte/ep02/script/tokenizer_check.png (beat 13) |
