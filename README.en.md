<p align="right">
  <a href="README.en.md">🇺🇸</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="README.md">🇧🇷</a>&nbsp;&nbsp;&nbsp;
</p>

<img alt="GoStack" src=./src/assets/header-bootcamp.png />

<h3 align="center">
  Challenge 07: GoFinances Web
</h3>

<p align="center">
  <a href="#rocket-about-the-application">About the application</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#cd-installed-packages">Installed packages</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#memo-licence">Licence</a>
</p>

<img alt="Gofinances" src=./src/assets/gofinances.gif />

## :rocket: About the application

A transaction management application, GoFinances, in React.js along with TypeScript, using routes and sending files by form.

This is an application that connects to [Database Upload](https://github.com/bruno-fialho/desafio-database-upload) backend, and displays the transactions created and allows the import of a CSV file to generate new ones records in the database.

### Application Template

The template is available in the following URL: **[Access Template](https://github.com/Rocketseat/gostack-template-fundamentos-reactjs)**

**Tip**: In case you don't know how to use Github repositories as templates, we have a guide in **[Rocketseat FAQ](https://github.com/Rocketseat/bootcamp-gostack-desafios/tree/master/faq-desafios).**

Navigate to the created folder and open it in the Visual Studio Code, remember to execute the command `yarn` in your terminal in order to install all the dependencies

### Preparing the backend

First of all, for the frontend to connect correctly to the backend, in the `backend` folder you must execute the commands `yarn add cors` and then `yarn add @types/cors -D`.

After that in the `app.ts` file still on the backend, import `cors` and add `app.use (cors ())` before the line containing `app.use (routes)`.

### Application features

The application has the following features:

- **`List your API transactions`**: Your `Dashboard` page is able to display a listing through a table, with the field `title`, `value`, `type` and `category` of all transactions that are registered in your API.

- **`Display your API balance`**: Your `Dashboard` page displays the balance that is returned from your backend, containing the grand total, along with the total of entries and exits.

- **`Import CSV files`**: On your `Import` page, allows sending a file in `csv` format to your backend, which will import transactions into your database. The csv file must follow the following [template](https://github.com/Rocketseat/bootcamp-gostack-desafios/blob/master/desafio-database-upload/assets/file.csv).

### Specification of tests

In each test, you have a brief description of what your application must do in order for the test suits pass.

If you have questions about what the tests are, and how to interpret them, take a look at **[Rocketseat FAQ](https://github.com/Rocketseat/bootcamp-gostack-desafios/tree/master/faq-challenges).**

For this challenge we have the following tests:

- **`should be able to list the total balance inside the cards`**: In order for this test to pass, your application must allow cards containing the total of `income`, `outcome` and the total subtraction of `income - outcome` to be displayed on your backend `balance`.

* **`should be able to list the transactions`**: For this test to pass, your application must allow all transactions that are returned from your backend to be listed within a table.

- **`should be able to navigate to the import page`**: In order for this test to pass, you must allow the page exchange through the Header, by the button that contains the name `Importar`.

- **`should be able to upload a file`**: For this test to pass, you must allow a file to be sent via the drag-n-drop component on the `import` page, and it is possible to display the name of the file sent to the input.

## :cd: Installed packages

The following is a list of installed packages:

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

	Optional
- [eslint](https://eslint.org/)
- [prettier](https://prettier.io/)
- [eslint-import-resolver-typescript](https://github.com/alexgorbatchev/eslint-import-resolver-typescript#readme)
- [eslint-plugin-jsx-a11y](https://github.com/evcohen/eslint-plugin-jsx-a11y#readme)
-[eslint-plugin-react](https://github.com/yannickcr/eslint-plugin-react)

## :memo: Licence

This project is under license from MIT. See the archive [LICENSE](LICENSE) to more details.
