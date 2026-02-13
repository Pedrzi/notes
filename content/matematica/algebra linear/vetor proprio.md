---
title: vetor proprio
description:
aliases: [autovetor, autovalor, Vetor próprio, Vetor Próprio, valor próprio, Valor próprio]
draft: false
date: 2025-12-04
tags: [math]
parent:
criado: 2026-02-05T13:46:44Z
modificado: 2026-02-06T11:58:19Z
---

## Definição

Um autovetor, ou vetor próprio, é um [[matematica/algebra linear/vetores/index|vetor]] ($v$) não nulo que muda apenas por um valor [[escalar]] $\lambda$ após uma [[aplicacao linear|transformação linear]] $A$.

$$
\begin{align}
 & Av = \lambda v \\
 & Av - \lambda v = 0  \\
 & (A - \lambda I)v = 0
\end{align}
$$

O valor $\lambda$ é dito como autovalor, ou valor próprio de A. Se um dos autovalores for 0 então a [[aplicacao linear|aplicação linear]] é uma [[matriz inversa|matriz singular]].

> [!note]- Condição para $\lambda$ ser um autovalor
> para $lambda$ ser um autovalor de $A$ a seguinte condição precisa ser válida:
> $$\det(A - \lambda I) = 0$$
