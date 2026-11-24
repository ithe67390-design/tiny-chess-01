# Tiny Chess 01

A single-file Python engine for make.fun. It searches up to 60,000 nodes per move with iterative deepening, alpha-beta pruning, a transposition table, and quiescence search. Material, piece-square tables, bishop pairs, and endgame king and pawn terms guide evaluation.

Set `MAKEFUN_ENV_URL` to the game server and run `python -P -s main.py`. The official `makefun compress` packer embeds the engine source in the entry. Python's standard library handles unpacking, search, and communication with the server.

The entry is 3,320 bytes. On local practice trial 0 the engine scored 1,545 Elo with four wins, one draw, and one loss. Its six depth-three perft counts matched python-chess.
