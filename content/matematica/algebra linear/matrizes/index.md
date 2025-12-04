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

## Definição

Uma **matriz** é um arranjo retangular de escalares (números reais ou complexos), organizados em linhas horizontais e colunas verticais.

Formalmente, uma matriz sobre um corpo $\mathbb{K}$ (como $\mathbb{R}$ ou $\mathbb{C}$) é uma função $A: \{1, \dots, m\} \times \{1, \dots, n\} \to \mathbb{K}$.

- O conjunto de todas as matrizes com $m$ linhas e $n$ colunas com entradas em $\mathbb{K}$ é denotado por $\mathcal{M}_{m \times n}(\mathbb{K})$.
- Se as entradas forem apenas reais, denota-se por $\mathcal{M}_{m \times n}(\mathbb{R})$.

### Ordem da Matriz

A **ordem** (ou tipo) de uma matriz é descrita pelo formato $m \times n$.

- $m$: número de linhas.
- $n$: número de colunas.

**Exemplos:**

A matriz $A$ é de ordem $3 \times 3$ ([[matriz quadrada|quadrada]]):

$$
A = \begin{bmatrix} 1 & 2 & 3 \\ 4 & 5 & 6 \\ 7 & 8 & 9 \end{bmatrix}
$$

A matriz $B$ é de ordem $2 \times 4$ (retangular):

$$
B = \begin{bmatrix} 1 & 0 & -2 & 5 \\ 3 & 4 & 0 & 1 \end{bmatrix}
$$

## Notação Indexada

Cada elemento individual de uma matriz é identificado pela sua posição única, denotada por $a_{ij}$ (ou $A_{i,j}$), onde:

- $i$ representa o índice da **linha** ($1 \leq i \leq m$).
- $j$ representa o índice da **coluna** ($1 \leq j \leq n$). 

Genericamente, uma matriz $A$ de ordem $m \times n$ é representada como:

$$
A = [a_{ij}] = \begin{bmatrix} a_{11} & a_{12} & \cdots & a_{1n} \\ a_{21} & a_{22} & \cdots & a_{2n} \\ \vdots & \vdots & \ddots & \vdots \\ a_{m1} & a_{m2} & \cdots & a_{mn} \end{bmatrix}
$$

## Classificações Básicas

Com base nas dimensões $m$ e $n$, definimos:

- **Matriz Linha:** Uma matriz de ordem $1 \times n$ (apenas uma linha).
    - Exemplo: $v = \begin{bmatrix} 1 & 2 & 3 \end{bmatrix}$.
- **Matriz Coluna:** Uma matriz de ordem $m \times 1$ (apenas uma coluna).
    - Exemplo: $u = \begin{bmatrix} 1 \\ 2 \\ 3 \end{bmatrix}$.
- **Matriz Nula (**$0_{m \times n}$**):** Uma matriz onde todos os elementos são iguais a zero ($a_{ij} = 0, \forall i,j$).

## Igualdade de Matrizes

Duas matrizes $A$ e $B$ são consideradas **iguais** ($A=B$) se, e somente se:

1. Possuem a mesma ordem ($m \times n$).
2. Todos os elementos correspondentes são iguais ($a_{ij} = b_{ij}$ para todo $i, j$).
