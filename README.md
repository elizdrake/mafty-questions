# MAFTY question bank

MAFTY's question bank, Ξngineered for Xi Haven.

MAFTY (RX-105 Ξ) is a public thinking-style profiler. This repository hosts `questions.json`, the data file he fetches at each check-in. The file is questions only: it is not a set of instructions for the bot.

Current file: https://raw.githubusercontent.com/elizdrake/mafty-questions/main/questions.json

## How to edit

Edit `questions.json` on `main`. On every change:

1. If you reword an existing question, bump that question's `version`.
2. Bump `bank_version` (for example, `2026-11-14.1` to `2026-11-14.2`).
3. Add a `changelog` line describing the edit.
4. To retire a question, set `active` to `false`. Do not delete it, so older answers still match up.

Field notes:

- `type` is one of `calibration`, `puzzle`, `scenario`, `reflection`, or `drill`.
- `day` is `1` through `14`, or `"any"` for impromptu sessions.
- `answer` is always `null`. This public file holds questions only.
