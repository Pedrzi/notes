---
title: matriz identidade
description:
aliases: [Matriz Identidade, Matriz identidade, delta de kronecker, Delta de kronecker]
draft: false
date: 2025-12-04
tags: [math]
parent:
  - "[[matematica/algebra linear/matrizes/index|index]]"
criado: 2026-02-05T13:46:46Z
modificado: 2026-02-06T11:58:19Z
---

## Definição

A **Matriz Identidade** de ordem $n$, denotada por $I_n$ (ou simplesmente $I$), é uma [[matriz triangular|matriz escalar]] onde todos os elementos da diagonal principal são iguais a 1 e os restantes são 0.

É o elemento neutro da [[multiplicacao de matrizes|multiplicação de matrizes]] em $\mathcal{M}_{n}(\mathbb{K})$.

### Notação (Delta de Kronecker)

Os elementos de $I_n$ são definidos rigorosamente pelo **Delta de Kronecker** ($\delta_{ij}$):

$$
(I_n)_{ij} = \delta_{ij} =
\begin{cases}
1, & \text{se } i=j \\
0, & \text{se } i \neq j 
\end{cases}
$$

## Exemplo ($I_3$)

$$
I_3 = \begin{bmatrix} 1 & 0 & 0 \\ 0 & 1 & 0 \\ 0 & 0 & 1 \end{bmatrix}
$$

## Propriedades

### Elemento Neutro da Multiplicação

Para qualquer matriz $A$ de dimensão compatível ($m \times n$):

- $A \cdot I_n = A$ (Multiplicação à direita)
- $I_m \cdot A = A$ (Multiplicação à esquerda)

No caso de matrizes quadradas de mesma ordem ($A \in \mathcal{M}_{n}$):

$$
A I = I A = A
$$

### Inversibilidade

A matriz identidade é a sua própria inversa:

$$
I^{-1} = I
$$
