# JS Craziness Reflections

* There was certainly a lot covered in that video. I think it's awesome that JavaScript has ways of providing instructions and limitations to those who use your functions, as adequate feedback is essential in development.
* We've been importing many things in our WWE repository. It's good that you don't have to write your entire project in one file as that can get messy very quickly. I find it similar to importing classes in Java, such as using the `Scanner`
  to add extra capabilities without including hundreds of lines of code.
* The way we edited corresponding elements in parallel arrays was a lot more complex than what I've done in other programming languages. In C#, I'd use a `for` loop and use the index as the increment. With this, we can modify values in
  parallel arrays however we want. If we want to do this without mutating the original arguments, though, I can see how it gets complicated. We couldn't use a `foreach` type loop as we can't modify the value being used.
* I was wondering if there was a `contains` equivalent in JavaScript. I tried to use that several times for the second part of today's homework until I saw that JavaScript uses `includes` instead.
* I also didn't notice the curly brackets around the parameters in the `lib.js` file. I was confused when I used BELTS, CHAMPIONS, and "Tag Team Champions" as arguments and Vite would return an error saying "term1" was undefined.
  After a little troubleshooting, I realized that I had to create an object with those three properties and pass that into `removeCorrespondingItemsByString` for it to work.
