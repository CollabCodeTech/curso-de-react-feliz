## 08 Para saber mais Módulo 01

### 08.1 Porque o ViteJS é melhor que o CRA

A [documentação do ViteJS](https://vitejs.dev/guide/why.html#slow-server-start) já nos dá uma boa referência disso

#### Pontos positivos

- Ele já utiliza o Rollup que é um pouco mais rápido que o webpack para fazer o build.
- Em ambiente de desenvolvimento ele não utilizar o Rollup e sim o ESBuild que é muito mais performatica e junto com o conceito de módulo import e export do próprio navegador

> Com isso ao invés do Rollup ter que fazer todo o build da aplicação ao modificar um arquivo, ele faz o processo inverso, ou seja, ele faz o processo e build do arquivo modificado e todos os arquivos que são referenciados por ele anteriormente, não tendo que reprocessar os outros arquivos, tornando o processo muito mais rápido.

Quando temos um projeto pequeno está _diferença_ não é tão notada, mas quando o projeto cresce e fica grande, com muitas implementações em React faz muita diferença, por isso antes do ViteJS muitas empresas implementavam o React sem o uso do CRA

#### Pontos negativos

- Toda a configuração tem que ser feita na _mão_ no arquivo vite.config.js, então algumas tarefas como configurar o `Jest` é mais complicado em relação ao CRA que já vem configurado.

Caso você queira utilizar a o `Jest` ou outras ferramentas pode acessar o [ViteJS awesome](https://github.com/vitejs/awesome-vite) que tem vários pacotinhos com templates já prontos e configurados para você utilizar como por exemplo:

- [vite-react-express-boilerplate](https://github.com/joeynguyen/vite-react-express-boilerplate) - Full-Stack template with React and Express.
- [vite-react-tailwind-template](https://github.com/Innei/vite-react-tailwind-template) - React 17, TypeScript, Jest, ESLint, Prettier, Husky, Tailwind CSS, PostCSS, pnpm.

Entre outros pacotinhos felizes.
