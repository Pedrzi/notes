---
title: matriz hermitiana
description:
aliases: [Matriz Hermítica, matriz hermítica, matriz auto-adjunta, hermitiana]
draft: false
date: 2025-12-04
tags: []
parent:
  - "[[matematica/algebra linear/matrizes/index|index]]"
criado: 2026-02-05T13:46:46Z
modificado: 2026-02-06T11:58:19Z
---

## Definição

Seja $n \in \mathbb{N}$. Uma matriz $A \in \mathcal{M}_{n}(\mathbb{K})$ diz-se:

- Hermítica se $A^* = A$
- Anti-Hermítica se $A^* = -A$

## Exemplo

A matriz $A$ é uma matriz hermítica

$$
A =
\begin{bmatrix}
1 & 0 & 2+3i \\
0 & 2 & -i \\
2-3i & i & 6
\end{bmatrix}
$$
## Hermítica Definida Positiva

Seja $n$ um natural qualquer, $x$ uma matriz coluna complexa qualquer com $n$ linhas e $A$ uma matriz hermítica de ordem $n$:

A matriz $A$ diz-se **semi-definida positiva** se $x^*Ax \geq 0$ e **definida positiva** se $x^*Ax > 0$ e $x \neq 0_{n,1}$
