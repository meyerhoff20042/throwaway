# Summary

## Translating to Binary
* ASCII (American Standard Code for Information Interchange) is a 7-bit binary system. You can send 128 values over the wire using ASCII.
  * Instead of allowing only numbers to be converted, different letters and characters were assigned binary values. For example, "A" is 65 in ASCII or 1000001 in binary.
  * This system is used in most of the English-speaking world. Other countries have developed their separate encoding systems, and many are incompatible with each other.
* The different standards, while incompatible, worked fine in a world where faxes and letters were dominant. Once the World Wide Web connected computers worldwide, this became a problem.
  * To remedy this, the Unicode Consortium was created. There are over 100,000 Unicode characters that cover many different languages.
* The problem with having 100,000 characters in UTF-8 is that they need 32 bits to encode it. Since the English alphabet remained in its original designation, a string of English text contained hundreds of zeros and only a few ones.
  * For many older computer systems, eight consecutive zeroes indicate the end of a string. As a result, they will not process any other characters in the text.
* UTF-8 created a system that is compatible with both UTF-8 and ASCII. By adding bits that designate the length and placement of characters, it added room for many more values in a system that originally only supported 128.

## Homework Code Review
* Backticks are better for template literals than doing string concatenation. ESLint provides a message suggesting backticks if concatenation is used.
* `const` creates a constant variable that cannot be changed; `let` allows the variable's value to change.

## Assignments and Comparisons
* The number of equal signs in an operator can determine how it is used. In JavaScript, `=` assigns a value to a variable, `==` compares the values of two operands, and `===` compares both operands' values and data types.
  * Replacing the first equal sign in a comparison operator with an exclamation mark `!` does the inverse; `!=` and `!==` both mean not equal.
* These operators work right to left. JavaScript looks at the value on the right and compares it to the value on the left.
  * For example, the statement `const num1 = 10;` instructs JavaScript to create the value 10 and assign it to the constant variable num1.

# Reflections
* I enjoyed the YouTube video about the history of ASCII. We discussed Unicode and how it relates to binary in our Information Technology class (CIS-185 I think) and converted letters into binary and vice versa.
* In the different coding languages I've worked with, JavaScript is the first that I've seen use the `===` operator. I use `==` and `!=` in C# quite frequently and I think having an operator that compares the values **and** data types
  of two operands is a nice feature.

# Examples
```javascript
// Strings
const firstName = "Jimmy";
const lastName = "Richardson";
console.log(`${firstName} ${lastName}`);  // "Jimmy Richardson"

// Numbers
const num1 = 6;
const num2 = 9;
const difference = num1 - num2; // -3

// Booleans

// MarkDown notes are due on Tuesdays
const isTuesday = true;
const areNotesDue = isTuesday; // true

// Comparison Operators
const num3 = "9";  // string
console.log(num2 == num3);     // true
console.log(num2 === num3);    // false
```
