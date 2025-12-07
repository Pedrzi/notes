---
title: Matriz Simétrica
description:
aliases:
draft: false
date: 2025-12-04
tags:
  - matemática
parent:
  - "[[matematica/algebra linear/matrizes/index|index]]"
---

## Matriz Simétrica

Uma matriz quadrada $A \in \mathcal{M}_{n}(\mathbb{K})$ diz-se **simétrica** se for igual à sua [[transposicao|transposta]]:

$$
A^T = A
$$

Em termos de elementos, isso significa que $a_{ij} = a_{ji}$ para todos os índices $i, j$. A matriz funciona como um "espelho" em relação à diagonal principal.

### Exemplo

$$
A = \begin{bmatrix} 1 & \mathbf{2} & \mathbf{3} \\ \mathbf{2} & 4 & \mathbf{5} \\ \mathbf{3} & \mathbf{5} & 6 \end{bmatrix}
$$

## Matriz Antissimétrica

Uma matriz quadrada $A \in \mathcal{M}_{n}(\mathbb{K})$ diz-se **antissimétrica** se for igual ao simétrico da sua [[transposicao|transposta]]:

$$
A^T = -A
$$

Em termos de elementos, $a_{ij} = -a_{ji}$.

> [!info] Propriedade da Diagonal
>  Para que $a_{ii} = -a_{ii}$ seja verdade, todos os elementos da **diagonal principal** de uma matriz antissimétrica devem ser **nulos** (zero).

### Exemplo

$$
B = \begin{bmatrix} 0 & \mathbf{2} & \mathbf{-1} \\ \mathbf{-2} & 0 & \mathbf{4} \\ \mathbf{1} & \mathbf{-4} & 0 \end{bmatrix}
$$

## Propriedades e Teoremas

Seja $A$ uma matriz quadrada qualquer de ordem $n$:

### Construção de Simetria

A partir de qualquer matriz quadrada $A$, podemos construir matrizes com simetria definida:

1. $A + A^T$ é sempre uma **matriz simétrica**.
2. $A - A^T$ é sempre uma **matriz antissimétrica**.
3. $AA^T$ ou $A^TA$ é sempre uma **matriz simétrica**

### Decomposição

Toda a matriz quadrada $A$ pode ser decomposta de forma única na soma de uma matriz simétrica ($S$) e uma matriz antissimétrica ($K$):

$$
A = 
\underbrace{\frac{1}{2} (A + A^T)} _{\text{Simétrica}} + 
\underbrace{\frac{1}{2} (A - A^T)} _{\text{Antissimétrica}}
$$

## Matriz Simétrica Definida Positiva

todo
