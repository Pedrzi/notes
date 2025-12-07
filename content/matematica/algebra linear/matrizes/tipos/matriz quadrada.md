---
title: Matrizes Quadradas
description:
aliases:
date: 2025-12-04
tags:
  - matemática
  - matriz
parent:
  - "[[matematica/algebra linear/matrizes/index|index]]"
---

## Definição

Uma **Matriz Quadrada** é uma matriz onde o número de linhas ($m$) é estritamente igual ao número de colunas ($n$).

Dizemos que $A$ é uma matriz quadrada de **ordem** $n$. O conjunto dessas matrizes sobre um corpo $\mathbb{K}$ é denotado por $\mathcal{M}_{n}(\mathbb{K})$.

> [!info]- Notação
>  - Na notação padrão $\mathcal{M}_{m \times n}$, o índice $m$ é omitido, resultando em $\mathcal{M}_{n}$
>  
>  - Uma matriz de ordem $n$ também pode ser representada por $A=[a_{ij}]_{n}$

### Exemplo ($\mathcal{M}_{3}(\mathbb{R})$)

$$
A = \begin{bmatrix} 1 & 2 & 3 \\ 4 & 5 & 6 \\ 7 & 8 & 9 \end{bmatrix}
$$

## Estrutura das Diagonais

### Diagonal Principal

Formada pelos elementos $a_{ij}$ onde $i=j$ *(do canto superior esquerdo ao inferior direito)*.

- _Exemplo acima:_ $1, 5, 9$.
- Os elementos $a_{ii}$ são designados por **elementos principais**.
- A diagonal diz-se **positiva** se $a_{ii} > 0$ para todo $i$, e **não negativa** se $a_{ii} \ge 0$.
- A soma destes elementos define o [[traco da matriz]].

### Diagonal Secundária

Formada pelos elementos $a_{ij}$ onde $i + j = n + 1$ *(do canto superior direito ao inferior esquerdo)*.

- _Exemplo acima:_ $3, 5, 7$.

## Tipos Notáveis de Matrizes Quadradas

A estrutura quadrada permite classificações baseadas na disposição dos zeros, simetria e inversão:

- **Por disposição de elementos (Triangulação):**
    - [[matriz triangular|Matriz Triangular]] *(Superior, Inferior e Diagonal)*
- **Por Simetria (Transposição):**
    - [[matriz simetrica|Matriz Simétrica]] *($A = A^T$)*
    - [[matriz hermitiana|Matriz Hermítica]] *(Complexa: $A = A^*$)*
- **Por Ortogonalidade e Inversão:**
    - [[matriz inversa|Matriz Inversível]] *($\det(A) \neq 0$)*
    - [[matriz ortogonal|Matriz Ortogonal]] *(Real: $A^{-1} = A^T$)*
    - [[matriz unitaria|Matriz Unitária]] *(Complexa: $A^{-1} = A^*$)*
- **Outros:**
    - [[matriz definida positiva|Matriz Definida Positiva]]
