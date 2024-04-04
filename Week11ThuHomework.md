# Video Code Walkthrough Comparison

Your walkthrough was pretty different from mine. In your `for` loop, you created a variable for the person and applied the `verifyAdulthood` function inside the `console.log` statement.
In mine, I created a variable for the message and then displayed it with a `console.log` statement.
In our functions, I didn't read the directions about not changing the original code and modified the function to only take the person object as opposed to name and age parameters.

# _Eloquent JavaScript_ Chapter 4 Notes

* Objects allow us to group several of the primitive data types to form more complex objects.

### Data Sets
* _Data sets_ allow us to store sequences of values in data types called **arrays**. When declaring an array, you use square brackets `[]` to surround a list of values separated by commas.
* When referencing a specific value inside an array, you use square brackets again to denote the index of that value (`listOfNumbers[2]` returns the third element in that sequence).

### Properties
* We can access properties of objects in two ways:
  * Using a dot after the object name (`value.x`)
  * Using square brackets (`value[x]`)
* The two methods differ slightly; using a dot calls the literal name of the property (characters to the right of the dot are assumed to be a string).
  When using square brackets, JavaScript will convert the characters on the right to a string and use that as a property name. This means that property names with spaces or that are numbers
  will require the use of square brackets.
* A common example of a property is the `length` property of an array. This returns the number of elements inside the array.

### Methods
* Some properties hold function values, like the `toUpperCase()` method for a string. In this instance, it will convert all characters in the string to uppercase.
* Properties that contain functions are called *methods* of the value they belong to.
* Arrays have `push` and `pop` methods for adding and removing values. They operate on a *stack*, meaning that popping a value out will remove the most recently added value.

### Objects
* Objects are collections of properties. They can hold many properties of different data types and can be used to create complex variables with characteristics.
* The book uses a "weresquirrel" as an example. For a daily log program, an object called `day1` is created which holds `squirrel` and `events` values.
  * `squirrel` is a boolean that will show whether or not the user became a squirrel that day.
  * `events` is an array of strings that list the user's activities that day.
* Objects' properties can be read individually. If you try to read a property that doesn't exist, JavaScript will return `undefined`.

### Mutability
* Primitive data types discussed earlier are *immutable*, meaning they cannot be changed once assigned. However, the properties of objects can be changed.
* Objects whose bindings grasp the same object will change in unison. Objects initially assigned to another object's binding will share the same value until the first object's value is changed.

### The Lycanthrope's Log
* Jacques the Weresquirrel creates a log to record his daily activities and track if he became a squirrel that day. The `squirrel` and `events` values are part of the `journal` object.
* After logging several days, Jacques checks if eating pizza is leading to the squirrelifications. After doing some complex correlation calculations, he determined that eating pizza had little impact on his squirrel problem.

## Reflections
* I've used objects several times in my coding career. However, this will be my first time creating objects with properties within the main program. In C#, objects with properties are typically
  created using separate class (.cs) files, as you only have access to the simple data types in the main program.
* It took me a minute to understand the difference between accessing properties using a period vs. square brackets, but I think I understand the difference now.
* This is the first language I've seen where constants are used frequently. In C#, Java, and Python, most of the variables we create are changed frequently so the program can take new information.
  Is it normal for JavaScript to use a lot of constants, or is that just for simplicity right now?
