# _Eloquent JavaScript_ Chapter 3

## Summary

#### Functions
* Functions are essential in coding; they let us create new methods that prevent repetition and allow us to structure larger programs.
* In JavaScript, they are created using the keyword `function` and typically come with parameters to be passed into the function's body, where the code executes when it's called.
  * Functions can have one parameter, many parameters, or none at all. Values of parameters are given by the caller of the function.

#### Bindings and Scopes
* The area where bindings are declared is very important. The binding's scope depends on the block of code it is declared in; variables declared inside a function can only be accessed inside that function.
* Bindings declared outside of a function are global, meaning they can be accessed anywhere in the program.
* JavaScript also recognizes nested scopes, meaning you can build functions within other functions.

#### Declaring Functions
* Functions can be declared anywhere inside a program and can also be called from anywhere inside a program. When first running, the program will add all functions to memory and then run the rest of the code.

#### Arrow Functions
* Another notation of functions uses an arrow (`=>`) instead of the `function` keyword. Despite being very different, they function similarly.

#### The Call Stack
* Computers need to remember the context in which a function was called. They store this information in the _call stack_.
* Once the called function is complete, the computer will remove the top context and use it to continue executing the program.
* It's possible to overload the computer's memory with call stacks, such as creating an infinite loop of functions.

#### Optional Arguments
* Despite defining the number of parameters when creating the function, you can add as many as you want and JavaScript will ignore the extras.
* However, not having an argument for each parameter will cause the remaining parameters to be assigned the value `undefined`.
  * These two features can lead to the program producing the wrong results and it's not clear where things went sideways.
* There is a way for a function to get the whole list of arguments it was passed and allow it to accept any number of arguments. However, that's for the next chapter.

#### Closure
* Local bindings are recreated each time a function is called. This allows the program to reference its value multiple times without issue, a feature known as _closure_.
* This feature can be used to create functions that can repeat an arbitrary number of times without any logic errors.

## Reflections
* I've used some of these concepts in my work in C#. I can think of a recent example where I needed to access a certain text file based on a variable name, and I created a method that, depending on the string passed to it,
  could find the file and assign it to a FileInfo variable. However, I needed to do this multiple times in another method that built a list of phones for an audit program, and this required a special string variable that
  was not included in the original GetFile method. I ended up creating a local GetFile method inside the method that needed a special variable and used it multiple times.
* I've never used the arrow notation when creating a function, but it'd be interesting to see how it differs from the `function` keyword.
* I think having flexibility with parameters is a good thing for creating flexible functions (especially more complex ones). I've seen a couple of instances where I felt a certain method would be handy but I did not have
  all the arguments for it and needed to create variables specifically for that purpose. It would be easier to allow flexibility in the function's code and produce a wider range of results.

## Thoughts on the `hummus` function
* The `hummus` function presented in the Homework Due Tuesday section is an interesting showcase of JavaScript's nested scope capabilities. Within the function, it creates another one called `ingredient` and calls it six times.
* I think it's a decent way to show how nested scope and local bindings interact. But I think having two adjacent functions that both use a local variable with the same name might've demonstrated this better.
