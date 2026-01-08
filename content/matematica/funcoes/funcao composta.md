---
title: Função Composta
description:
aliases:
  - Funcao Composta
  - Função Composta
  - Composta
  - composta
  - Função composta
  - função composta
draft: false
date: 2026-01-08
tags:
  - matemática
parent:
  - "[[matematica/funcoes/index]]"
---

## Definição

Sejam $A, B, C$ conjuntos e $f: A \to B$, $g : B \to C$ funções. Então, a correspondência de $A$ para $C$ que a cada elemento $x$ de $A$ faz corresponder o elemento $g(f(x))$ de $C$ é uma função de $A$ para $C$.

> [!note]- Notação
> A composta de duas funções pode ser notada como:
> $$
> f \circ g
> $$
> Essa notação é lida como $f$ após $g$.

## Propriedades

Sejam $A,B,C,D$ conjuntos e $f : A \to B$, $g : B \to C$ e $h : C \to D$ funções. Então:

1. $(h \circ g) \circ f = h \circ (g \circ f)$
2. $id_{B} \circ f = f = f \circ id_{A}$
3. Se $f$ e $g$ são [[funcao injetiva|injetivas]], então $g \circ f$ é injetiva.
4. Se $f$ e $g$ são sobrejetivas, então $g \circ f$ é sobrejetiva.
5. Se $f$ e $g$ são bijetivas, então $g \circ f$ é bijetiva.