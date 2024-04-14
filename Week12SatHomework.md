# Multi-Paradigm Nature of JavaScript

* I like the idea of a multi-paradigm programming language. I think it allows for more possibilities and more freedom when writing programs. While there are obviously standard protocols that need to be followed,
  JavaScript being a multi-paradigm language means people from many different coding backgrounds can learn how to code in JavaScript.
* In our example, we used a single object to eliminate some of the parameters that were initially required. *Clean Code* recommends functions to have two or less parameters, and creating an object with the three
  properties needed to run the function was our workaround. This allows us to only pass one parameter and helps prevent someone mixing up the order of variables.
  * When passing an object as a parameter, we need to extract the object's properties in order for the function to work as intended. We do this through **destructuring**, where we use dot notation to indicate which
    property we want to use for a statement (i.e. `object.name`).
  * We also want to give default values in case the object that was passed does not have the desired parameters. We do this by assigning values to parameters when the function is first declared. It will appear as though we
    are giving the parameters arbitrary values we are actually providing them defaults if there is no valid property in the argument.
  * Another good failsafe to have when working with JavaScript functions is to use default values when **no** parameter is passed. This can be done by enclosing the parameters in brackets and adding `= {}` to the end of the
    function declaration line.
