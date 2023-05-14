---
title: "Tutorial Git"
description: "Tutorial para aprender os conceitos básicos de como usar o Git."
pubDate: "May 3 2023"
heroImage: "/git.png"
---

Neste tutorial, vamos cobrir os seguintes tópicos:

- O que é Git
- Instalação do Git
- Configuração do Git
- Comandos básicos do Git
- Trabalhando com Branches
- Trabalhando com repositórios remotos
- Resolução de conflitos
- Trabalhando com Tags

### O que é Git

Git é um sistema de controle de versão distribuído, ou seja, ele permite que várias pessoas trabalhem em um projeto simultaneamente, sem que precisem estar na mesma rede ou servidor. Cada usuário tem uma cópia do repositório completo em sua máquina local, e as alterações são compartilhadas por meio de "pushes" e "pulls" entre as máquinas.

### Instalação do Git
Antes de começar, você precisa instalar o Git em sua máquina. Você pode baixá-lo em https://git-scm.com/downloads e seguir as instruções para instalar em seu sistema operacional.

### Configuração do Git

Antes de começar a usar o Git, é importante configurar algumas informações básicas, como seu nome e endereço de e-mail. Para isso, use os seguintes comandos:

```
git config --global user.name "Seu Nome"
```
```
 git config --global user.email "seuemail@email.com"`
```

### Comandos básicos do Git

Algumas das operações básicas do Git são:

- `git init`: Cria um novo repositório local.
- `git add`: Adiciona arquivos ao índice (staging area) para serem commitados.
- `git commit`: Salva as alterações no repositório com uma mensagem de commit.
- `git status`: Mostra o status atual do repositório.
- `git log`: Mostra o histórico de commits.
- `git diff`: Mostra as diferenças entre arquivos.
- `git branch`: Mostra as branches disponíveis.
- `git checkout`: Troca para uma branch específica.


### Trabalhando com Branches

Branches são ramificações do projeto principal, que permitem trabalhar em diferentes recursos sem interferir no código principal. Algumas operações básicas com branches são:

- `git branch nome_branch`: Cria uma nova branch.
- `git checkout nome_branch`: Troca para a branch específica.
- `git merge nome_branch`: Mescla as alterações de uma branch em outra.
- `git branch -d nome_branch`: Deleta uma branch específica.

### Resolução de conflitos

Quando duas pessoas fazem alterações no mesmo arquivo ao mesmo tempo, pode ocorrer um conflito. Para resolvê-lo, é preciso abrir o arquivo em questão, editar manualmente as partes conflitantes e escolher qual versão será mantida. Depois de resolver os conflitos, é preciso commitar as alterações.

### Trabalhando com repositórios remotos

Para trabalhar em equipe, é comum usar repositórios remotos. Algumas das operações mais comuns são:

- `git remote add nome_repositorio URL_repositorio`: Adiciona um repositório remoto.
- `git clone URL_repositorio`: Clona um repositório remoto para sua máquina local.
- `git push nome_repositorio nome_branch`: Envia as alterações locais para o repositório remoto.
- `git pull nome_repositorio nome_branch`: Obtém as alterações mais recentes do repositório remoto.

### Trabalhando com Tags

As tags são pontos de referência específicos em um histórico de commits. Elas são usadas para marcar versões estáveis, lançamentos ou pontos importantes no desenvolvimento do projeto. Algumas operações com tags são:

- `git tag nome_tag`: Cria uma nova tag no commit atual.
- `git tag -a nome_tag -m "Mensagem da tag"`: Cria uma nova tag anotada com uma mensagem.
- `git tag`: Lista todas as tags existentes.
- `git show nome_tag`: Mostra informações sobre uma tag específica.
- `git push nome_repositorio nome_tag`: Envia uma tag específica para o repositório remoto.
- `git push nome_repositorio --tags`: Envia todas as tags para o repositório remoto.

