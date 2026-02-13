---
title: dominio e imagem
description: Definição de domínio e imagem (contradomínio) de uma relação binária.
aliases: [domínio de uma relação, imagem de uma relação]
draft: false
date: 2026-01-08
tags: [math]
parent:
  - "[[matematica/relacoes binarias/index|Relacao Binaria]]"
criado: 2026-02-05T13:46:44Z
modificado: 2026-02-06T11:58:19Z
---

## Definições

Seja $R$ uma [[matematica/relacoes binarias/index|Relação Binária]] de $A$ em $B$ (ou seja, $R \subseteq A \times B$).

### Domínio

O **domínio** de $R$, denotado por $D_R$ (ou $\text{Dom}(R)$), é o conjunto de todos os primeiros elementos dos pares ordenados que pertencem a $R$. Ou seja, são os elementos de $A$ que estão relacionados com alguém.

$$
D_R = \{ x \in A : \exists y \in B, (x, y) \in R \}
$$

Note-se que $D_R \subseteq A$.

### Imagem

A **imagem** (ou contradomínio) de $R$, denotada por $Im_R$ (ou $\text{Img}(R)$), é o conjunto de todos os segundos elementos dos pares ordenados que pertencem a $R$.

$$
Im_R = \{ y \in B : \exists x \in A, (x, y) \in R \}
$$

Note-se que $Im_R \subseteq B$.

### Exemplo

Seja $A = \{1, 2, 3\}$, $B = \{a, b, c\}$ e $R = \{(1, a), (1, b), (3, c)\}$.

- **Domínio:** $D_R = \{1, 3\}$ (o 2 não está relacionado com ninguém).
- **Imagem:** $Im_R = \{a, b, c\}$ (todos os elementos de B são atingidos).
