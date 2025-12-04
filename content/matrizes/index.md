---
title: Matrizes
description:
aliases:
  - matriz
  - matrizes
  - Matriz
  - Matrizes
date: 2025-12-04
tags:
  - matemática
---

## 1. Definição
---

Uma **matriz** é um arranjo retangular de números (reais ou complexos), organizados em linhas e colunas. O conjunto de todas as matrizes com $m$ linhas e $n$ colunas com entradas reais é denotado por $M_{m \times n}(\mathbb{R})$.

A **ordem** (ou dimensão) de uma matriz é descrita pelo formato $m \times n$.

- $m$: número de linhas.
- $n$: número de colunas.

Por exemplo, a matriz $A$ abaixo é de ordem $3 \times 3$ (três linhas e três colunas):

$$
A =
\begin{bmatrix}
1 & 2 & 3 \\ 
4 & 5 & 6  \\
7 & 8 & 9
\end{bmatrix}
$$

## 2. Notação Indexada
---

Cada elemento individual de uma matriz é identificado pela sua posição única, denotada por $a_{ij}$, onde:

- $i$ representa o índice da **linha** ($1 \leq i \leq m$).
- $j$ representa o índice da **coluna** ($1 \leq j \leq n$).

Genericamente, uma matriz $A$ de ordem $m \times n$ é representada como:

$$
A = (a_{ij}) =
\begin{bmatrix} 
a_{11} & a_{12} & \cdots & a_{1n} \\ 
a_{21} & a_{22} & \cdots & a_{2n} \\
\vdots & \vdots & \ddots & \vdots \\ 
a_{m1} & a_{m2} & \cdots & a_{mn}
\end{bmatrix}
$$

## Relacionado
---
```base
filters:
  and:
    - file.hasLink("matrizes/index")
views:
  - type: table
    name: Table

```
