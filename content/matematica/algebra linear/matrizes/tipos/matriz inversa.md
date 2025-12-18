---
title: Matriz Inversa
description:
aliases:
  - Matriz Inversível
  - matriz inversa
  - matriz singular
  - matriz invertível
  - matrizes inversas
  - matrizes invertíveis
  - matrizes inversíveis
draft: false
date: 2025-12-04
tags:
  - matemática
parent:
  - "[[matematica/algebra linear/matrizes/index|index]]"
---

## Definição

Seja $A \in \mathcal{M}_{n}(\mathbb{K})$ uma [[matriz quadrada|Matrizes Quadradas]] de ordem $n$.

Diz-se que $A$ é **invertível** se existir uma única [[matematica/algebra linear/matrizes/index|matriz]] $B \in \mathcal{M}_{n}(\mathbb{K})$ tal que:

$$
AB = BA = I_n
$$

Onde $I_n$ é a [[Matriz Identidade]] de ordem $n$. A [[matematica/algebra linear/matrizes/index|matriz]] $B$ é designada por **inversa** de $A$ e representa-se por $A^{-1}$.

> [!warning] Atenção
>  Uma [[matriz quadrada]] que **não** admite inversa diz-se **singular** ou **não invertível**.

## Teorema: Unicidade da Inversa

Este teorema prova que se uma matriz possui inversas à esquerda e à direita, elas devem ser iguais, garantindo a unicidade da inversa.

> [!info] Teorema
>  Sejam $n \in \mathbb{N}$ e $A, B, C \in \mathcal{M}_{n}(\mathbb{K})$. Se $AB = I_n$ e $CA = I_n$, então $B = C$, $A$ é invertível e $A^{-1} = B = C$.

**Demonstração:**

Admitamos que $AB = I_n$ e $CA = I_n$. Então:

$$
C = C I_n = C(AB) = (CA)B = I_n B = B
$$

Portanto, $A$ é invertível e $A^{-1} = B$.

## Condição de Verificação Simplificada

Embora a definição formal exija a verificação da comutatividade ($AB=I$ e $BA=I$), para matrizes quadradas basta verificar um dos lados.

> [!info] Teorema
>  Se $A$ e $B$ são matrizes quadradas de ordem $n$ e $AB = I_n$, então conclui-se automaticamente que $BA = I_n$, logo $B = A^{-1}$.

## Propriedades

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

### Exemplo de Verificação

Para verificar se $B$ é inversa de $A$:

$$
A = \begin{bmatrix} 1 & 2 \\ 1 & 1 \end{bmatrix}, \quad B = \begin{bmatrix} -1 & 2 \\ 1 & -1 \end{bmatrix}
$$

Calculando o produto:

$$
AB = \begin{bmatrix} 1(-1)+2(1) & 1(2)+2(-1) \\ 1(-1)+1(1) & 1(2)+1(-1) \end{bmatrix} = \begin{bmatrix} 1 & 0 \\ 0 & 1 \end{bmatrix} = I_2
$$

Logo, $B = A^{-1}$.
