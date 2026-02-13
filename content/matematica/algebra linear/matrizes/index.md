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
  - math
criado: 2026-02-05T13:46:45Z
modificado: 2026-02-07T13:19:28Z
---
# Matrizes

## Definição

Uma **matriz** é um arranjo retangular de escalares (números reais ou complexos), organizados em linhas horizontais e colunas verticais.

Formalmente, uma matriz sobre um corpo $\mathbb{K}$ (como $\mathbb{R}$ ou $\mathbb{C}$) é uma função $A: \{1, \dots, m\} \times \{1, \dots, n\} \to \mathbb{K}$.

> [!note]- Notação Básica
> O conjunto de todas as matrizes com $m$ linhas e $n$ colunas com entradas em $\mathbb{K}$ é denotado por $\mathcal{M}_{m \times n}(\mathbb{K})$.

> [!NOTE]- Notação Indexada
> Cada elemento individual de uma matriz é identificado pela sua posição única, denotada por $a_{ij}$ (ou $A_{i,j}$), onde:
> 
> - $i$ representa o índice da **linha** ($1 \leq i \leq m$).
> - $j$ representa o índice da **coluna** ($1 \leq j \leq n$). 
> 
> Genericamente, uma matriz $A$ de ordem $m \times n$ é representada como:
> 
> $$A = [a_{ij}] = \begin{bmatrix} a_{11} & a_{12} & \cdots & a_{1n} \\ a_{21} & a_{22} & \cdots & a_{2n} \\ \vdots & \vdots & \ddots & \vdots \\ a_{m1} & a_{m2} & \cdots & a_{mn} \end{bmatrix}$$
> 

### Ordem da Matriz

A **ordem** (ou tipo) de uma matriz é descrita pelo formato $m \times n$.

- $m$: número de linhas.
- $n$: número de colunas.

**Exemplos:**

A matriz $A$ é de ordem $3 \times 3$ ([[matriz quadrada|quadrada]]):

$$A = 
\begin{bmatrix} 
1 & 2 & 3 \\ 
4 & 5 & 6 \\ 
7 & 8 & 9  
\end{bmatrix}$$

A matriz $B$ é de ordem $2 \times 4$ (retangular):

$$B = \begin{bmatrix}
1 & 0 & -2 & 5 \\ 3 & 4 & 0 & 1 
\end{bmatrix}$$
### Classificações Básicas

Com base nas dimensões $m$ e $n$, definimos:

- **Matriz Linha:** Uma matriz de ordem $1 \times n$ (apenas uma linha).
    - Exemplo: $v = \begin{bmatrix} 1 & 2 & 3 \end{bmatrix}$.
- **Matriz Coluna:** Uma matriz de ordem $m \times 1$ (apenas uma coluna).
    - Exemplo: $u = \begin{bmatrix} 1 \\ 2 \\ 3 \end{bmatrix}$.
- **Matriz Nula (**$0_{m \times n}$**):** Uma matriz onde todos os elementos são iguais a zero ($a_{ij} = 0, \forall i,j$).

## Propriedades
### Igualdade de Matrizes

Duas matrizes $A$ e $B$ são consideradas **iguais** ($A=B$) se, e somente se:

1. Possuem a mesma ordem ($m \times n$).
2. Todos os elementos correspondentes são iguais ($a_{ij} = b_{ij}$ para todo $i, j$).

## Tipos de Matrizes

### Matriz Inversa

Seja $A \in \mathcal{M}_{n}(\mathbb{K})$ uma [[matriz quadrada|Matrizes Quadradas]] de ordem $n$.

Diz-se que $A$ é **invertível** se existir uma única [[matematica/algebra linear/matrizes/index|matriz]] $B \in \mathcal{M}_{n}(\mathbb{K})$ tal que:

$$
AB = BA = I_n
$$

Onde $I_n$ é a [[Matriz Identidade]] de ordem $n$. A [[matematica/algebra linear/matrizes/index|matriz]] $B$ é designada por **inversa** de $A$ e representa-se por $A^{-1}$.

> [!warning]- Atenção
>  Uma [[matriz quadrada]] que **não** admite inversa diz-se **singular** ou **não invertível**.

> [!NOTE]- Verificando a inversa
> Para verificar se $B$ é inversa de $A$:
> 
> $$
> A = \begin{bmatrix} 1 & 2 \\ 1 & 1 \end{bmatrix}, \quad B = \begin{bmatrix} -1 & 2 \\ 1 & -1 \end{bmatrix}
> $$
> 
> Calculando o produto:
> 
> $$
> AB = \begin{bmatrix} 1(-1)+2(1) & 1(2)+2(-1) \\ 1(-1)+1(1) & 1(2)+1(-1) \end{bmatrix} = \begin{bmatrix} 1 & 0 \\ 0 & 1 \end{bmatrix} = I_2
> $$
> 
> Logo, $B = A^{-1}$.

#### Propriedades

Sejam $A$ e $B$ matrizes invertíveis de ordem $n$ e $\lambda$ um [[escalar]] não nulo ($\lambda \neq 0$).

1. **Involução:** A inversa da inversa é a própria matriz original.
$$
(A^{-1})^{-1} = A
$$
2. **Inversa do Produto:** A inversa de um produto é o produto das inversas **por ordem inversa**.
$$
(AB)^{-1} = B^{-1}A^{-1}
$$
3. **Inversa da [[transposicao|Transposta]]:** A operação de inversão comuta com a [[transposicao|transposição]].
$$
(A^T)^{-1} = (A^{-1})^T
$$

#### Teorema: Unicidade da Inversa

Este teorema prova que se uma matriz possui inversas à esquerda e à direita, elas devem ser iguais, garantindo a unicidade da inversa.

Sejam $n \in \mathbb{N}$ e $A, B, C \in \mathcal{M}_{n}(\mathbb{K})$. Se $AB = I_n$ e $CA = I_n$, então $B = C$, $A$ é invertível e $A^{-1} = B = C$.

**Demonstração:**

Admitamos que $AB = I_n$ e $CA = I_n$. Então:

$$C = C I_n = C(AB) = (CA)B = I_n B = B$$

Portanto, $A$ é invertível e $A^{-1} = B$.

##### Condição de Verificação Simplificada

Embora a definição formal exija a verificação da comutatividade ($AB=I$ e $BA=I$), para matrizes quadradas basta verificar um dos lados.

> [!info]- Teorema
>  Se $A$ e $B$ são matrizes quadradas de ordem $n$ e $AB = I_n$, então conclui-se automaticamente que $BA = I_n$, logo $B = A^{-1}$.


## Operações



## Submatrizes