# Week 7 Summary

## Fix Template Repo to Include `.vscode` Directory
* `.vscode` was ignored; it was listed in the `.gitignore` file, meaning it wasn't pushed to GitHub. Delete `.vscode` from the file so it can be pushed to GitHub.

## Re-Examining Last Week's Code
* **Semicolons `;`:** They are optional in JavaScript, but are recommended. Semicolons mark the end of a statement in code; it is the end of a complete statement and tells the compiler that the next characters are part of a new statement.
  * Extensions like ESLint and Prettier will automatically add semicolons if they're not present.
* **Returns:** The `return` statement marks the end of a block of code.
  * Blocks of code refer to chunks of code within a set of brackets; these encased statements form a function or other complex method.
  * The `return` statement can also tell the function what to return to the caller. The arguments entered after the keyword are sent back to the caller and will typically change the value of a variable.
* **`const`**: This keyword is used to create a variable that can hold data for later use.
  * To declare a new variable in JavaScript, write `const` followed by the variable's name. In last week's code, `sum` is a variable declared using the statement `const sum`.
  * This keyword is once again optional, but it is highly recommended that you write `const` when declaring variables.

## _Eloquent JavaScript_ Example Code
* The keyword `let` is similar to `const`. Both are used to declare variables; however, a variable declared with `const` can only be assigned a value once while `let` variables can be manipulated an infinite amount of times.
* `while` is used to initiate a conditional loop. As long as the condition in parentheses is met, the loop will repeat. Once the condition is no longer true, the loop will break after the last iteration and the compiler will continue running through the code.
  * In many `while` loops, the variable/value in the condition will be manipulated after each iteration and will eventually break the condition. This is the case in _Eloquent JavaScript_'s code; the variable `count` is increased by one each loop until the
    value is greater than 10.

## _Eloquent JavaScript_ Chapter 1: Values, Types, and Operators
* _Values_ play an important role in separating data. In JavaScript, values are separated by creating separate variables to hold information.
* Many data types can be represented using variables:
  * **Numbers:** Computers can hold over 18 quintillion whole numbers and a large amount of fractions. While fraction operations are not guaranteed to be precise, the result is good enough for most situations.
  * **Strings:** Strings are used to represent text. While using just letters and spaces is pretty simple (just enclose them in quotes), using special characters such as 'newline' and 'tab' can be difficult. An escape character must be used to add those characters into a string. In JavaScript, this is the backslash (`\`). For example, adding a newline character to a string is done using "\n".
    * Similar to how numbers can be combined, strings can be concatenated. By using the + operator, two different strings will be combined. For example, "Hello World!" can be concatenated with `"Hello " + "World!"`.
  * **Boolean Values:** These are quite simple compared to numbers and strings. Boolean values have only two possibilities, similar to a binary switch. These can be interpreted as "yes/no", "true/false", or "on/off", but they all serve the same purpose.
    * Logical operators can be used to manipulate boolean values. JavaScript provides several: `&&` requires two true values ("and"), and `||` only needs one true value ("or"). The exclamation mark (!) flips the value from true to false and vice versa ("not").
    * There is even a _ternary_ operator which can accept three values. Written with a question mark and colon, it can look like this: `true ? 1 : 2`. The first value picks one of the other two based on its condition; in this instance, `true` values pick 1
      while `false` values will pick 2.
  * **Empty Values:** Some values don't contain any information. In JavaScript, the words `null` and `undefined` are used to indicate empty values. The two words are interchangeable most times.

## Strings
* Strings can be declared using double quotes (""), single quotes (''), and backticks (``). Be consistent with your string punctuation.
  * Double quotes are the best when punctuation is featured in the string.
  * Backticks are easiest when using template literals. These special places in strings can be filled with other variables using a dollar sign "$" and encasing the variable name in curly brackets "{}".
    * It's possible to use template literals without needing backticks. However, you will need to use + operators to concatenate the strings.

## Numbers, Booleans, Comparisons, `const` and `let`
* Declaring variables that hold number values is pretty straightforward in JavaScript. Simply add the number on the right side of a `const` declaration statement and you're set.
* Booleans represent true or false. These can be declared using one of these words, but do not encase them in quotations or JavaScript will interpret them as strings.
  * They are typically used in comparisons. By using a condition on the right side of the declaration statement, the boolean will be assigned a true/false value based on that condition's outcome.
* Strings, numbers, and booleans are all considered _primitive_ data types. They represent one individual piece of data; in other words, they are discrete pieces of data.
* The keyword `const` is commonly used when declaring primitive data types. In these cases, "const" is short for "constant"; the variable's value cannot be altered once initially assigned.
  * When dealing with other variable types, `const` serves as a constant _reference_ as opposed to a constant _value_. 
* The keyword `let` allows for the values in variables to change.

# Reflections
* I see many similarities between JavaScript and other object-oriented languages like C#. Some of the major differences have been the variable keywords (using `const` and `let` instead of `int`, `string`, and `bool`) and how strict the languages are
  (vanilla JavaScript is pretty flexible while C# has a more rigid structure). I'm looking forward to seeing how JavaScript is used in a web development environment and how its logic interacts with HTML and CSS, which are structured **very** differently.
* I think this will be the most exciting part of CIS-177 for me. Going back to my previous point, JavaScript strongly resembles languages I've used in the past so I'm hoping it will come pretty easy for me. I've done a little research on JavaScript
  applications and the language is everywhere in the development sphere.
