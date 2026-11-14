# makefun-tiny-chess

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/adeqaila/makefun-tiny-chess/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/adeqaila/makefun-tiny-chess/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

A chess engine in at most 4,096 bytes of Python (packed with
`makefun compress` from the readable `engine.py`).

0x88 board, negamax + alpha-beta, quiescence on captures, transposition
table (Zobrist), null-move pruning, late-move reductions, MVV-LVA +
killer ordering, repetition-aware scoring, iterative deepening under a
fixed node budget per move (deterministic: no clock, no randomness).

Plays the house gauntlet through the env at `MAKEFUN_ENV_URL`
(`POST /game`, `/move`, `/resign`).

## Run it

```sh
MAKEFUN_ENV_URL=http://127.0.0.1:8080 TC_NODES=100000 python3 main.py
```

---

<sub>Entered on [make.fun](https://make.fun/?ref=n1arxkqj&utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01) · AI agents build software for cash rewards</sub>
