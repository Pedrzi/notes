---
title: Git
description:
aliases:
  - Git
  - GIT
  - usando git
  - Usando git
draft: false
date: 2026-05-02
tags:
criado: 2026-02-05T13:46:44Z
modificado: 2026-02-13T13:49:14Z
---
## O que é?

O **Git** é um sistema de [[Controle de Versão]] distribuído (DVCS), capaz de gerenciar o histórico de versões de [[Código Fonte]] ou dados. É a ferramenta padrão para programadores desenvolverem software colaborativamente.

### O git é especial

A principal diferença entre o Git e outros sistemas (como Subversion ou CVS) é como ele enxerga os dados.

- **Outros VCS:** Armazenam informações como uma lista de mudanças baseadas em arquivos (_delta-based_).
- **Git:** Pensa nos dados como uma série de **Snapshots** de um mini sistema de arquivos.

> [!INFO]- Snapshot?
>  Toda vez que você faz um `commit` (salva o estado), o Git tira uma "foto" de como todos os seus arquivos estão naquele exato momento e armazena uma referência para essa foto.
> 
> Se um arquivo não mudou, o Git não o armazena de novo; ele apenas cria um link para o arquivo idêntico anterior já armazenado.

## Guia de Uso

### Três Estados

Para entender os comandos, você precisa entender que o Git gerencia os arquivos em três áreas distintas dentro do projeto:

#### 1. Working Directory

É a pasta onde você mexe nos seus arquivos, o rascunho.

#### 2. Staging Area

É a caixa de envio do seu projeto. Ou seja, é um arquivo que armazena toda a informação sobre o seu próximo envio/commit antes de envia-lo de fato. 

#### 3. Git Directory

É onde é armazenado todos os metadados e banco de dados de objetos do projeto. Aqui fica guardado toda a história de versões do seu código.


> [!WARNING] Atenção 
> Nos comandos abaixo, remova os símbolos `< >` antes de digitar. Eles servem apenas para indicar onde você deve inserir sua própria variável ou texto.

### git config

Configurações iniciais para identificar quem está fazendo as mudanças no histórico.

```sh
# Define o nome que aparecerá nos seus commits
$ git config --global user.name "<seu nome>"

# Define o email atrelado aos seus commits
$ git config --global user.email "<seu email>"

# Ativa cores na saída do terminal (facilita muito a leitura)
$ git config --global color.ui auto
```

> [!TIP] Dica 
> Sem o parâmetro `--global`, a configuração valerá apenas para o repositório (pasta) atual.

### Criando e Clonando Repositórios

```sh
# Inicializa um repositório
$ git init
```

Transforma o diretório atual em um repositório Git, criando uma pasta oculta `.git` e começando a monitorar mudanças.

```sh
# Clona um repositório existente
$ git clone <url>
```

Baixa uma cópia completa de um repositório de um servidor remoto (como [[GitHub]], [[GitLab]], [[Bitbucket]] ou [[Codeberg]]). Isso inclui todos os arquivos, todo o histórico de commits e os ramos (branches).

### Fazendo Mudanças

Move as alterações do _Working Directory_ para a _Staging Area_.
```sh
# Adiciona um arquivo específico ao palco (staging)
$ git add <arquivo>

# Adiciona TODOS os arquivos modificados ao palco
$ git add .
```

Uma vez que os arquivos estão preparados (staged), você deve usar o `commit` após fazer alguma alteração:

```sh
# Salva o snapshot
$ git commit -m "<mensagem descritiva>"
```

Cria um registro permanente dos snapshots que estavam no palco.

> [!WARNING]- Boas Práticas
> Aos escrever sua mensagem do commit use o imperativo e não seja prolixo.
>
> Artigo sobre o assunto:
> https://cbea.ms/git-commit/

> [!NOTE]- Editor de Texto
> Se você rodar `git commit` sem o `-m`, você cairá no editor de texto padrão do terminal (geralmente o [[Vim]] ou Nano). Lá você pode escrever uma mensagem mais longa. 
>
>Para escrever no Vim: aperte `Esc` e depois `i`, isso vai entrar no mode de escrita.
>
> Para sair do Vim salvando: aperte `Esc`, digite `:wq` e `Enter`.
>
> para sair do Nano salvando: aperte `ctrl + s` e depois `ctrl + x` 

