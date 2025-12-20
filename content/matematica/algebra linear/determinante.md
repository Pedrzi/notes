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
  - determinantes
  - Determinantes
draft: false
date: 2025-12-18
tags:
  - matemática
parent:
---

## Definição

É uma função matricial que associa uma [[matematica/algebra linear/matrizes/index|matriz]] à um [[escalar]]. Esta função permite saber se a matriz tem ou não inversa, pois toda [[matriz inversa|matriz singular]] tem determinante igual à 0. Além disso, a determinante também expressa o volume n-dimensional dado pela forma geométrica formada pelos [[matematica/algebra linear/vetores/index|vetores]] da matriz.

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

onde $M_{ij}$ é a [[submatriz]] obtida removendo a linha $i$ e a coluna $j$ de $A$.

$(-1)^{i+j} \det(M_{ij})$ é chamado de **cofator** $(C_{ij})$.

## Propriedades

Sejam $A$ e $B$ [[matriz quadrada|matrizes quadradas]] de ordem $n$.

1. Determinante da [[Matriz Identidade]]
    O determinante da [[matriz identidade]] é sempre igual a 1.
    
2. **Determinante da [[transposicao|Transposta]]**
$$
\det(A^T) = \det(A)
$$

3. **Determinante da Inversa**

$$
\det(A^{-1}) = \frac{1}{\det(A)}
$$

4. **Multiplicatividade**

$$
\det(A) \times \det(B) = \det(AB)
$$

5. **Multiplicação por [[Escalar]]**

$$
\det(\lambda A) = \lambda ^n \det(A)
$$

6. Determinante da [[Matriz Ortogonal]]
    O determinante de uma [[matriz ortogonal]] é sempre $\pm 1$.
    
7. Determinante de uma [[Matriz Triangular]]
    O determinante de uma [[matriz triangular]] é sempre o produto dos elementos da diagonal principal.
    
8. Linha ou Coluna Multiplicada por [[Escalar]]
    Se uma das linhas ou colunas da matriz $A$ é multiplicada por um escalar $\lambda$, o determinante será igual a $\lambda \det(A)$.
    
9. Linha ou Coluna de Zeros
    Se uma linha ou coluna for composta por apenas zeros, então $\det(A) = 0$.
    
10. Permutação de Linhas ou Colunas
    Se duas linhas ou colunas de uma matriz $A$ são permutadas, o determinante da nova matriz é $-\det(A)$.
	
11. [[teorema de jacobi]] 
