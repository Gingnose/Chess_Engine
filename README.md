This is an soritary chess enginne creation endeavour that aims to reach the strength higher than me 
(about 1750 elo on chess.com). First prototype will be hard-coded and all the evaluation function etc will be
arbitarily examined by testing each generation. After this project I'm also aiming to build chess AI that runs
by NN ideally by RL (However, for the computational limitation, I don't know how much strong it can get)

For piece evaluation:
I adopted a Fischer evaluation score for now
![スクリーンショット 2024-03-07 15 16 23](https://github.com/Gingnose/Chess_Engine/assets/136443889/a25cd029-5a55-499e-88c9-2380209f91eb)

Currently the strongest chess engine is stockfish 16 which estimated to be around 3800? elo.
stockfish 16 runs on NNUE architecture.

![image](https://github.com/Gingnose/Chess_Engine/assets/136443889/d480e0ff-ff65-4660-9c8c-39a1c8e13148)


I would like to eventually rewrite the codes in C++ for exploration efficiency.

Stockfish 16 is opensource:
GitHub: https://github.com/official-stockfish/Stockfish
