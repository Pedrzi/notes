---
title: Aplicação Linear
description:
aliases:
  - Aplicacao Linear
  - Aplicação linear
  - aplicação linear
  - Aplicação Linear
  - transformação linear
  - Transformação linear
  - Mapa linear
  - mapa linear
  - aplicações lineares
  - Aplicações lineares
  - mapas lineares
  - Transformações lineares
  - transformações lineares
draft: true
date: 2025-12-19
tags:
  - matemática
parent:
---

## Definição

Uma **aplicação linear** (ou transformação linear) é uma função $f: V \to V'$ entre dois [[Espaço Vetorial|espaços vetoriais]] $V$ e $V'$ (sobre o mesmo corpo $\mathbb{K}$) que preserva as operações de adição vetorial e multiplicação por [[escalar]].

Para que $f$ seja linear, deve satisfazer simultaneamente duas condições para quaisquer [[matematica/algebra linear/vetores/index|vetores]] $u, v \in V$ e qualquer [[escalar]] $\lambda \in \mathbb{K}$:

1. **Aditividade (Preservação da Soma):**
 $$
 f(u + v) = f(u) + f(v)
 
$$
 
2. **Homogeneidade (Preservação da Escala):**
$$
f(\lambda v) = \lambda f(v)
$$

> [!info]- [[combinacao linear|Combinação Linear]]
>  Estas duas propriedades podem ser resumidas numa única condição: $f$ preserva [[Combinação Linear|combinações lineares]].
> 
> $$
> f(\alpha u + \beta v) = \alpha f(u) + \beta f(v)
> $$

## Propriedades Importantes

### 1. Elemento Neutro

Uma consequência imediata da definição é que toda a aplicação linear mapeia o vetor nulo do domínio no vetor nulo do contradomínio:

$$
f(0_V) = 0_{V'}
$$

### 2. [[nulidade|Núcleo]] e [[funcao injetiva|Injetividade]]

O **[[nulidade|Núcleo]]** (ou _Kernel_) de $f$, denotado por $\ker(f)$ ou $N(f)$, é o conjunto de [[matematica/algebra linear/vetores/index|vetores]] em $V$ que são mapeados para o zero em $V'$.

$$
\ker(f) = \{ v \in V : f(v) = 0_{V'} \}
$$

- **Teorema:** Uma aplicação linear $f$ é [[Função Injetiva|injetiva]] se, e somente se, o seu [[nulidade|núcleo]] contiver apenas o vetor nulo ($\ker(f) = \{0_V\}$).

### 3. Imagem e Sobrejetividade

A **Imagem** de $f$, denotada por $\text{Im}(f)$, é o subconjunto de [[matematica/algebra linear/vetores/index|vetores]] em $V'$ que são atingidos pela função.

- **Teorema:** A imagem de uma aplicação linear é sempre um **subespaço vetorial** de $V'$.

### 4. Representação Matricial

Se $V$ e $V'$ têm dimensões finitas ($n$ e $m$, respetivamente), qualquer aplicação linear $f$ pode ser representada univocamente por uma [[matematica/algebra linear/matrizes/index|matriz]] $A$ de ordem $m \times n$.

$$
f(v) = A \cdot v
$$

_(Onde_ $v$ _é representado como um vetor coluna)._
