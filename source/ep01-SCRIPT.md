# LostByte Ep01 — Why Does ChatGPT Make Things Up? AI Hallucinations Explained

Narrator: Byte (Kokoro, one voice). Sources: SOURCES.md. Any on-screen number carries a SOURCE: chip.

## Beat 1 (0:00) — Cold open
- Card: `Confident and wrong`
- Visual: bit_scene_mockup
- Sources: S2

Bit here had a simple question. Who wrote that famous paper on sleep and memory? The chatbot answered instantly. A real-sounding author, a journal, a year, even a page number. Bit pasted it into an essay, felt clever, and went to make toast. One problem. That paper does not exist. Never did. The chatbot made it up, and it sounded exactly as sure as when it tells you water is wet. So what just happened?

## Beat 2 (0:30) — Episode card
- Card: `Why AI makes things up`
- Visual: title_card
- Sources: —

Hey, I'm Byte, and this is LostByte Explained, episode one. Today's question: why does ChatGPT, and every chatbot like it, sometimes make things up? Not on purpose, and not because it's broken. By the end of this video you'll know three things. How these models actually produce an answer. Why their training quietly rewards confident guessing. And a handful of simple, free habits that catch most made-up answers before they catch you.

## Beat 3 (1:00) — Plain-English definition
- Card: `> hallucination = confident fiction`
- Visual: byte_bit_dialogue
- Sources: S1, S2

Bit asks me, so what's the official word for this? Researchers call it a hallucination. In plain English, that's when an AI produces something that sounds fluent and believable but is false, or isn't supported by the source it was given. The key part is the confidence. A hallucination doesn't come with a warning label. It reads just as smooth as a correct answer, which is exactly why it's so easy to believe, and easy to miss.

## Beat 4 (1:30) — Analogy
- Card: `Super-powered autocomplete`
- Visual: diagram_autocomplete
- Sources: S3

Here's the analogy I like best. You know the autocomplete on your phone, guessing your next word? Now imagine one trained on a huge share of the public internet, books and articles, so good it can finish whole essays. That's roughly what a chatbot is. Autocomplete doesn't look anything up. It predicts what usually comes next. Ask it for a citation, and it writes something shaped like a citation, whether or not one exists.

## Beat 5 (2:00) — How it works: step 1
- Card: `Words become tokens`
- Visual: diagram_tokens
- Sources: S3, S4

Step one. When you type a question, the model chops your text into small pieces called tokens. A token might be a whole word, part of a word, or punctuation. Each token becomes a list of numbers the model can work with. Then a neural network called a transformer looks at all those tokens together and works out how they relate, so it knows which earlier words matter most for predicting what comes next.

## Beat 6 (2:30) — How it works: step 2
- Card: `One token at a time`
- Visual: diagram_next_token
- Sources: S3, S2

Step two. The model scores every possible next token and picks a likely one. Then it adds that token to the text and does the whole thing again, one token at a time, until the answer is finished. Notice what's missing. At no point does it stop and check a database of facts. It's choosing what sounds most probable given everything it read in training. Usually probable and true line up. Sometimes they don't.

## Beat 7 (3:00) — How it works: step 3
- Card: `Guessing gets rewarded`
- Visual: diagram_test_scoring
- Sources: S2

Step three, the aha. OpenAI researchers compare it to a multiple choice test. If you leave a question blank, you get zero. If you guess, you might get lucky. A model asked for someone's birthday that it doesn't know has about a one in three hundred sixty-five chance if it guesses, and zero if it says I don't know. When tests only score accuracy, guessing wins the leaderboard. So models learn to guess, confidently.

## Beat 8 (3:30) — Myth busted
- Card: `Not lying. Not glitching.`
- Visual: myth_vs_fact
- Sources: S2, S5

Myth: the AI is lying to you, or it's a mysterious glitch. Neither is quite right. Lying means knowing the truth and hiding it. The model has no built-in truth check to hide from. And it's not mysterious either. Researchers can explain the statistics behind it. Rare, one-off facts, like a random person's birthday, can't be learned from patterns alone. Research also suggests models often carry some signal about what they don't know.

## Beat 9 (4:00) — Real-world example
- Card: `Fake citations, measured`
- Visual: counter_stat
- Sources: S6

Here's a real measurement. In a 2023 study, researchers asked ChatGPT to write short literature reviews on forty-two topics and checked all six hundred thirty-six citations. Fifty-five percent of the citations from GPT-3.5 were fabricated. For GPT-4, it was eighteen percent. Newer models do better, and these numbers are from 2023, so treat them as a snapshot. But the lesson holds. Even a much better model can still hand you references that simply don't exist.

