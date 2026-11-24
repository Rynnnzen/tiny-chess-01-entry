# tiny-chess-01 entry

A deterministic alpha-beta chess engine in under 4 KiB of Python.

`main.py` plays through the make.fun env. It parses the FEN, generates
legal moves (castling, en passant, promotions, check detection), and
searches with alpha-beta, quiescence, piece-square tables, MVV-LVA move
ordering, killers and a transposition table, to a fixed 100,000-node
budget per move. No clock, no randomness, standard library only.

MIT, see LICENSE.
