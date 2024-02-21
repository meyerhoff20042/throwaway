# Creating a NodeJS Template Repo

* Open the terminal and navigate to the directory which will contain your files.
* Create a directory for your node template. Make a new .vscode directory within the first directory, which will include `settings.json` and `extensions.json` files.
  * Use the `touch` command to create the two _.json_ files.
  * The contents of the files are pretty self-explanatory. `extensions.json` will contain VSCode extensions needed for your project, and `settings.json` will contain settings that affect your project.
    * **_THESE FILES ARE ESSENTIAL IN CREATING THE NODEJS TEMPLATE REPO!_**
* Open your project in Visual Studio Code.
* Make sure to download either Node.js (Windows) or Homebrew (Mac/Linux) to use NPM (node package manager). Initialize the NPM with `npm init --yes`.
  * NPM uses a new file called `package.json`. This file allows you to install and use NPM.
  * Initialize ESLint with the command `npm init @eslint/config`. Answer the questions from your terminal to finish the setup process.
    * Initializing ESLint will install many packages onto your computer. A _node_modules_ directory will be created in your working files, along with a JavaScript file named `.eslintrc.js`.
    * Your `package.json` file will also be updated with ESLint information.
* Install "Prettier" using the command `npm install --save-dev --save-exact prettier`.
  * Prettier works with ESLint and does extra formatting on top of ESLint's standardization.
  * A `.prettierrc` file will be added to your working files. It is empty by default.
    * You can add a `.prettierignore` file to tell Prettier what code you want the extension to ignore.
  * Use the command `npm install --save-dev eslint-config-prettier` to configure Prettier with ESLint. Then add "prettier" to the `.eslintrc.js` file in "extends".
* Change the extension on `.eslintrc.js` from "_.js_" to "_.cjs_" to remove a VSCode error asking you to update the file's contents to the ECMAScript standard.
  * Make sure the values listed in "extends" are in brackets to comply with the _.cjs_ specifications.
* Create a `.gitignore` file in your project for Git to ignore the _node_modules_ directory. You can use AI to generate the code for the file.
* Commit the files on the terminal, then push them to the GitHub repository.