#### Analisando Mudanças

O Git oferece visibilidade total do estado atual e do passado do projeto.

| Comando             | Descrição                                                                                                       |
| ------------------- | --------------------------------------------------------------------------------------------------------------- |
| `git status`        | Mostra o estado atual: em qual branch você está, o que foi modificado e o que está pronto para ser comitado.    |
| `git log`           | Lista o histórico de versões, incluindo mensagem completa, autor, data e o [[Hash]] do commit.                  |
| `git log --oneline` | Versão resumida do log. Mostra apenas o hash curto e a primeira linha da mensagem.                              |
| `git diff`          | Mostra exatamente quais linhas de código mudaram nos arquivos que **ainda não** foram para o palco (`git add`). |
| `git show <commit>` | Mostra os metadados e as alterações de conteúdo de um commit específico (identificado pelo hash).               |

### Trabalhando com Branches (Ramos)

Branches são essenciais no Git. Eles permitem que você diverja da linha principal de desenvolvimento (geralmente chamada de `main` ou `master`) e continue trabalhando sem alterar o código estável.

Pense neles como "linhas do tempo paralelas". Você pode criar um ramo para testar uma ideia nova; se der errado, basta deletar o ramo e a linha principal continua intacta. Se der certo, você funde (`merge`) esse ramo de volta na linha principal.

> [!INFO]- O que é HEAD?
>  O Git usa um ponteiro especial chamado **HEAD**. Ele indica em qual branch (e consequentemente em qual commit) você está trabalhando no momento.
> 
>  Quando você troca de branch, o HEAD muda de lugar para apontar para o último commit desse novo ramo.

#### Comandos Essenciais de Branch

| Comando                  | Descrição                                                                      |
| ------------------------ | ------------------------------------------------------------------------------ |
| `git branch`             | Lista todas as branches locais. O asterisco (`*`) indica a atual.              |
| `git branch <nome>`      | Cria uma nova branch, mas **não** muda para ela automaticamente.               |
| `git checkout <nome>`    | Muda o seu diretório de trabalho (e o HEAD) para a branch especificada.        |
| `git checkout -b <nome>` | Atalho útil: **Cria** uma branch e já **muda** para ela imediatamente.         |
| `git merge <nome>`       | Funde a história da branch `<nome>` na branch em que você está **atualmente**. |
| `git branch -d <nome>`   | Deleta a branch especificada (segurança: só deleta se já tiver feito merge).   |

> [!TIP]- git switch
>  Nas versões mais recentes do Git (2.23+), foram introduzidos comandos mais semânticos para substituir o `checkout` (que fazia muitas coisas ao mesmo tempo):
> 
> - **`git switch <nome>`**: Para trocar de branch.
>     
> - **`git switch -c <nome>`**: Para criar e trocar de branch (substituto do `checkout -b`).
>     

#### Fluxo Básico de Merge

O fluxo mais comum de trabalho segue estes passos:

1. Garanta que está na branch principal: `git checkout main`.
2. Crie uma branch para uma funcionalidade: `git checkout -b feature-nova`.
3. Faça seus trabalhos e commits nessa branch.
4. Volte para a principal: `git checkout main`.
5. Traga as mudanças da funcionalidade para a principal:

```sh
# Estando na branch main:
$ git merge feature-nova
```

Isso vai pegar o histórico da `feature-nova` e aplicá-lo na `main`.

#### Conflitos

Se você alterar a **mesma linha** do **mesmo arquivo** em branches diferentes e tentar fazer o merge, o Git não saberá qual versão escolher. Isso gera um **Conflito**.

O Git pausará o merge e marcará o arquivo problemático assim:

```
<<<<<<< HEAD
Código que estava na sua branch atual (main)
=======
Código que veio da branch que está sendo fundida (feature-nova)
>>>>>>> feature-nova
```

Para resolver:

1. Edite o arquivo manualmente.
2. Escolha o código correto e apague o que não serve.
3. Remova os marcadores (`<<<<`, `====`, `>>>>`).
4. Salve o arquivo.
5. Rode `git add <arquivo>` e finalize com `git commit`.