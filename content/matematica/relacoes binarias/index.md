---
title: index
description:
aliases: [Relacao Binaria, Relação Binária, Relação binária, relação binária]
draft: false
date: 2026-01-08
tags: [math]
parent:
criado: 2026-02-05T13:46:44Z
modificado: 2026-02-06T11:58:19Z
---

## Definição

Uma **relação binária** é um conjunto de pares ordenados onde os elementos são pares $(a,b)$ indicando que $a$ está associado a $b$.

Formalmente, dados dois conjuntos $A$ e $B$, uma relação binária de $A$ em $B$ (ou correspondência de $A$ para $B$) é qualquer subconjunto $R$ do produto cartesiano $A \times B$.

$$
R \subseteq A \times B
$$

- **Conjunto de Partida:** O conjunto $A$.
- **Conjunto de Chegada:** O conjunto $B$.

> [!info] Relação em $A$ 
> Quando $A = B$, dizemos simplesmente que $R$ é uma **relação binária em** $A$.

## Notação

- Quando $(a, b) \in R$, dizemos que $a$ está relacionado com $b$ por $R$ e escrevemos:

$$
a \ R \ b
$$
- Quando $(a, b) \notin R$, dizemos que $a$ **não** está relacionado com $b$ por $R$ e escrevemos:

$$
a \ \cancel{R} \ b
$$

## Conjunto das Relações

Dados dois conjuntos $A$ e $B$, o conjunto de todas as relações binárias possíveis de $A$ em $B$ é o conjunto das partes do produto cartesiano, denotado por $\mathcal{P}(A \times B)$.

### Cardinalidade

Se os conjuntos $A$ e $B$ forem finitos e tiverem, respetivamente, $n$ e $m$ elementos, então o número total de relações possíveis é dado por:

$$
|\mathcal{P}(A \times B)| = 2^{n \times m}
$$

## Relações Especiais

### Relação Vazia e Universal

- **Relação Vazia:** O conjunto vazio $\emptyset$ é uma relação binária de $A$ em $B$.
- **Relação Universal:** O conjunto total $A \times B$ é a relação universal de $A$ em $B$.

### Relações em $A$

Seja $A$ um conjunto não vazio. Destacam-se duas relações fundamentais:

1. **Relação Identidade (**$id_A$**):** Associa cada elemento apenas a si próprio.

$$
id_{A} = \{(a,a) : a \in A\}
$$

2. **Relação Universal em** $A$ **(**$\omega_A$**):** Associa todos os elementos a todos os elementos (o quadrado cartesiano).
 
$$
\omega _{A} = A^{2} = \{(x,y) : x,y \in A\}
$$
