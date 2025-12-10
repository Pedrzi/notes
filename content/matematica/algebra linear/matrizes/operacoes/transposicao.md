---
title: Matriz Transposta
description:
aliases:
  - transposta
  - Transposição de Matrizes
draft: false
date: 2025-12-04
tags:
  - matemática
parent:
  - "[[matematica/algebra linear/matrizes/index|index]]"
---

## Definição

Seja $A$ uma [[matematica/algebra linear/matrizes/index|matriz]] $m \times n$. Então $A^T$, a transposta de $A$, denota a matriz obtida por: 

$$
A^T = [a_{ij}]^T = [a_{ji}]
$$

O elemento $(i,j)$ de $A$ vira o elemento $(j,i)$ de $A^T$.

Isso é, as colunas da matriz $A$ tornam-se as linhas e vice-versa.

**Exemplo:**

$$
A =
\begin{bmatrix}
1 & 2 & 3  \\
4 & 5 & 6 \\
7 & 8 & 9
\end{bmatrix}
$$
$$
A^T = 
\begin{bmatrix}
1 & 4 & 7 \\
2 & 5 & 8  \\
3 & 6 & 9
\end{bmatrix}
$$

## Propriedades

1. $(A^T)^T = A$
2. $(AB)^T = B^TA^T$
3. $(sA)^T = sA^T$
4. $(rA + sB)^T = rA^T + sB^T$
