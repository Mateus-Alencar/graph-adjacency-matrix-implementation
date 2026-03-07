# Matriz de Adjacência de Grafos

Repositório dedicado à implementação de grafos e dígrafos utilizando matriz de adjacência. Ela incluí documentação, exemplos e código da implementação

## Sumário
graph-adjacency-matrix-implementation
├── src/
│   └── grafo.py
├── examples/
│   └── exemplo_grafo.py
└── README.md

## Conceitos

Um **Grafo** é uma estruta de dados compostas por: **Vértices**(nós) e **Areas**(conexões).
```txt
G = (V, E)

```

Um **dígrafo** (grafo direcionado) possui arestas com direção.
Exemplo:
```txt
A -> B
B -> C
C -> A
```
>[!NOTE]  
> Em caso de dúvida, consulte o [seguinte repositório](https://github.com/Mateus-Alencar/EstruturaDeDados/blob/main/DOCS/grafos.md).

### Matriz de Adjacência

A matriz de adjacência é uma forma de representar grafos utilizando uma matriz quadrada.

Se um grafo possui N vértices, a matriz terá dimensão: `N x N`

Cada posição da matriz indica se existe conexão entre dois vértices.

Exemplo:
Grafo com vértices: `
```txt
A, B, C
```
Conexões:
```txt
A — B
A — C
```
Matriz de adjacência:

    A B C
A [ 0 1 1 ]
B [ 1 0 0 ]
C [ 1 0 0 ]

Onde:

1 → existe aresta

0 → não existe aresta