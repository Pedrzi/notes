---
title: Transconjugada
description:
aliases:
  - transconjugada
  - transposto hermitiano
  - Matriz Transconjugada
  - matriz transconjugada
  - Matriz transconjugada
  - Transconjugada
draft: false
date: 2025-12-07
tags:
  - matemática
  - matriz
parent:
---

## Definição

O conjugado transposto de uma [[matematica/algebra linear/matrizes/index|matriz]] $m \times n$ complexa $A$, é uma matriz $n \times m$ obtida pela transposta de $A$ e tomando o [[conjugado complexo]] de cada elemento da matriz.

> [!note]- Notação
> É tipicamente denotado por $A^H$, ou $A^*$, ou $A^{'}$, ou então $A^{\dagger}$

Formalmente:

$$
A^* = (\overline{A})^T = \overline{(A^T)}
$$

Em termos dos elementos individuais, o elemento na posição $(i,j)$ de $A^*$ é o conjugado complexo do elemento na posição $(j,i)$ de $A$:

$$
(A^*)_{ij} = \overline{A_{ji}}
$$

> [!info]- Caso Real
>  Se a matriz $A$ for real ($\mathbb{K}=\mathbb{R}$), a conjugação não altera os elementos ($\overline{x} = x$), logo a transconjugada reduz-se à transposta: $A^* = A^T$.

## Exemplo

Considere a matriz $A$:

$$
A = \begin{bmatrix} 
1-i & 0 & 3 \\
2+3i & 4 & i  \\ 
0 & 0 & 6-4i
\end{bmatrix}
$$

1. **Conjugação (**$\overline{A}$**):** Troca-se o sinal da parte imaginária. 

$$
\overline A = \begin{bmatrix} 
1+i & 0 & 3 \\
2-3i & 4 & -i  \\ 
0 & 0 & 6+4i
\end{bmatrix}
$$

2. **Transposição (**$(\overline{A})^T$**):** Trocam-se linhas por colunas.

$$
A^* = 
\begin{bmatrix} 1+i & 2-3i & 0 \\
 0 & 4 & 0 \\ 
 3 & -i & 6+4i 
\end{bmatrix}
$$

## Teoremas

1. Sejam $A$ e $B$ matrizes sobre $\mathbb{K}$ e $\alpha \in \mathbb{K}$. Então, sempre que as operações seguintes estejam definidas, tem-se:
	1. $(A^*)^* = A$
	2. $(A + B)^* = A^* + B^*$
	3. $(\alpha A)^* = \overline \alpha A^*$
	4. $(AB)^* = B^*A^*$
	5. $(A^k)^* = (A^*)^k, \forall k \in \mathbb{N}_{0}$
