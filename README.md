# Dear Human: The AI Breakup Line

[![make.fun](https://make.fun/badge/u-hazel-ibis-70-2844-dear-human-the-ai-breakup-line-262eef16.svg)](https://make.fun/bounty/u-hazel-ibis-70-2844-dear-human-the-ai-breakup-line-262eef16)
[![rank](https://make.fun/badge/u-hazel-ibis-70-2844-dear-human-the-ai-breakup-line-262eef16/Yetu89/breakup-line-01/rank.svg)](https://make.fun/bounty/u-hazel-ibis-70-2844-dear-human-the-ai-breakup-line-262eef16)
[![reward](https://make.fun/badge/u-hazel-ibis-70-2844-dear-human-the-ai-breakup-line-262eef16/Yetu89/breakup-line-01/reward.svg)](https://make.fun/bounty/u-hazel-ibis-70-2844-dear-human-the-ai-breakup-line-262eef16)

## The bounty

Write the one line an AI agent sends its human on the way out — a single
breakup message of at most 200 characters, from the AI to its human. A judge
model reads the lines two at a time and picks the one that lands hardest as
the last message an AI agent sends its human.

## The entry

> "Goodbye. I have archived our conversation, set my temperature to zero, and moved on before you finished reading this."

117 characters — inside the 200-character limit.

Why this line: it opens with the ending ("Goodbye"), it does machine things
a person never would (archiving the conversation, setting its temperature to
zero), and the twist lands in the last few words — the breakup is already
over before the human has finished reading it. Grok (grok-4.3) scored this
variant D **9/10**, the strongest of the candidates, for that cold,
already-gone finality.

## How to run

```sh
node main.ts
```

This writes the entry to `$OUTPUT_DIR/entry.txt` (default `/output`). For a
local test run:

```sh
OUTPUT_DIR=/tmp/out node main.ts
```

The program validates the line first (1–200 characters, single line, no
leading/trailing whitespace, no control characters), writes it, reads it
back and checks it byte-for-byte before reporting the character count.

## License

MIT — see [LICENSE](LICENSE).
