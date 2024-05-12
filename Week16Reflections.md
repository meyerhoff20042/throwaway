# Form Validation Reflections

* That was a rough assignment for me to get through. After following the videos, I was able to get basic validation onto my form, but I was encountering errors with my
  Email text box. For whatever reason, when the email didn't fit the criteria specified by the Validator class, it would trigger the error on the name text box instead of
  the email. I tried many different things to fix this, including:
  * Using `nextElementSibling` instead of `parentNode`
  * Moving the hideErrors and renderErrors functions to `main.js` instead of `utils.js`
  * Addressing the email text box specifically in the `hideError` and `renderError` methods
  * And many other far-fetched ideas
* What ended up fixing it for me was adding embedded JavaScript functions inside the HTML file that would validate the form before submitting it. I wanted to do it on `main.js`, but for whatever reason,
  the HTML file was unable to recognize functions from the separate file that weren't made in the videos. I assume I imported something wrong somewhere, but there was nothing I was able to find to fix it.
* I learned a lot of new things on this journey, through trial & error, web docs, and AI assistance. As mentioned previously, I learned about `nextElementSibling` and how that differs from `parentNode`
  (`parentNode` would reference the `form` class itself while `nextElementSibling` actually retrieved the element).
  * I examined the Validator GitHub page to look for extra information that might help, and I learned of many different ways Validator can be useful. It can validate emails, phone numbers, and you can
    even add custom specifications for it.
  * I had never used the `required` tag in an HTML form before today, and I'm glad I know that exists now.
  * I spent a long time trying to work an `onclick` attribute into the submit button, and it took a long conversation with ChatGPT before it informed me that I needed to use an `onsubmit` attribute
    in the form itself.
* During this time, I pushed a lot of changes onto the GitHub repository. I needed to use pretty specific commit messages and on several occasions needed to highlight certain lines. This was the first
  time I had to do that and it was a lot easier than I thought it'd be.
