---
title: Injetividade
description:
aliases:
  - função injetiva
  - Função injetiva
  - Função Injetiva
  - injetividade
  - Injetividade
  - função injetora
  - Função Injetora
  - Função injetora
  - injectiva
  - Injectiva
  - função injectiva
  - Função Injectiva
  - Injetiva
  - injetiva
draft: false
date: 2025-12-19
tags:
  - matemática
  - função
parent:
  - "[[matematica/funcoes/index]]"
---

## Definição

Injetividade é a preservação da distinção dos elementos de uma função, ou seja, uma função $f : A \to B$ é injetiva quando para quaisquer dois elementos distintos do conjunto $A$ eles tem imagens distintas por $f$.

$$
\forall _{x, y \in A} (x \neq y \implies f(x) \neq f(y))
$$

ou

$$
\forall_{x, y \in A} (f(x) = f(y) \implies x=y)
$$

ou

$$
\neg \exists _{x, y \in A} (x \neq y \land f(x) = f(y))
$$

## Prova da Injetividade

Uma prova de que a função $f$ é injetiva depende de como a função é apresentada e quais propriedades ela contém. Para funções que são dadas por alguma fórmula, há uma ideia básica. Usamos a contra positiva da definição de injetividade, Então:

$$
f(x) = f(y) \implies x = y
$$

### Exemplos

$$
f = 2x + 3
$$

Seja $f : X \to Y$. Suponha que $f(x) = f(y)$. Então:

$$
2x + 3 = 2y + 3 \implies 2x = 2y \implies x = y
$$

Portanto, por definição $f$ é injetiva.

$$
g(x) = \frac{2x+5}{1+x^{2}}
$$

$g(x)$ não é injetiva, já que para $g(0)$ e $g\left( \frac{2}{5} \right)$ temos $g(0) = g\left( \frac{2}{5} \right)$, ou seja, $g(x) = g(y)$ com $x \neq y$. 

### Outros Métodos

#### [[derivada|Derivação]]

Se uma função é diferenciável e definida em algum intervalo, então é suficiente mostrar que a derivada é sempre positiva ou sempre negativa nesse intervalo.

#### [[aplicacao linear|Transformações lineares]]

Se $f$ é uma transformação linear então é suficiente mostrar que o [[nulidade|núcleo]] de $f$ só contém o [[matematica/algebra linear/vetores/index|vetor]] zero.

#### Domínio Finito

É possível verificar todas as imagens de cada elemento e verificar se nenhuma imagem ocorre duas vezes.