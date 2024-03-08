# _Eloquent JavaScript_ Summary
### From _Automatic Type Conversion_

* JavaScript is very flexible when assessing data types. Using _type coercion_, the language can convert the data types of variables to the type it needs.
  * However, this system can sometimes lead to undesired outcomes for the developer. For example, some expressions will result in the value `NaN`. If you see this in your code, check for accidental type conversions.
  * The same is true when comparing two values. JavaScript has several different operators that assess two values differently. `==` will compare the raw values of two variables; for example, the expression `console.log(false == 0)`
  It will output `false` even though it compares a boolean to a float. The easy solution for this problem is to use `===` instead, as this operator compares both the values and data types of the two variables. This is recommended for most applications.
* When using logical operators such as `&&` and `||`, different data types are handled strangely. The left side is converted to a Boolean to decide what to do, but it can return either value depending on the operator and the result of that conversion.
  * This is useful when using a default value. When a default value is used on the left side of a comparison statement, using `||` will replace it with the value on the right.
    * `&&` has the opposite effect, returning the left value instead.
  * A system called _short-circuit evaluation_ can also be seen with comparison statements. In a statement using `||`, a _true_ value on the left side will cause the program to not even glance at the right value. The same applies when using `&&`
    and there's a false statement on the left.

# Reflections
* I learned a lot of new information in these last couple of sections. I didn't realize the comparison operators had a large amount of rules and guidelines, but given the flexibility of JavaScript, it makes sense.
* The concept of type coercion will take some time to get used to. In languages like C#, even a small conversion like `int` to `double` requires the use of certain keywords and methods. It's interesting how JavaScript is able to determine which
  data type is appropriate for the expression and how it can adjust values as needed.
