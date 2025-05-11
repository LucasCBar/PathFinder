# PathFinder - Labirinto 2D com Algoritmo A*

Este projeto implementa o algoritmo A* para encontrar o menor caminho entre dois pontos em um labirinto 2D, evitando obstáculos e considerando o custo dos movimentos.

## 🔍 Problema

Dado um labirinto representado por uma matriz 2D, o objetivo é ajudar um robô de resgate a sair do ponto inicial `S` e alcançar o ponto final `E` com o menor custo, evitando as células com obstáculos (`1`).

### Exemplo de entrada:

S 0 1 0 0  
0 0 1 0 1  
1 0 1 0 0  
1 0 0 E 1  

### Saída esperada:

[(0, 0), (1, 0), (1, 1), (2, 1), (3, 1), (3, 2), (3, 3)]

## 💡 Algoritmo Utilizado

### Algoritmo A*

O A* é uma técnica de busca heurística que combina:

- `g(n)`: custo do caminho percorrido até o nó `n`
- `h(n)`: estimativa de custo restante até o destino (heurística)
- `f(n) = g(n) + h(n)`: estimativa total do custo do caminho

#### Heurística utilizada: Distância de Manhattan

h(n) = |x_atual - x_final| + |y_atual - y_final|

## 🛠️ Como executar o projeto

1. Clone o repositório:
   git clone https://github.com/seuusuario/pathfinder-a-star.git
   cd pathfinder-a-star

2. Execute o código:
   python main.py

3. Para rodar os testes:
   python -m unittest tests/test_pathfinder.py
