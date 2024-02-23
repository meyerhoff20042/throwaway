# Introduction to JavaScript

### Node Template Starting Files

* Files required in the Node Template include `extensions.json` and `settings.json`.
* A configuration file named `.eslintrc.cjs` is also included in the project files. This file has several examples of JavaScript datatypes:
  * String: "airbnb-base" and "prettier" are strings, a phrase that is stored in a variable.
  * Collection: A group of related variables; for example, the two strings mentioned above are in the same collection labeled "extends". Collections are surrounded with square brackets "[]".
* `package.json` lists extensions used in the project, such as ESLint. These are added using commands such as `npm install`.

### `index.js` and JavaScript terms

* JavaScript terms used in this file include:
  * **Function:** Written with the `function` keyword, followed by the function's name (i.e. `addNumbers`). After this are the parameters involved with the function in parentheses `(num1, num2)`.
    * Function names use camelCase. The first word is lowercase, and every subsequent word begins with a capital letter.
    * After the function name and parameters are defined, within curly brackets "{}" will be the nested code within the function. Most functions will end with a `return` statement.
    * Functions are called by name and the arguments are passed using parentheses, in the same order that they will be used in the function. For example, `addNumbers` has two parameters, `num1` and `num2`. To pass arguments into these
      parameters, we must order them the same way. To pass 5 into `num1` and 10 into `num2` would look like this: `const sum = addNumbers(5, 10);`.
        * This line of code creates a variable called `sum`. Given the two arguments, this variable will hold the return value of the `addNumbers` function. In this case, `sum` is equal to 15.
  * **Variable:** Variables are a placeholder for many things; they can represent numbers, words, phrases, boolean values, and other characters. In this instance, the variable `sum` will hold the output of the `addNumbers` function.
    * To create a variable, you must declare a variable type (in this case `const`) and then provide the name. To assign a value to this variable, add an equals sign then write the code that will determine its value.
  * **Print:** Printing in JavaScript is done using `console.log` followed by the desired output in parentheses and quotation marks. To print the sum of `addNumbers` onto the terminal, we use `console.log("The sum is:", sum);`.
    * After running this line of code, the console will show "The sum is: 15".
    * *_Note: When referencing variables in `console.log` statements, do not put the variable name in quotations._*
   
## Reflections

* I think JavaScript will be fun to use in my web development career. It seems similar in design to C# and Python, two languages that I've taken classes on and (in the case of C#) used extensively. With this experience,
  I'm hoping JavaScript will be easier for me to learn than CSS has been.
* I'm also interested to see how JavaScript affects a website's presentation. From the example shown in the videos we only saw the addition of two numbers and the sum printed on the terminal. I'm curious to see what more complex JavaScript
  looks like in the context of web design, and if functions and variables are used in the same manner.
