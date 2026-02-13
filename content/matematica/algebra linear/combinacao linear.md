---
title: combinacao linear
description:
aliases: [Combinacao Linear, combinação linear, Combinação linear]
draft: false
date: 2025-12-18
tags: [math]
parent:
criado: 2026-02-05T13:46:44Z
modificado: 2026-02-06T11:58:19Z
---

## Definição

Seja $V$ um espaço vetorial sobre um corpo $\mathbb{K}$ (onde os elementos de $\mathbb{K}$ são chamados de **escalares** e os de $V$ de **[[matematica/algebra linear/vetores/index|vetores]]**).

Uma **combinação linear** é a soma de [[matematica/algebra linear/vetores/index|vetores]] multiplicados por escalares.

Se $v_1, v_2, \dots, v_n$ são [[matematica/algebra linear/vetores/index|vetores]] e $a_1, a_2, \dots, a_n$ são escalares, a combinação linear destes [[matematica/algebra linear/vetores/index|vetores]] com estes coeficientes é expressa por:

$$
w = a_1 v_1 + a_2 v_2 + \dots + a_n v_n = \sum_{i=1}^{n} a_i v_i
$$

## Exemplo

Considere dois [[matematica/algebra linear/vetores/index|vetores]] no plano, $u_1$ e $u_2$. Um [[matematica/algebra linear/vetores/index|vetor]] $v$ é uma combinação linear deles se puder ser "construído" [[multiplicacao de matrizes|escalando]] e [[soma de matrizes|somando]] esses [[matematica/algebra linear/vetores/index|vetores]].

Por exemplo, se $v = 2u_1 + 1.5u_2$:

1. Duplicamos o comprimento de $u_1$ ($2u_1$).
2. Aumentamos $u_2$ em 50% ($1.5u_2$).
3. Somamos os resultados pela [[regra do paralelogramo]].

> [!info]- Importância
>  O conceito de combinação linear é central na [[matematica/algebra linear/index|álgebra linear]]. O conjunto de todas as combinações lineares possíveis de um grupo de [[matematica/algebra linear/vetores/index|vetores]] chama-se **[[span|subespaço gerado]]** (span).
