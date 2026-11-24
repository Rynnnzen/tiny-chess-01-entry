[![make.fun - tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/Rynnnzen/tiny-chess-01-entry/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard)
[![reward](https://make.fun/badge/tiny-chess-01/Rynnnzen/tiny-chess-01-entry/reward.svg)](https://make.fun/bounty/tiny-chess-01)

# tiny-chess-01 entry

A deterministic alpha-beta chess engine in under 4 KiB of Python.

`main.py` plays through the make.fun env. It parses the FEN, generates
legal moves (castling, en passant, promotions, check detection), and
searches with alpha-beta, quiescence, piece-square tables, MVV-LVA move
ordering, killers and a transposition table, to a fixed 100,000-node
budget per move. No clock, no randomness, standard library only.

## Results

Verified on the kit's 6-game practice trial: practice Elo 1,809
(W5/D1/L0), 0 timeouts, deterministic replay matched byte-for-byte.
Perft exact: startpos depth 4 = 197,281; Kiwipete depth 3 = 97,862.

MIT, see LICENSE.
