---
title: Funcao Sobrejetiva
description:
aliases:
  - função sobrejetiva
  - Função sobrejetiva
  - Função Sobrejetiva
  - sobrejetividade
  - Sobrejetividade
  - função sobrejetora
  - Função sobrejetora
  - Função Sobrejetora
  - sobrejetora
  - Sobrejetora
  - função sobrejectiva
  - Função sobrejectiva
  - Função Sobrejectiva
  - sobrejectiva
  - Sobrejectiva
  - função onto
  - Função onto
  - onto
  - sobrejetiva
  - Sobrejetiva
draft: false
date: 2026-01-08
tags:
  - matemática
  - função
parent:
  - "[[matematica/funcoes/index]]"
---

## Definição

Uma função $f: A \to B$ é sobrejetiva quando todo elemento de $B$ é imagem de algum elemento de $A$.

$$
\forall_{y \in B} \exists _{x \in A} f(x) = y.
$$

De forma equivalente, $f$ é sobrejetiva quando o [[matematica/funcoes/index|contradomínio]] de $f$ coincide com o seu conjunto de chegada, ou seja, $f(A) = B$.

## Prova de Sobrejetividade

Para provar que uma função sobrejetiva, temos que ter uma função $f : X \to Y$ tal que a imagem $im(X)$ de $f$ é igual ao [[matematica/funcoes/index|contradomínio]] $Y$. Suponha um elemento $y \in Y$ arbitrário e mostre que existe um elemento $x \in X$ para que $f(x) = y$.

### Exemplo

Seja $f : \mathbb{R} \to \mathbb{R}$ tal que  $f(x) = x+1$.

Suponha $y \in \mathbb{R}$. Temos $f(x) = x + 1 = y$ o que implica $x = y - 1$. Note que $(y-1) \in \mathbb{R}$ para todo $y$ em $\mathbb{R}$. Portanto, segue da definição que $f$ é sobrejetiva. 
