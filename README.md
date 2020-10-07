<p align="right">
  <a href="README.en.md">🇺🇸</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="README.md">🇧🇷</a>&nbsp;&nbsp;&nbsp;
</p>

<img alt="GoStack" src=./src/assets/header-bootcamp.png />

<h3 align="center">
  Desafio 07: GoFinances Web
</h3>

<p align="center">
  <a href="#rocket-sobre-a-aplicação">Sobre a aplicação</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#cd-pacotes-instalados">Pacotes instalados</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#memo-licença">Licença</a>
</p>

<img alt="Gofinances" src=./src/assets/gofinances.gif />

## :rocket: Sobre a aplicação

Uma aplicação de gestão de transações, a GoFinances, no React.js junto com TypeScript, utilizando rotas e envio de arquivos por formulário.

Essa é uma aplicação que se conectaa ao backend do [Database Upload](https://github.com/bruno-fialho/desafio-database-upload), e exibe as transações criadas e permite a importação de um arquivo CSV para gerar novos registros no banco de dados.


### Template da aplicação

O template está disponível na seguinte url: **[Acessar Template](https://github.com/Rocketseat/gostack-template-fundamentos-reactjs)**

**Dica**: Caso não saiba utilizar repositórios do Github como template, temos um guia em **[FAQ da Rocketseat](https://github.com/Rocketseat/bootcamp-gostack-desafios/tree/master/faq-desafios).**

Agora navegue até a pasta criada e abra no Visual Studio Code, lembre-se de executar o comando `yarn` no seu terminal para instalar todas as dependências.

### Preparando o backend

Antes de tudo, para que o frontend se conecte corretamente ao backend, na pasta do `backend` deve executar os comandos `yarn add cors` e depois `yarn add @types/cors -D`.

Depois disso no arquivo `app.ts` ainda no backend, importe o `cors` e adicione `app.use(cors())` antes da linha que contém `app.use(routes)`.

### Funcionalidades da aplicação

A aplicação tem as seguintes funcionalidades:

- **`Listar as transações da sua API`**: Sua página `Dashboard` é capaz de exibir uma listagem através de uma tabela, com o campo `title`, `value`, `type` e `category` de todas as transações que estão cadastradas na sua API.

- **`Exibir o balance da sua API`**: Sua página `Dashboard` exibe o balance que é retornado do seu backend, contendo o total geral, junto ao total de entradas e saídas.

- **`Importar arquivos CSV`**: Na sua página `Import`, permite o envio de um arquivo no formato `csv` para o seu backend, que irá fazer a importação das transações para o seu banco de dados. O arquivo csv deve seguir o seguinte [modelo](https://github.com/Rocketseat/bootcamp-gostack-desafios/blob/master/desafio-database-upload/assets/file.csv).

### Especificação dos testes

Em cada teste, tem uma breve descrição no que sua aplicação deve cumprir para que o teste passe.

Caso você tenha dúvidas quanto ao que são os testes, e como interpretá-los, dé uma olhada no **[FAQ da Rocketseat](https://github.com/Rocketseat/bootcamp-gostack-desafios/tree/master/faq-desafios).**

Para esse desafio, temos os seguintes testes:

- **`should be able to list the total balance inside the cards`**: Para que esse teste passe, sua aplicação deve permitir que seja exibido na sua Dashboard, cards contendo o total de `income`, `outcome` e o total da subtração de `income - outcome` que são retornados pelo `balance` do seu backend.

* **`should be able to list the transactions`**: Para que esse teste passe, sua aplicação deve permitir que sejam listados dentro de uma tabela, toda as transações que são retornadas do seu backend.

- **`should be able to navigate to the import page`**: Para que esse teste passe, você deve permitir a troca de página através do Header, pelo botão que contém o nome `Importar`.

- **`should be able to upload a file`**: Para que esse teste passe, você deve permitir que um arquivo seja enviado através do componente de drag-n-drop na página de `import`, e que seja possível exibir o nome do arquivo enviado para o input.

## :cd: Pacotes instalados

A seguir segue uma lista dos pacotes instalados:

- [react](https://reactjs.org/)
- [react-scripts](https://github.com/facebook/create-react-app#readme)
- [react-dropzone](https://github.com/react-dropzone/react-dropzone)
- [react-router-dom](https://github.com/ReactTraining/react-router#readme)
- [typescript](https://www.typescriptlang.org/)
- [ts-jest](https://kulshekhar.github.io/ts-jest)
- [axios](https://github.com/axios/axios)
- [filesize](https://filesizejs.com/)
- [history](https://github.com/ReactTraining/history#readme)
- [polished](https://polished.js.org/)
- [styled-components](https://styled-components.com/)

	Opcional
- [eslint](https://eslint.org/)
- [prettier](https://prettier.io/)
- [eslint-import-resolver-typescript](https://github.com/alexgorbatchev/eslint-import-resolver-typescript#readme)
- [eslint-plugin-jsx-a11y](https://github.com/evcohen/eslint-plugin-jsx-a11y#readme)
-[eslint-plugin-react](https://github.com/yannickcr/eslint-plugin-react)

## :memo: Licença

Esse projeto está sob a licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.
