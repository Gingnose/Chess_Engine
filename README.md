This is an soritary chess enginne creation endeavour that aims to reach the strength higher than me 
(about 1800 elo on chess.com). First prototype will be hard-coded and all the evaluation function etc will be
arbitarily examined by testing each generation. After this project I'm also aiming to build chess AI that runs
by NN ideally by RL (However, for the computational limitation, I don't know how much strong it can get)

For piece evaluation:
I adopted a Fischer evaluation score for now
![スクリーンショット 2024-03-07 15 17 30](https://github.com/Gingnose/Chess_Engine/assets/136443889/deb37c64-3bc4-4ce0-aef1-eb5b6bd607c9)
![スクリーンショット 2024-03-07 15 16 23](https://github.com/Gingnose/Chess_Engine/assets/136443889/088c50b6-4804-4567-83e0-a32cdb5dc8d3)

EDIT:
Renewed version of (* more sotisiphicated version of) evaluation score & heatmap for each pieces (adopted from sunfish)
Pawn: 100, Knight: 280, Bishop: 320, Rook: 479, Queen: 929, King: 99999

piece score was upgraded to more nuanced values

Pawn heatmap:
![image](https://github.com/Gingnose/Chess_Engine/assets/136443889/00d3a26e-d096-4efd-9c63-080f298f8239)

Note that 1st and 8th rank are set to 0 since pawn doesn't either unable to exist (1st rank) or promoted (8 th rank). 

Knight heatmap:
![image](https://github.com/Gingnose/Chess_Engine/assets/136443889/49716c25-5574-48e1-b5d6-198447c37a2a)

As you can see, [1, 2] square has high score (which is a b7 square that forks the king and rook.

![image](https://github.com/Gingnose/Chess_Engine/assets/136443889/726d6fb5-bc22-486f-8e02-f2ff1a209bd6)

As you can see bishop suffers less from being passive in the first rank because it is a long range piece.


![image](https://github.com/Gingnose/Chess_Engine/assets/136443889/4ff72b62-296e-44c4-b835-1cac4b543291)

As people say, rooks love 7th rank!

![image](https://github.com/Gingnose/Chess_Engine/assets/136443889/ba1a6f6c-6e88-4beb-8881-f764c3b754f5)

Only the opponents' queen's square is dark... it is probably not a good idea to exchange queens in general

![image](https://github.com/Gingnose/Chess_Engine/assets/136443889/7a4d87c9-0467-4f80-989b-153cc7cb6f7d)

king wants to be castled and tucked in the corner. However, king's square value can change lagely on the stage of the game and need adjustments accordingly.







Currently the strongest chess engine is stockfish 16 which estimated to be around 3800? elo.
stockfish 16 runs on NNUE architecture.

![image](https://github.com/Gingnose/Chess_Engine/assets/136443889/cbc70ab9-c7ed-42c6-bc14-109c18865934)

I would like to eventually rewrite the codes in C++ for exploration efficiency.

Stockfish 16 is opensource:
GitHub: https://github.com/official-stockfish/Stockfish
