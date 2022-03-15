## 07 - Envia projeto pro Github

Vamos entrar no [github](https://github.com/) e criar o repositório para nosso projeto

### Tarefas

1. Criar o projeto no Github;
2. Envia projeto pro Github;

### Passo a passo

#### 1. Envia projeto pro Github

Primeiro vamos criar um repositório `ambiente-react` e depois vamos copiar a url do repositório. No nosso caso é `git@github.com:marcobrunodev/ambiente-react.git`

#### 2. Envia projeto pro Github

```bash
~/Desktop/chatcollab$ git remote add origin git@github.com:marcobrunodev/ambiente-react.git
~/Desktop/chatcollab$ git push
fatal: The current branch main has no upstream branch.
To push the current branch and set the remote as upstream, use

	git push --set-upstream origin main

```

> Como é nosso primeiro commit temos que dar o comando `git push --set-upstream origin main` mas podemos dar o comando reduzido, `git push -u origin main`

```bash
~/Desktop/chatcollab$ git push -u origin main
```

Agora nosso repositório já está no github.
