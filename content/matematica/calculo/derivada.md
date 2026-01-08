---
title: Derivada
description:
aliases:
draft: false
date: 2025-12-13
tags:
  - matemática
parent:
---
## Definição

A derivada de uma [[matematica/funcoes/index|função]] $f$ num ponto $x$ representa a taxa de variação instantânea de $f$ em relação a $x$. Formalmente, é definida pelo [[limite]]:

$$\frac{df}{dx} = \lim_{ \Delta x \to 0 } \frac{f(x+ \Delta x) - f(x)}{\Delta x}$$

> [!note]- Notação
>  A derivada pode ser denotada por: $f'(x)$, $\dot{f}$ (notação de [[Newton]]), $\frac{df}{dx}$ (notação de [[Leibniz]]) ou $D_{x}f$.

## Regras de Derivação

Para os exemplos abaixo, considere as funções elementares:

$g(x) = \sin x \implies g'(x) = \cos x$
$h(x) = x^2 \implies h'(x) = 2x$

### 1. Regra da Potência

A base para derivar polinómios.

$$
\frac{d}{dx}(x^n) = nx^{n-1}
$$

### 2. Regra da Soma (Linearidade)

A derivada da soma é a soma das derivadas.

$$
\frac{d}{dx}[g(x) + h(x)] = g'(x) + h'(x)
$$

#### Exemplo

$$
\frac{d}{dx}(\sin x + x^2) = \cos x + 2x
$$

### 3. Regra do Produto

$$
\frac{d}{dx}[g(x)h(x)] 
=
g(x)h'(x) + h(x)g'(x)
$$

#### Exemplo

$$
\frac{d}{dx}(x^2 \sin x) 
=
(\sin x)(2x) + (x^2)(\cos x)
$$

### 4. Regra do Quociente

$$
\frac{d}{dx}\left[ \frac{g(x)}{h(x)} \right] 
=
\frac{g'(x)h(x) - g(x)h'(x)}{[h(x)]^2}
$$

#### Exemplo

$$
\frac{d}{dx}\left( \frac{\sin x}{x^2} \right) 
=
\frac{(\cos x)(x^2) - (\sin x)(2x)}{(x^2)^2} 
=
\frac{x\cos x - 2\sin x}{x^3}
$$

### 5. Regra da Cadeia (Composição)

Usada para funções compostas $f(x) = g(h(x))$.

$$
\frac{df}{dx} = g'(h(x)) \cdot h'(x)
$$

#### Exemplo

Seja $f(x) = \sin(x^2)$. Aqui a função "de fora" é seno e a "de dentro" é $x^2$.

$$\frac{df}{dx} = \cos(x^2) \cdot 2x$$