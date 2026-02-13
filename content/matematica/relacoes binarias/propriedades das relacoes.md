---
title: propriedades das relacoes
description:
aliases: [Propriedades das Relações]
draft: false
date: 2026-01-08
tags: [math]
parent:
  - "[[matematica/relacoes binarias/index|Relacao Binaria]]"
criado: 2026-02-05T13:46:44Z
modificado: 2026-02-06T11:58:19Z
---

## Propriedades Fundamentais

Seja $R$ uma relação binária num conjunto $A$ (ou seja, $R \subseteq A \times A$). Dizemos que $R$ é:

### 1. Reflexiva

Cada elemento está relacionado consigo próprio.

$$
\forall x \in A, \quad (x, x) \in R
$$

_(Exemplo: Relação "ser igual a" ou "ser menor ou igual a")._

### 2. Simétrica

Se um elemento está relacionado com outro, o inverso também é verdade.

$$
\forall x, y \in A, \quad (x, y) \in R \implies (y, x) \in R
$$

_(Exemplo: Relação "ser irmão de")._

### 3. Antissimétrica

Se dois elementos distintos estão relacionados num sentido, não podem estar no outro. Se estiverem nos dois sentidos, têm de ser o mesmo elemento.

$$
\forall x, y \in A, \quad [(x, y) \in R \land (y, x) \in R] \implies x = y
$$

_(Exemplo: Relação "ser menor ou igual a",_ $\le$_)._

### 4. Transitiva

Se $x$ está relacionado com $y$ e $y$ com $z$, então $x$ está relacionado com $z$.

$$
\forall x, y, z \in A, \quad [(x, y) \in R \land (y, z) \in R] \implies (x, z) \in R
$$

_(Exemplo: Relação "ser maior que",_ $>$_)._
