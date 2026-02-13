---
title: Computadores
description:
aliases:
  - Computador
  - computadores
  - Computadores
  - computação
  - Computação
draft: true
date: 2026-02-07
tags:
  - computing
parent:
criado: 2026-02-05T13:46:44Z
modificado: 2026-02-08T15:46:18Z
---
## O que é um Computador?

Um **computador** é uma máquina que pode ser programada para executar uma sequência determinada de operações automaticamente. A função primária envolve três pilares:

1. **Armazenar** ([[Memória]])
2. **Recuperar** (Fetch)
3. **Processar** ([[Processamento de Dados]])

> [!info]- Definição de Programa
>  Uma sequência de instruções que descreve uma tarefa a ser performada é chamada de **[[Programa]]**. Este, geralmente, é escrito em uma [[programming language|Linguagem de Programação]].

Um computador pode ser visto como um conjunto de camadas.

> [!NOTE]- Diagrama
> ```mermaid
> graph TD
>     %% Nós
>     L6[Level 6<br/>usuário]
>     L5[Level 5<br/>linguagem de alto nível]
>     L4[Level 4<br/>linguagem assembly]
>     L3[Level 3<br/>Máquina do Sistema Operacional]
>     L2[Level 2<br/>ISA]
>     L1[Level 1<br/>Microarquitetura]
>     L0[Level 0<br/>Lógica Digital]
> 
>     %% Conexões
>     L6 --- L5
>     L5 -- Tradução (compilador) --> L4
>     L4 -- Tradução (montador) --> L3
>     L3 -- interpretação parcial (SO) --> L2
>     L2 -- Execução direta ou <br/>interpretação (microprograma) --> L1
>     L1 -- hardware --> L0
> ```
> 

A camada 6 é a qual todos estão acostumados com, é lá que está contido softwares como 
### Capacidades do Hardware

Os [[Circuitos Digitais|circuitos eletrônicos]] de um computador (especificamente na [[CPU]]) são capazes de executar um conjunto restrito de instruções simples, tais como:

- **Aritmética:** Somar dois números.
- **Lógica:** Verificar se um número é igual a outro (operações booleanas).
- **Movimentação:** Copiar informação de uma parte da memória para outra.
- **Controle de Fluxo:** Decidir qual próxima instrução executar baseado em uma [[Condicional|condição lógica]].


> [!NOTE] Linguagem de Máquina
> Essas instruções primitivas constituem uma linguagem, a [[programming language|linguagem de máquina]], que é usada por programadores para operar um computador.



## Diferença: Computador vs. Calculadora

Embora ambos processem números, um dispositivo só é classificado formalmente como um **computador de uso geral** se possuir ambas as características abaixo. Isso é o que permite a flexibilidade de software.

### 1. Sequência de Instrução Dependente de Dados

É a habilidade de criar ramos de execução condicional (Branching).

- O sistema pode escolher executar o "Caminho A" ou o "Caminho B" dependendo de valores que **só são conhecidos durante a execução** do programa (Runtime).
- _Exemplo:_ `Se X > 10, faça Y; senão, faça Z`.

### 2. Seleção de Informação Dependente de Dados

É a habilidade de usar uma informação para localizar outra informação (Endereçamento Indireto ou [[ponteiro|Ponteiros]]).

- O computador usa um dado processado para determinar **onde** na memória buscar o próximo dado.
- Isso permite estruturas complexas como [[Arrays]], listas ligadas e bancos de dados.

> [!summary]- Resumo
>  Uma calculadora simples segue uma sequência
>  linear fixa. Um computador adapta sua execução e se acesso à memória baseando-se nos próprios dados que está processando.

