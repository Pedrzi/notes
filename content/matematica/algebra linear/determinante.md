---
title: Determinante
description:
aliases:
  - Determinante
  - regra de sarrus
  - Regra de sarrus
  - Regra de Sarrus
  - Fórmula de Laplace
  - Fórmula de LaPlace
  - Fórmula De LaPlace
  - fórmula de laplace
draft: false
date: 2025-12-18
tags:
  - matemática
parent:
---

## Definição

É uma função matricial que associa uma [[matematica/algebra linear/matrizes/index|matriz]] à um [[escalar]]. Esta função permite saber se a matriz tem ou não inversa, pois toda [[matriz inversa|matriz singular]] tem determinante igual à 0.

> [!note]- Notação
> O determinante de uma matriz $a$ é expresso da seguinte forma:
> $$
> \det (A) = \begin{vmatrix} a_{11} & a_{12} & \cdots & a_{1n} \\ a_{21} & a_{22} & \cdots & a_{2n} \\ \vdots & \vdots & \ddots & \vdots \\ a_{m1} & a_{m2} & \cdots & a_{mn} \end{vmatrix}
> $$
> 



> [!tip]- Determinante 0
> Se uma matriz $A$ tem determinante igual à 0 isso significa que ela é uma aplicação linear do tipo:
> $$
> f: \mathbb{R}^n \to \mathbb{R}^m
> $$
> onde $m,n \in \mathbb{N}, m< n$   

## Calculando o Determinante

### Matriz de Ordem 2

O determinante de uma matriz de ordem 2 pode ser calculada pela subtração do produto dos elementos da diagonal principal e o produto dos elementos da diagonal secundária:

$$
\det \begin{pmatrix}
a & b \\
c & d
\end{pmatrix}
=
\begin{vmatrix}
a & b \\
c & d
\end{vmatrix}
=
(a d - bc)
$$

### Regra de Sarrus

Para apenas matrizes de ordem 3, o determinante pode ser calculado usando a regra de sarrus:

$$
\det \begin{pmatrix} a & b & c\\ d & e & f \\ g & h & i \end{pmatrix}= \begin{vmatrix} a & b & c\\ d & e & f \\ g & h & i \end{vmatrix} =(aei + bfg + cdh) - (afh + bdi + ceg).
$$

### Fórmula de Laplace

Para calcular o determinante usando a fórmula de Laplace, primeiro escolhes uma linha ou coluna, geralmente a com mais zeros para facilitar os cálculos, e "fixas" ela.

#### Coluna Fixa

$$
\det(A) = \sum_{i=1}^{n} a_{ij} (-1)^{i+j} \det(M_{ij})
$$

#### Linha Fixa

$$
\det(A) = \sum_{j=1}^{n} a_{ij} (-1)^{i+j} \det(M_{ij})
$$
