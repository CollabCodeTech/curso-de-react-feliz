## 04 - Pasta .vscode para um mundo dev mais feliz

### Tarefas

1. Criar a pasta `.vscode`;
2. Criar o `settings.json` dentro de `.vscode`;
3. Configuração inicial do `settings.json`;
4. Adicionar os plugins do `ESLint` e `Prettier` no `.vscode`

### Passo a passo

#### 1. Criar a pasta .vscode

Abra o terminal do seu SO, se estiver no Windows use o Power Shell, Git BASH ou similares para que o comando do Linux funcione. Se estiver no Linux ou Mac, ambos têm comandos muitos similares. Agora que você já está com o seu terminal aberto vamos executar os seguintes passos:

Entre no Desktop com o comando a seguir:

```bash
cd ~/Desktop
```

Acessar a pasta **chatcollab**:

```bash
~/Desktop$ cd chatcollab
```

Criar a pasta **.vscode** e acessar a pasta:

```bash
~/Desktop/chatcollab$ mkdir .vscode
~/Desktop/chatcollab$ cd .vscode
```

#### 2. Criar o settings.json dentro de .vscode

Criar o arquivo **settings.json**:

```bash
~/Desktop/chatcollab/.vscode$ touch settings.json
```

#### 3. Configuração inicial do `settings.json`;

Quando você digitar `(Ctrl + ,)` para abrir a tela de Configurações do Visual Studio Code e você clicar ![abrir configuração JSON](img/ico-config-json-vscode.png) você vé o arquivo `settings.json` do Visual Studio Code. Não temos porque salvar toda a configuração no nosso projeto, mas a configuração a baixo que faz parte da configuração do `Prettier`

```JSON
...

    "editor.formatOnSave": true,
    "[javascriptreact]": {
        "editor.defaultFormatter": "esbenp.prettier-vscode"
    }
...
```

Então vamos abrir o arquivo `settings.json` no Visual Studio Code e colocar o conteúdo abaixo.

```JSON
{
    "editor.formatOnSave": true,
    "[javascriptreact]": {
        "editor.defaultFormatter": "esbenp.prettier-vscode"
    }
}
```

Também é bom colocar o nosso padrão para o _`[TAB]`_ fazendo a alteração o arquivo fica assim:

```JSON
{
    "editor.formatOnSave": true,
    "[javascriptreact]": {
        "editor.defaultFormatter": "esbenp.prettier-vscode"
    },
    "editor.tabSize": 2,
}
```

#### 4. Adicionar os plugins do ESLint e Prettier no .vscode

Para adicionar os plugins como recomendação para os próximos desenvolvedores é de uma forma mais visual e feliz.

Para informar os plugins necessários também acompanharem o projeto é só irmos em cada Plugin clicar na engrenagem (![engrenagem](img/ico-settings.png)) e depois em na ultima opção `Add to Workspace Recommendations` e depois disso será criado dentro da pasta `.vscode` o arquivo `extensions.json`

Depois de efetuar isso o arquivo `extensions.json` ficara conforme a baixo:

```JSON
{
  "recommendations": [
    "esbenp.prettier-vscode",
    "dbaeumer.vscode-eslint"
  ]
}
```
