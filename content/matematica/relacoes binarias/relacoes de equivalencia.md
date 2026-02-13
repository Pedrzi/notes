---
title: relacoes de equivalencia
description:
aliases: [Relacoes De Equivalencia, Relações de Equivalência]
draft: false
date: 2026-01-09
tags: [math]
parent:
criado: 2026-02-05T13:46:44Z
modificado: 2026-02-06T11:58:19Z
---
## Definição


## Definição

Uma relação binária $R$ num conjunto $A$ diz-se uma **relação de equivalência** se verificar, simultaneamente, as três propriedades seguintes:

1. **Reflexiva** ($xRx$)
2. **Simétrica** ($xRy \implies yRx$)
3. **Transitiva** ($xRy \land yRz \implies xRz$)

O objetivo de uma relação de equivalência é agrupar elementos que partilham uma certa característica comum.

## Classe de Equivalência

Seja $R$ uma relação de equivalência em $A$ e $x \in A$. A **classe de equivalência** de $x$, denotada por $[x]_R$ (ou $\bar{x}$), é o subconjunto de $A$ formado por todos os elementos que estão relacionados com $x$:

$$
[x]_R = \{ y \in A : (x, y) \in R \}
$$

> [!info] Partição
>  O conjunto de todas as classes de equivalência forma uma **partição** de $A$. Ou seja, a união das classes é o conjunto $A$ todo, e a interseção entre classes distintas é vazia.

## Conjunto Quociente

O conjunto de todas as classes de equivalência define-se como o **conjunto quociente** de $A$ por $R$, denotado por $A/R$:

$$
A/R = \{ [x]_R : x \in A \}
$$
