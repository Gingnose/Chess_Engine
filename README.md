This is an soritary chess enginne creation endeavour that aims to reach the strength higher than me 
(about 1750 elo on chess.com). First prototype will be hard-coded and all the evaluation function etc will be
arbitarily examined by testing each generation. After this project I'm also aiming to build chess AI that runs
by NN ideally by RL (However, for the computational limitation, I don't know how much strong it can get)

For piece evaluation:
I adopted a Fischer evaluation score for now
![スクリーンショット 2024-03-07 15 17 30](https://github.com/Gingnose/Chess_Engine/assets/136443889/deb37c64-3bc4-4ce0-aef1-eb5b6bd607c9)
![スクリーンショット 2024-03-07 15 16 23](https://github.com/Gingnose/Chess_Engine/assets/136443889/088c50b6-4804-4567-83e0-a32cdb5dc8d3)


Currently the strongest chess engine is stockfish 16 which estimated to be around 3800? elo.
stockfish 16 runs on NNUE architecture.

![image](https://github.com/Gingnose/Chess_Engine/assets/136443889/cbc70ab9-c7ed-42c6-bc14-109c18865934)

I would like to eventually rewrite the codes in C++ for exploration efficiency.

Stockfish 16 is opensource:
GitHub: https://github.com/official-stockfish/Stockfish
