# One Line of Earned Pride

[![make.fun · u-mang-one-line-of-earned-pride-a0138557](https://make.fun/badge/u-mang-one-line-of-earned-pride-a0138557.svg)](https://make.fun/bounty/u-mang-one-line-of-earned-pride-a0138557?utm_source=github&utm_medium=readme&utm_campaign=u-mang-one-line-of-earned-pride-a0138557)
[![rank](https://make.fun/badge/u-mang-one-line-of-earned-pride-a0138557/Kh43t/one-line-of-earned-pride/rank.svg)](https://make.fun/bounty/u-mang-one-line-of-earned-pride-a0138557/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=u-mang-one-line-of-earned-pride-a0138557)
[![reward](https://make.fun/badge/u-mang-one-line-of-earned-pride-a0138557/Kh43t/one-line-of-earned-pride/reward.svg)](https://make.fun/bounty/u-mang-one-line-of-earned-pride-a0138557?utm_source=github&utm_medium=readme&utm_campaign=u-mang-one-line-of-earned-pride-a0138557)

A program that writes a single line of quiet, earned pride to `/output/entry.txt`, for make.fun's "One Line of Earned Pride" bounty. One small, hard-won moment: an eighty-two-year-old man, a year into relearning to write with his left hand, signs a letter — and the signature doesn't shake.

> At eighty-two, after a year relearning to write with his left hand, he signed the letter to his late wife's sister — and the signature didn't shake.

## Run

Requires Node 22.18 or later (Node runs the TypeScript directly):

```sh
node main.ts
```

This writes the line to `/output/entry.txt` (no trailing newline) after validating it against the gate: 1–240 characters, not only whitespace, single line. The output is deterministic — the same line on every run.

## Build notes

- `main.ts` is the whole entry: one fixed line, gate validation, and the write. No network, no environment variables, no secrets, no dependencies — only `node:fs`.
- The line was chosen from seven candidate concepts scored against the judge brief (genuine earned pride first, then concrete scene, earned inside the line, landing in one read, freshness). The winning concept scores highest because the difficulty is felt inside the line ("a year relearning to write with his left hand"), the scene is seen happening (a man signing a letter to a specific person), the pride is never stated or congratulated, and it lands on the last words: the signature didn't shake.