## Beat 10 (4:30) — Why it matters to you
- Card: `Your time. Your trust.`
- Visual: amber_warning
- Sources: S1

So why should you care? Because you're the one who pays when a made-up answer slips through. Maybe it's a wrong dosage, a fake law, or a product spec that doesn't exist, and you lose time or money acting on it. Maybe it's a fake quote in a school essay or a work email with your name on it. The model won't take the blame. The fix is simple: treat confident answers as drafts, not verdicts.

## Beat 11 (5:00) — Honest caveats
- Card: `Better, not perfect`
- Visual: byte_honest_face
- Sources: S2, S7

Now, the honest caveats. Chatbots are genuinely useful, and they're right far more often than this video might make you feel. Training methods using human feedback have made them more truthful and better at following instructions. Newer models hallucinate less. But less isn't never. They're weakest on rare facts, exact numbers, quotes, citations, recent events and niche topics. Those are exactly the places where you should slow down and double-check before trusting anything.

## Beat 12 (5:30) — How to spot it
- Card: `Check the specifics`
- Visual: checklist
- Sources: S6, S8

How do you spot a fabrication? Watch for very specific details you didn't ask for: exact page numbers, precise statistics, named studies, direct quotes. Those are the easiest things to invent and the hardest to notice. Search for any citation yourself; if you can't find it, assume it's fake. Ask the same question twice in a new chat. If the details keep changing, that's a red flag. Real facts tend to stay put.

## Beat 13 (6:00) — Free settings to try
- Card: `Allow "I don't know"`
- Visual: terminal_prompt
- Sources: S8

Here are free fixes that work in any chatbot. First, give it permission to be unsure: add, if you don't know, say so. Anthropic's own guide recommends exactly that. Second, paste in the actual source document and ask it to answer only from that text. Third, ask it to quote the exact sentences that support each claim. If it can't find a supporting quote, tell it to take the claim back.

## Beat 14 (6:30) — Mini demo (mock-up)
- Card: `> answer only from source`
- Visual: labeled_mockup_chat
- Sources: S8

Quick demo, and this is a labeled mock-up, not a real screenshot. Bit asks, who wrote that sleep paper? Version one, no guardrails: a polished, invented citation. Version two, Bit pastes in the real article and writes: answer only from this text, quote your evidence, and say I don't know if it isn't there. Now the reply quotes the real author's line, or admits it can't find one. Same model. Very different honesty.

## Beat 15 (7:00) — What's coming next
- Card: `Look it up first`
- Visual: diagram_retrieval
- Sources: S9, S2

What's next? Two big ideas, both evergreen. One is retrieval: instead of answering from memory, the model searches real documents first and builds its answer on them, often with links you can check. The other is changing how models get graded, so confident wrong answers cost more than saying I'm not sure. Neither makes hallucinations vanish completely. But together they push chatbots toward admitting what they don't know.

## Beat 16 (7:30) — Recap
- Card: `Predicts. Guesses. Verify.`
- Visual: recap_three_points
- Sources: S2, S3

Let's recap in three points. One: a chatbot predicts likely words, one token at a time. It doesn't look facts up unless it's connected to a source. Two: training and testing have rewarded confident guessing over saying I don't know, so when it's unsure, it often guesses anyway. Three: you can fight back. Give it permission to be unsure, give it real sources, ask for quotes, and verify anything specific yourself.

## Beat 17 (8:00) — Byte's Takeaway
- Card: `Trust, but verify`
- Visual: takeaway_card
- Sources: S2, S8

Byte's Takeaway. Should you stop using chatbots because they make things up? Nope. Keep them, but change the job you give them. They're brilliant first drafters, explainers and brainstorm partners. They're unreliable fact checkers. So here's my verdict: use it to think, not to cite. Anything with a name, a number, a date or a quote gets checked against a real source before it leaves your screen. That's the whole trick.

## Beat 18 (8:30) — Bookend
- Card: `Bit checks the source`
- Visual: bit_scene_resolved
- Sources: S6

Back to Bit and that sleep paper. This time, Bit asks again and adds: if you're not sure, say so. The chatbot admits it can't confirm the author. Bit searches the title, finds no such paper, and picks a real study from the library database instead. Essay saved, toast only slightly burnt. Now, your turn. What's the wildest thing a chatbot has confidently told you? Drop it in the comments, and subscribe for episode two.
