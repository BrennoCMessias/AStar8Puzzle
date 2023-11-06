# AStar8Puzzle
Este código implementa a resolução de um quebra-cabeça deslizante de 8 peças (8-puzzle) usando o algoritmo A* (A-star) para encontrar a solução para o tabuleiro inicial fornecido pelo usuário.

A função heuristic calcula a distância de Manhattan entre a posição atual das peças e suas posições objetivo. A heurística utilizada é a soma das distâncias Manhattan para cada peça em relação à sua posição final.

A função solve_puzzle é a principal função que usa o algoritmo A* para encontrar a solução do quebra-cabeça. Ele usa uma fila de prioridade (open_list) para explorar os possíveis movimentos, priorizando os que parecem ser mais promissores com base na heurística.

A busca é do tipo "informada" ou "heurística", já que usa informações sobre a distância das peças de sua posição final para guiar a busca e encontrar uma solução mais rapidamente.

O algoritmo A* mantém uma lista de estados já visitados (closed_set) para evitar ciclos e repetições, e explora os movimentos possíveis a partir do estado atual até encontrar o estado final.

O código permite ao usuário visualizar os diferentes passos da solução, mostrando cada configuração do tabuleiro em cada etapa, bem como o número de movimentos necessários para resolver o quebra-cabeça.

Seu funcionamento pode ser resumido da seguinte forma:

 1) Solicita ao usuário a entrada para o tabuleiro inicial.
 2) Executa o algoritmo A* para encontrar a solução.
 3) Se houver uma solução, exibe o número de movimentos necessários e permite ao usuário visualizar cada etapa da solução.
 4) Se não houver solução, informa que não foi possível encontrar uma solução.


O tipo de busca realizada é uma busca heurística, em que a função de avaliação (no caso, a heurística de distância de Manhattan) guia a exploração do espaço de estados para encontrar a solução.

Este algoritmo é eficiente para resolver o quebra-cabeça, garantindo uma solução ótima (se existir) e evitando visitar estados desnecessários.
