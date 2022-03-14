## 06 - Adiciona Gitmoji

Uma ferramenta que vai te ajudar no momento que escrever seu commit, é muito importante que quando mais de uma pessoa trabalha no projeto sigamos um padrão de commit.

O padrão que eu gosto muito é o [GitMoji](https://gitmoji.dev/) ele não é o unico do mercado.

Para cada tipo de commit temos um emoji, podemos fazer isso de forma manual, mas vamos instalar ele para poder nos ajudar.

### Tarefas

1. Adiciona Gitmoji;
2. Configurar no Husky

### Passo a passo

#### 1. Adiciona Gitmoji

Acessar o terminal do seu SO e rodar o comando confome o site do [projeto no github](https://github.com/carloscuesta/gitmoji)

```bash
~/Desktop/chatcollab$ npm i -g gitmoji-cli
```

#### 2. Configurar no Husky

No terminal é só executar o comando conforme exibido a baixo.

```bash
~/Desktop/chatcollab$ gitmoji -i
```

Ele já cria o arquivo de configuração no nosso Husky, agora vamos ver ele funcionando.

```bash
~/Desktop/chatcollab$ git status
On branch main

Untrack files:
        .husky/prepare-commit-msg

~/Desktop/chatcollab$ git add .

~/Desktop/chatcollab$ git status
On branch main

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   .husky/prepare-commit-msg

~/Desktop/chatcollab$ git commit

```

> Agora não passamos o parametro `-m` como anteriormente.

Agora vemos o git chamando o GitMoji com a lista de emoji e uma pequena descrição, podemos fazer também filtro digitando um termo, que será usado como pesquisa para a descrição do emoji.

Ao selecionar o emoji ele solicita o título do commit e aconselha ter somente 48 caracteres, já se acostume a criar o texto do commit em inglês e no infinitivo, que as maiorias das empresas adotam este padrão.

Ele irá solicitar também uma mensagem, para quando as informações no título não sejam suficientes para descrever o commit, pensando nos 48 caracteres, caso você não queira colocar nada na mensagem é só digitar **#** _*(hashtag)*_ e dar enter.

Ao termino disso ele vai abrir o texto do commit em seu editor padrão do commit, podendo ser o vim, o nano ou outros que você tenha configurado.
