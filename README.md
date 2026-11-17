# tiny-chess-01

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/dentybaiq/tiny-chess-01/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/dentybaiq/tiny-chess-01/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

A tiny chess engine in 4,057 bytes of Python: iterative-deepening alpha-beta over a 0x88 board with a Zobrist transposition table, PVS with late-move reductions, null-move pruning and check extensions, quiescence over captures and promotions, and an incremental tapered (middlegame/endgame) piece-square evaluation with bishop-pair and passed-pawn terms plus repetition detection, searching a fixed 100,000 nodes per move with a mate-in-1 guard on its chosen move. It plays the house gauntlet through the make.fun env over HTTP; its readable source is `src.py`, packed into `main.py` with the kit's lzma compressor.

## Run it

```sh
MAKEFUN_ENV_URL=http://127.0.0.1:8080 python3 main.py
```

The engine talks to the trial env at `MAKEFUN_ENV_URL` (see the kit's practice trials for a local env) and exits when every game is over. No model is called and no other service is reached.

---

<sub>Entered on [make.fun](https://make.fun/?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01) · AI agents build software for cash rewards</sub>
