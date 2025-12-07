---
title: Matriz Unitária
description:
aliases:
  - Matriz Unitária
draft: false
date: 2025-12-04
tags:
  - matemática
parent:
  - "[[matematica/algebra linear/matrizes/index|index]]"
---

## Definição

Uma matriz quadrada complexa $A \in \mathcal{M}_{n}(\mathbb{C})$ diz-se **unitária** se o produto pela sua [[conjugado transposto|Matriz Transconjugada]] ($A^*$) resultar na [[matriz identidade]]:

$$
A A^* = I_n = A^* A
$$
> [!info]- Inversa
> Uma consequência imediata da definição é que toda matriz unitária é [[matriz inversa|invertível]] e sua inversa é igual á sua [[conjugado transposto|transconjugada]]:
> $$
> A^{-1} = A^*
> $$

> [!info]- Determinante
> Outra consequência de suas propriedades é que:
> $$
> \det(A) \neq 0
> $$

Esta definição implica que as linhas (e colunas) da matriz formam uma [[base ortonormal]] em relação ao [[produto interno]].

## Exemplo

A seguinte matriz $A$ é unitária:

$$
A =
\begin{bmatrix} 
 0 & i \\ 
 -i & 0  \\
\end{bmatrix}
$$
$$
A^* =
\begin{bmatrix}
0 & i \\ 
-i & 0 
\end{bmatrix}
$$

$$
A A^* = \begin{bmatrix} 0 & i \\ -i & 0 \end{bmatrix} \begin{bmatrix} 0 & i \\ -i & 0 \end{bmatrix} = \begin{bmatrix} -i^2 & 0 \\ 0 & -i^2 \end{bmatrix} = I_2
$$

## Propriedades Algébricas

Sejam $A$ e $B$ matrizes unitárias de ordem $n$.

1. **Fecho da Inversão:** A inversa de uma matriz unitária ($A^{-1}$) é também uma matriz unitária.
2. **Fecho do Produto:** O produto de duas matrizes unitárias ($AB$) é também uma matriz unitária.
