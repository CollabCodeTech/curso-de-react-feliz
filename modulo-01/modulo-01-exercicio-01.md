## 01 - Iniciar projeto com ViteJS

### Tarefas

1. Pelo terminal, crie um projeto com o [ViteJS](https://vitejs.dev/) no Desktop (área de trabalho) do seu SO ou em outro lugar que você preferir;

### Passo a passo

#### 1. Crie pasta do projeto

Para saber como inicia um projeto com o ViteJS podemos acessar a página [get started](https://vitejs.dev/guide/#scaffolding-your-first-vite-project) para ver a documentação atualizada.

Abra o terminal do seu SO, se estiver no Windows use o Power Shell, Git BASH ou similares para que o comando do Linux funcione. Se estiver no Linux ou Mac, ambos têm comandos muitos similares. Agora que você já está com o seu terminal aberto vamos executar os seguintes passos:

Entre no Desktop com o comando a seguir:

```bash
cd ~/Desktop
```

Criar o projeto react dentro do Desktop:

```bash
yarn create vite
```

A criação do projeto é interativa, então serão feitas algumas perquntas para que você responda

A primeira pergunta é o nome do projeto, nosso projeto se chama **chatcollab**

```bash
? Project name: chatcollab
```

Depois de informar o nome do projeto é só dar **[Enter]**

A Segunda pergunta é sobre qual framework será utilizado, nos iremos utilizar o react

```bash
? Select a framework:
    vanilla
    vue
>   react
    preact
    lit
    svelte
```

Utilize as setas do teclado para navegar até a palavra react e de **[Enter]**

A próxima pergunta é sobre uma variante do framework, se você irá utilizar ReactJS _"puro"_ ou com TypeScript, no nosso caso é só dar **[Enter]** para escolher o `react`

```bash
? Select a variant:
>   react
    react-ts
```

Com isso já temos nosso projeto criado e a informação final no terminal é parecida com a que está sendo mostrada a baixo:

```bash
Scaffolding project in /app/chatcollab...

Done. Now run:

  cd chatcollab
  yarn
  yarn dev

Done in 8.88s.
```

Como nos orienta vamos acessar a pasta do projeto e rodar o comando `yarn` para instalar as dependências do projeto e depois o comando `yarn dev` para iniciar o projeto.

Acessar a pasta **chatcollab**:

```bash
~/Desktop/$ cd chatcollab
```

> Caso queira ver os arquivo de uma forma mais elegante é só rodar o comando `code .` para abrir o Visual Code com os arquivos do nosso projeto.

Instalar as dependências:

```bash
~/Desktop/chatcollab$ yarn
```

> Nesta etapa vemos que o ViteJS é mais rápido para baixar as dependencias do projeto em relação ao [Create React App](https://create-react-app.dev/)

```bash
yarn install v1.22.17
info No lockfile found.
[1/4] Resolving packages...
[2/4] Fetching packages...
[3/4] Linking dependencies...
[4/4] Building fresh packages...
success Saved lockfile.
Done in 14.56s.
~/Desktop/chatcollab$ yarn dev
```

A saida do último comando é exibida a baixo e no informa o endereço e porta que nosso projeto está rodando

```bash

  vite v2.8.6 dev server running at:

  > Local: http://localhost:3000/
  > Network: use `--host` to expose

  ready in 472ms.
```
