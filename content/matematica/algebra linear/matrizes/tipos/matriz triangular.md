---
title: Matrizes Triangulares
description:
aliases:
  - Matriz triangular
  - matriz diagonal
  - Matriz Diagonal
  - Matriz diagonal
  - Matriz Escalar
  - matriz escalar
  - Matriz escalar
draft: false
date: 2025-12-06
tags:
  - matemática
parent:
  - "[[matematica/algebra linear/matrizes/index|index]]"
---

## Definição

Uma [[matriz quadrada]] $A = [a_{ij}]_n$ diz-se **triangular** quando todos os elementos acima ou abaixo da diagonal principal são nulos.

Existem dois tipos fundamentais:

### 1. Triangular Superior

Diz-se **triangular superior** se todos os elementos _abaixo_ da diagonal principal forem zero. Formalmente:

$$
i > j \implies a_{ij} = 0
$$

**Exemplo:**

$$
U =
\begin{bmatrix} 
 1 & 2 & 3 \\ 
 \mathbf{0} & 4 & 5 \\ 
 \mathbf{0} & \mathbf{0} & 6 
\end{bmatrix}
$$

### 2. Triangular Inferior

Diz-se **triangular inferior** se todos os elementos _acima_ da diagonal principal forem zero. Formalmente:

$$
i < j \implies a_{ij} = 0
$$

**Exemplo:**

$$
L =
\begin{bmatrix}  
1 & \mathbf{0} & \mathbf{0}  \\
2 & 3 & \mathbf{0} \\ 
4 & 5 & 6 
 \end{bmatrix}
$$

### 3. Diagonal

Diz-se **diagonal** se é simultaneamente triangular superior e inferior. Formalmente:

$$
i \neq j \implies a_{ij} = 0
$$
**Exemplo:**

$$
D =
\begin{bmatrix}
\mathbf{1} & 0 & 0 \\
0 & \mathbf{2} & 0 \\
0 & 0 & \mathbf{1}
\end{bmatrix}
$$
> [!note] Notação
> Uma matriz diagonal $A = [a_{ij}] \in \mathcal{M}_{n}(\mathbb{K})$ pode representar-se abreviadamente por $A = diag(a_{11}, a_{22}, \dots, a_{nn}).$
> No exemplo anterior, tem-se $D=diag(1,1,1).$

#### Escalar

Uma matriz diagonal diz-se **escalar** se todos os elementos da diagonal forem iguais entre si.

**Exemplo:**

$$
D =
\begin{bmatrix}
\mathbf{1} & 0 & 0 \\
0 & \mathbf{1} & 0 \\
0 & 0 & \mathbf{1}
\end{bmatrix}
$$
> [!tip]- Casos Especiais
> A [[matriz identidade|Matriz Identidade]] e Matriz Nula são alguns dos casos especiais da matriz escalar.