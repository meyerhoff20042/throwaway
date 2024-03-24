# Object Literals in JavaScript

### Creating Objects
```javascript
/**
 * Objects in JavaScript can have many different properties. These properties can be named and defined
in the same statement as the object itself, as shown below.
 */
const book = {
  title: "To Kill a Mockingbird",
  pubYear: 1960,
  genre: "coming-of-age",
  synopsis:
    "A poignant tale set in the racially-charged atmosphere of 1930s Alabama, following young Scout Finch's
    coming-of-age journey as she learns about empathy, injustice, and the complexities
    of human nature through her father's defense of a black man falsely accused of rape.",
};
```

The object is named "book" and its properties help identify it. The title, genre, and synopsis properties are all strings, and the pubYear property is an integer.

### Referencing Object Properties
```javascript
const book = {
  title: "To Kill a Mockingbird",
  pubYear: 1960,
  genre: "coming-of-age",
  synopsis:
    "A poignant tale set in the racially-charged atmosphere of 1930s Alabama, following young Scout Finch's
    coming-of-age journey as she learns about empathy, injustice, and the complexities
    of human nature through her father's defense of a black man falsely accused of rape.",
};

console.log(book["title"]);  // To Kill a Mockingbird
console.log(book.genre);     // coming-of-age
```

There are two ways to reference specific properties in objects: bracket notation and dot notation. Bracket location uses brackets and quotation marks to specify
the property (`book["title"]`), while dot notation only uses a single dot (`book.genre`).

### Potentially Confusing Concepts
#### Empty Values
JavaScript is a loosely typed language, meaning there are fewer restrictions on how you can write code. This can result in several terms that may seem unclear,
including `undefined`, `null`, and `not defined`. Let's clear this up. `undefined` results from using an unassigned value. For example, the statement `let x`
creates a variable `x`; however, no value is assigned to it, leaving it vacant.

The words `not defined` will show up when the program attempts to reference a nonexistent variable. Since the variable itself is missing, there is no value either.

While `undefined` is a placeholder for an unassigned variable, `null` is when a variable is intentionally left vacant. This doesn't have many practical uses, and
cannot be used with the `const` keyword.

#### What does `const` truly mean?
The keyword `const` is used when declaring a variable. The name implies that it's short for "constant"; however, this isn't necessarily the case. While this is true
for most situations involving simple variables, collection types such as arrays can still be manipulated even when declared with the `const` keyword. This can be seen
here:
```javascript
const toDoList = ["Clean Room", "Wash Clothes", "File Taxes", "Finish Homework"]
console.log(toDoList[0]);    // Clean Room

toDoList[0] = "Clean Litter Box";
console.log(toDoList[0]);    // Clean Litter Box
```

This example shows my to-do list for the upcoming days. When I finished cleaning my room I switched the first index from "Clean Room" to "Clean Litter Box". I was able
to do this despite declaring the array with the `const` keyword.

### Reflections
* I'm thrilled to work with objects and arrays as they are some of my favorite parts of programming. Being able to create unique objects and define their characteristics
  is a concept I have used in many of my projects, whether it's creating coins, phones, shapes, or vehicles. I'm glad to see JavaScript has many of these same features and
  they seem similar to how languages like C# and Python use objects.
* I am curious as to why using the `const` keyword creates a constant in every use besides arrays. It seems strange that it means constant in all cases except one.
