# Multi-Paradigm Nature of JavaScript

* I like the idea of a multi-paradigm programming language. I think it allows for more possibilities and more freedom when writing programs. While there are standard protocols that need to be followed,
  JavaScript being a multi-paradigm language means people from many different coding backgrounds can learn how to code in JavaScript.
* In our example, we used a single object to eliminate some of the parameters that were initially required. *Clean Code* recommends functions to have two or fewer parameters, and creating an object with the three
  properties needed to run the function was our workaround. This allows us to only pass one parameter and helps prevent someone from mixing up the order of variables.
  * When passing an object as a parameter, we need to extract the object's properties in order for the function to work as intended. We do this through **destructuring**, where we use dot notation to indicate which
    property we want to use for a statement (i.e. `object.name`).
  * We also want to give default values in case the object that was passed does not have the desired parameters. We do this by assigning values to parameters when the function is first declared. It will appear as though we
    are giving the parameters arbitrary values we are actually providing them defaults if there is no valid property in the argument.
  * Another good failsafe to have when working with JavaScript functions is to use default values when **no** parameter is passed. This can be done by enclosing the parameters in brackets and adding `= {}` to the end of the
    function declaration line.

# Document Object Model (DOM)

* From what I read, the Document Object Model appears to be our first step in adding JavaScript to our web development projects. I think the fundamentals we've learned in the last couple of weeks will help as we transition
  back to the web browser and begin using HTML elements as objects. By understanding the logic used when changing object properties and retrieving values of variables, we can use them to do things in our web pages that
  used to require changing the page source itself.
