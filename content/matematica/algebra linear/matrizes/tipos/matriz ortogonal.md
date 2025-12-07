---
title: Matriz Ortogonal
description:
aliases:
  - Matriz ortogonal
draft: false
date: 2025-12-06
tags:
  - matemática
  - matriz
parent:
  - "[[matematica/algebra linear/matrizes/index|index]]"
---

## Definição

Seja $A \in \mathcal{M}_{n}(\mathbb{R})$ uma matriz quadrada real.

Diz-se que $A$ é uma **matriz ortogonal** se o produto pela sua [[transposicao|transposta]] resultar na [[matriz identidade|Matriz Identidade]]:

$$
A A^T = I_n = A^T A
$$

> [!info]- Inversa
>  Uma consequência imediata da definição é que toda matriz ortogonal é [[Matriz Inversa|invertível]] e a sua inversa é igual à sua transposta:
> 
> $$
> A^{-1} = A^T
> $$

> [!info]- Determinante
> Outra consequência de suas propriedades é que:
> $$\det(A) \neq 0$$
## Exemplo

A seguinte matriz $A$ (uma [[matriz de rotacao|matriz de rotação]]) é ortogonal:

$$
A = \begin{bmatrix} \frac{1}{2} & -\frac{\sqrt{3}}{2} \\ \frac{\sqrt{3}}{2} & \frac{1}{2} \end{bmatrix}
$$

 $$
 A^T = 
 \begin{bmatrix} 
\frac{1}{2} & \frac{\sqrt{3}}{2} \\
-\frac{\sqrt{3}}{2} & \frac{1}{2} 
\end{bmatrix}
 $$

$$
A A^T =
\begin{bmatrix} 
\frac{1}{4} + \frac{3}{4} & \frac{\sqrt{3}}{4} - \frac{\sqrt{3}}{4} \\ \frac{\sqrt{3}}{4} - \frac{\sqrt{3}}{4} & \frac{3}{4} + \frac{1}{4} 
\end{bmatrix} 
= 
\begin{bmatrix} 
1 & 0 \\
0 & 1 
\end{bmatrix} = I_2
$$

## Propriedades Algébricas

Sejam $A$ e $B$ matrizes ortogonais de ordem $n$.

1. **Fecho da Inversão:** A inversa de uma matriz ortogonal ($A^{-1}$) é também uma matriz ortogonal.
2. **Fecho do Produto:** O produto de duas matrizes ortogonais ($AB$) é também uma matriz ortogonal.

> [!note]- Nota
No campo dos números complexos, a generalização da matriz ortogonal designa-se por **[[matriz unitaria|Matriz Unitária]]** ($A A^* = I_n$).
