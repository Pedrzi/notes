---
title: Funções
description:
aliases:
  - Funcao
  - Função
  - função
  - aplicação
  - Aplicação
  - domínio
  - Domínio
  - Codomínio
  - codomínio
  - contradomínio
  - Contradomínio
draft: false
date: 2026-01-08
tags:
  - matemática
  - função
parent:
---

## Definição

Sejam $A$ e $B$ conjuntos. Uma **função**, ou **aplicação**, de $A$ em $B$ é uma correspondência de $A$ para $B$, que cada elemento de $A$ é mapeado em um e apenas um elemento de $B$.

> [!note]- Notação
> Funções são representadas por letras minúculas $f$, $g$, $h$,...
> Escrevemos para uma função $f$ de $A$ em $B$ podemos escrever:
> $$
> \begin{align}
> f : & \ A \to B \\
> & a \mapsto f(a)
> \end{align}
> $$
> Onde $a \in A$ 

> [!note]- Notação
> O conjunto de todas as funções de $A$ para $B$ é escrito como:
> $$
>  B^A 
> $$
> 

### Domínio

Domínio ou conjunto de partida de $f$ é o conjunto $A$.

### Codomínio

Codomínio ou conjunto de chegada de $f$ é o conjunto $B$.

### Imagem

A Imagem ou o contradomínio de $f$ é o conjunto de todos os resultados de $f$ para cada elemento de $A$, ou seja:

$$
\mathrm{Im}(f) = \{f(x) : x \in A\} 
$$

Seja $X$ um subconjunto de $A$ e $Y$ um subconjunto de $B$.

#### Imagem de um Subconjunto

A imagem de $X$ é o conjunto: 

$$
f(X) = \{ f(x) : x \in X \}
$$

#### Imagem Inversa

A imagem inversa ou pré-imagem de $Y$ por $f$ é o conjunto 

$$
f^{-1} (Y) = \{ x \in A : f(x) \in Y \}
$$

> [!note]- Notação
> A imagem inversa de $Y$ por $f$ é também notada como $f^{\leftarrow}(Y)$

### Igualdade de Funções

Sejam $A_1, A_2, B_1, B_2$ conjuntos e sejam $f : A_{1} \to B_{1}$, $g : A_{2} \to B_{2}$ funções. Dizemos que as funções $f$ e $g$ são iguais, e escrevemos $f = g$, quando:

1. $A_1 = A_{2}$;
2. $B_{1} = B_{2}$;
3. $\forall x \in A_{1}, f(x) = g(x)$.

## Propriedades

Dada uma função $f : A \to B$. onde $A$ e $B$ são conjuntos e $A_{1} , A_{2} \subseteq A$ e $B_{1} , B_{2} \subseteq B$. Então,

1. $f(\emptyset) = \emptyset$
2. $f(A) \subseteq B$
3. $A_{1} \subseteq A_{2} \implies f(A_{1}) \subseteq f(A_{2})$
4. $f(A_{1} \cup A_{2}) = f(A_{1}) \cup f(A_{2})$
5. $f^{-1} (\emptyset) = \emptyset$
6. $f^{-1}(B) = A$
7. $B_{1} \subseteq B_{2} \implies f^{-1}(B_{1}) \subseteq f^{-1} (B_{2})$
8. $f^{-1} (B_{1} \cup B_{2}) = f^{-1} (B_{1}) \cup f^{-1}(B_{2})$
9. $f^{-1} (B_{1} \cap B_{2}) = f^{-1}(B_{1}) \cap f^{-1} (B_{2})$
