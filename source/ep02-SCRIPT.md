# LostByte Ep02 — How Does ChatGPT Actually Work? (No Jargon)

**STATUS: LOCKED — 2026-10-13 18:58 CT**

Narrator: Byte (Kokoro af_heart). Sources: SOURCES.md. Any on-screen number carries a SOURCE: chip.

## Flags

**Short candidates (5):**

- Beat 1 (Cold open): hook "Is there a tiny person typing inside ChatGPT?"
- Beat 5 (How it works: step 1): hook "ChatGPT doesn't read words. It reads tiles."
- Beat 6 (How it works: step 2): hook "King minus man plus woman equals... queen?"
- Beat 8 (Myth busted): hook "ChatGPT is not Googling your question."
- Beat 17 (Byte's Takeaway): hook "ChatGPT isn't a brain. It's the world's best guesser."

**Overlay beats:**

- Beat 5 (How it works: step 1): Word-tile split of a sample sentence + stat card: 1 token ≈ ¾ of an English word (rough estimate). SOURCE: OpenAI Help Center
- Beat 6 (How it works: step 2): 2D word map: king, man, woman, queen as dots; arrows showing king − man + woman lands near queen. SOURCE: Mikolov et al. 2013
- Beat 9 (Real-world example): Counter animates 0 → 175,000,000,000 with label 'GPT-3 (2020) adjustable settings'; dated chip '2020'. SOURCE: Brown et al. 2020
- Beat 10 (Why it matters to you): Two bars: 1.3B 'coached' model vs 175B 'uncoached' GPT-3, caption 'people preferred the smaller coached model'. SOURCE: Ouyang et al. 2022
- Beat 13 (Free tool to try): Recreated mock-up of the OpenAI Tokenizer (not a screenshot): model tab label shown exactly as on the page, 'GPT-5.x & O1/3'; input 'Why does ChatGPT make things up?'; colour-highlighted tiles Why| does| Chat|GPT| make| things| up|? (leading spaces belong to the tiles); counters Tokens 8 / Characters 32. SOURCE: OpenAI Tokenizer, platform.openai.com/tokenizer

**Dramatizations:** beat 1, beat 14, beat 18 (Bit scenes are invented illustrations; label on screen).

## Beat 1 (0:00) — Cold open  [SHORT · DRAMATIZATION]
- Card: `Is someone in there?`
- Visual: bit_scene_mockup
- Sources: —
- Short hook: "Is there a tiny person typing inside ChatGPT?"

Bit typed one line: write me a poem about burnt toast. Two seconds later, there it was. Rhymes, jokes, even a sad little ending for the toast. Bit leaned close to the screen and whispered, okay, who's in there? Is there a tiny writer living in the computer? Is it searching the internet? Reading my mind? Nope. What's really going on is stranger, simpler, and honestly kind of beautiful. Let's open it up.

## Beat 2 (0:30) — Episode card
- Card: `Inside the AI brain`
- Visual: title_card
- Sources: —

Hey, I'm Byte, and this is LostByte Explained, episode two: how does ChatGPT actually work, with no jargon. By the end, you'll know four things. How it chops up your words. How it knows which words belong together. How it learned all that in the first place. And why it can sound so helpful. Whenever a techy word sneaks in, I'll swap it for something from everyday life. Deal? Deal.

## Beat 3 (1:00) — Plain-English definition
- Card: `A very good guesser`
- Visual: byte_bit_dialogue
- Sources: S5

So Bit asks, what is it, really? Here's the one sentence version. ChatGPT is a program that looks at the words so far and guesses what word should come next, over and over, very fast. Experts call that prediction, but think of a weather forecast. A forecaster doesn't know tomorrow for sure. They look at patterns and say, probably rain. ChatGPT does the same thing with words: probably this word, then probably that one.

## Beat 4 (1:30) — Analogy
- Card: `An improv actor`
- Visual: scene_improv_stage
- Sources: S5

Picture an improv actor. Someone in the audience shouts a first line, and the actor keeps the scene going, one sentence at a time, without a script. They're not reading from a hidden page. They're drawing on every play, conversation and story they've ever soaked up. ChatGPT is like an actor who has soaked up an enormous library of text, and your message is the first line it's handed. Everything after is improvised.

## Beat 5 (2:00) — How it works: step 1  [SHORT · OVERLAY]
- Card: `Words become tiles`
- Visual: diagram_tokens
- Sources: S1, S2
- Short hook: "ChatGPT doesn't read words. It reads tiles."
- Overlay: Word-tile split of a sample sentence + stat card: 1 token ≈ ¾ of an English word (rough estimate). SOURCE: OpenAI Help Center

Step one: chopping. Before ChatGPT reads anything, it breaks your text into small pieces, like letter tiles in a word game. Experts call each piece a token. A common short word is usually one tile. A long or unusual word might be split into two or three. OpenAI's rough rule for English: one tile is about three quarters of a word. So a hundred tiles is roughly seventy-five words. It reads, and writes, in tiles.

## Beat 6 (2:30) — How it works: step 2  [SHORT · OVERLAY]
- Card: `A map of meaning`
- Visual: diagram_word_map
- Sources: S3
- Short hook: "King minus man plus woman equals... queen?"
- Overlay: 2D word map: king, man, woman, queen as dots; arrows showing king − man + woman lands near queen. SOURCE: Mikolov et al. 2013

Step two: a map. Each tile gets a spot on a giant invisible map, where words with similar meanings live close together. Dog sits near puppy. Paris sits near London. And the directions mean something too. Back in 2013, researchers showed a famous trick: start at king, step away from man, step toward woman, and you land closest to queen. Nobody drew that map by hand. It formed from reading lots of text.

## Beat 7 (3:00) — How it works: step 3
- Card: `The highlighter trick`
- Visual: diagram_attention
- Sources: S4

Step three, the aha. Take the word bank. Is it a river bank or a money bank? You'd check the rest of the sentence. ChatGPT does too. Picture it running a highlighter over everything you wrote, marking which earlier words matter most for the next guess. Fishing? River. Loan? Money. Researchers call this attention, and it's the key idea in the design behind ChatGPT, first published by Google researchers in 2017.

## Beat 8 (3:30) — Myth busted  [SHORT]
- Card: `Not a search engine`
- Visual: myth_vs_fact
- Sources: S5, S4, S12
- Short hook: "ChatGPT is not Googling your question."

Myth: ChatGPT looks up your answer somewhere, like a search engine or a giant file of saved replies. Usually, not quite. On its own, it writes each reply fresh, tile by tile, from patterns it absorbed while learning. ChatGPT can also search the web, and then it often shows you links to its sources. But the core engine isn't a filing cabinet. It's that improv actor again, building a brand new answer every single time.

## Beat 9 (4:00) — Real-world example  [OVERLAY]
- Card: `175 billion tiny knobs`
- Visual: counter_stat
- Sources: S5, S6
- Overlay: Counter animates 0 → 175,000,000,000 with label 'GPT-3 (2020) adjustable settings'; dated chip '2020'. SOURCE: Brown et al. 2020

So how did it learn? Training is basically a fill-in-the-blank game played billions of times. Hide the next word, let it guess, then nudge its settings toward the right answer. Picture a mixing desk covered in tiny knobs. GPT-3, an earlier model from 2020, had one hundred seventy-five billion of them. Researchers also found that bigger models, more text and more computing tend to improve results in a surprisingly steady, predictable way.

## Beat 10 (4:30) — Why it matters to you  [OVERLAY]
- Card: `From parrot to helper`
- Visual: diagram_training_coach
- Sources: S8, S9
- Overlay: Two bars: 1.3B 'coached' model vs 175B 'uncoached' GPT-3, caption 'people preferred the smaller coached model'. SOURCE: Ouyang et al. 2022

Here's the bit that matters for you. A model that only plays fill-in-the-blank is good at continuing text, not at helping. So people coached it. Human testers compared answers and picked the better ones, and the model was tuned toward those picks. In one OpenAI study, people preferred a coached model a hundred times smaller than GPT-3 over GPT-3 itself. That coaching is why it answers your question instead of rambling.

## Beat 11 (5:00) — Honest caveats
- Card: `Fluent isn't always right`
- Visual: byte_honest_face
- Sources: S7, S10

Now the honest caveats. Because it's always guessing likely words, it adds a little controlled randomness, like rolling a weighted die. Researchers found that always picking the single most likely word makes text bland and repetitive. That's why asking twice can give two different answers. It also learned from text up to a certain date, so it can be out of date. And, as we covered last episode, sounding sure isn't proof.

## Beat 12 (5:30) — How to use it: step 1
- Card: `Give it the context`
- Visual: checklist
- Sources: S4, S5

So, practical tip one. Remember the highlighter? It can only highlight what's in front of it. ChatGPT doesn't know your situation, your boss, or your budget unless you put them in the conversation. So give it context. Say who it's for, what you already tried, and what a good answer looks like. Paste in the email or recipe you're working on. More useful words in front of it means better guesses.

## Beat 13 (6:00) — Free tool to try  [OVERLAY]
- Card: `See your tiles`
- Visual: terminal_prompt
- Sources: S13, S1
- Overlay: Recreated mock-up of the OpenAI Tokenizer (not a screenshot): model tab label shown exactly as on the page, 'GPT-5.x & O1/3'; input 'Why does ChatGPT make things up?'; colour-highlighted tiles Why| does| Chat|GPT| make| things| up|? (leading spaces belong to the tiles); counters Tokens 8 / Characters 32. SOURCE: OpenAI Tokenizer, platform.openai.com/tokenizer

Free tool time. OpenAI has a free Tokenizer page on its website, with no login needed. Type a sentence and it colours in every tile. I typed last episode's question: why does ChatGPT make things up? Thirty-two characters became eight tiles. ChatGPT itself split into two, Chat and GPT, and each space rides along at the front of the next word. Try your own sentence, then a made up word, and watch.

## Beat 14 (6:30) — Mini demo (mock-up)  [DRAMATIZATION]
- Card: `> same question, twice`
- Visual: labeled_mockup_chat
- Sources: S7, S4

Quick demo. This is a dramatized mock-up, not a real screenshot. Bit asks, name my new cat. Answer one: Captain Whiskers. Bit asks again in a new chat: Professor Paws. Same question, different answer. That's the dice roll at work. Now Bit adds context: she's grey, grumpy, and loves sitting on keyboards. Suddenly the suggestions fit, like Sir Typo. Same model. More context, and the highlighter has something to work with.

## Beat 15 (7:00) — What's coming next
- Card: `Better coaching, more tools`
- Visual: diagram_retrieval
- Sources: S6, S8, S11, S12

What's next? The basic recipe, chop into tiles, place them on a map, highlight what matters, guess the next one, has stayed remarkably stable. What keeps changing is everything around it. More practice and more knobs, which researchers found improves results in predictable ways. Better coaching from human feedback. And more tools plugged in, like search or calculators, so the guesser can check things instead of only remembering them.

## Beat 16 (7:30) — Recap
- Card: `Tiles. Map. Highlighter.`
- Visual: recap_three_points
- Sources: S1, S3, S4

Let's recap in three points. One: tiles. ChatGPT chops your words into small pieces and writes back one piece at a time. Two: the map and the highlighter. Every piece has a place on a map of meaning, and the highlighter picks out which of your words matter for the next guess. Three: practice and coaching. Billions of fill-in-the-blank rounds, then human feedback, turned a text continuer into a helper.

## Beat 17 (8:00) — Byte's Takeaway  [SHORT]
- Card: `An expert guesser`
- Visual: takeaway_card
- Sources: S5, S9
- Short hook: "ChatGPT isn't a brain. It's the world's best guesser."

Byte's Takeaway. Is there a brain inside ChatGPT? Not like yours. There's no tiny person, no secret library of answers. There's an extraordinarily well practised guesser, coached by people to be helpful. My verdict: treat it like a brilliant improv partner. Give it a strong first line and plenty of context, and it can do amazing work. Just remember it's guessing, so you stay the one who decides what's true.

## Beat 18 (8:30) — Bookend  [DRAMATIZATION]
- Card: `Bit opens the box`
- Visual: bit_scene_resolved
- Sources: —

Back to Bit and the burnt toast poem. Bit isn't whispering at the screen anymore. Bit knows there's no tiny writer, just tiles, a map, a highlighter and a lot of practice. So this time Bit gives it a better first line: a poem for my grandma, who burns toast on purpose because she likes it crunchy. Much better poem. Your turn: what should we open up next? Comment below, and subscribe.
