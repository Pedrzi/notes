---
title: "regra de l'hopital"
description: Também conhecida como regra de Bernoulli.
aliases: [Regra De L'Hopital, Regra de L'Hôpital, regra de bernoulli, Regra de Bernoulli]
draft: false
date: 2025-12-15
tags: [math]
parent:
criado: 2026-02-05T13:46:44Z
modificado: 2026-02-06T11:58:19Z
---

## Teorema

A **Regra de L'Hôpital**, ou regra de [[johann bernoulli|Bernoulli]] permite calcular limites indeterminados derivando separadamente o numerador e o denominador.

> [!info]- Enunciado
>  Sejam $f$ e $g$ funções diferenciáveis num intervalo aberto contendo $a$ (exceto possivelmente em $a$), onde $g'(x) \neq 0$.
> 
> Se o [[limite]] $\lim_{x \to a} \frac{f(x)}{g(x)}$ resulta numa indeterminação do tipo:
> 
> $\frac{0}{0}$ ($\lim f(x) = 0$ e $\lim g(x) = 0$)
> ou
> $\frac{\infty}{\infty}$ ($\lim f(x) = \pm\infty$ e $\lim g(x) = \pm\infty$)
>  
> 
> Então:
> 
> $$
> \lim_{ x \to a } \frac{f(x)}{g(x)} = \lim_{ x \to a } \frac{f'(x)}{g'(x)}
> $$
> 
> _Desde que o [[limite]] à direita exista (finito ou infinito)._

> [!warning]- Atenção
>  Não confundir com a [[derivada#4. Regra do Quociente|Regra do Quociente]]. Na Regra de L'Hôpital, deriva-se o numerador e o denominador **independentemente**.
> 
> $$
> \frac{d}{dx}\left(\frac{f}{g}\right) \neq \frac{f'}{g'}
> $$

## Exemplos de Aplicação

### Caso $\frac{0}{0}$

Calcular $\lim_{x \to 0} \frac{\sin x}{x}$.

$\sin(0) = 0$ e $0 = 0$. Então temos $\frac{0}{0}$.

$f'(x) = \cos x$
$g'(x) = 1$

Aplicando a regra temos:

$$
\lim_{x \to 0} \frac{\cos x}{1} = 1
$$

### Caso $\frac{\infty}{\infty}$

Calcular $\lim_{x \to \infty} \frac{e^x}{2x}$.

$e^\infty \to \infty$ e $2(\infty) \to \infty$. Então temos $\frac{\infty}{\infty}$.

$f'(x) = e^x$
$g'(x) = 2$ 

Aplicando a regra temos:
$$
\lim_{x \to \infty} \frac{e^x}{2} = \infty
$$

