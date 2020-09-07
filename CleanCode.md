# Overview
* [Clean Code](#clean-code)
  * COM3
    * [Communicative](#communicative)
    * [Comprehensive](#comprehensive)
    * [Compact](#compact)

# Clean Code
One of the most important yet least discussed aspects of successful projects is clean code. Although it may be tempting to cut corners to have a feature implemented as quickly as possible, bad programming practices can lead you to much more frustration than you might expect. When writing code, remind yourself that you’ll be rereading that code many months from now — you want to make sure it’ll still make sense after you’ve had a long mental break from it.

Remember COM3:

**Com**municative

**Com**prehensive

**Com**pact

### Communicative
* Use descriptive variable and function names. 
    * `ascii_to_integer()` is far more readable than `atoi()`, for instance. You want to reduce the amount of mental memorization required to read your code.
* Write comments where your code is unclear. 
    * If there’s a specific reason you wrote your code in a particular way (i.e. if there is more than one approach to the problem), write a comment explaining why you chose that approach.
    * If you’re using a library that has a misleading or confusing function, add a comment for clarification.
    * If it is impossible to communicate the meaning of your code without a comment, do it.
* Avoid misinformation
    * If you update a line of code, make sure you re-read its corresponding comment (if it has one). If you make a change to a line of code without changing its comment, it will be *very* difficult to track down a bug introduced by your modification.
    * Don’t “pun” variable names. Sum_array, for instance, is a terrible variable name. Does it mean an array of sums? An array of summaries? What kind of sums/summaries is it holding? No one knows. If the array is holding the summaries of some temperatures, name it temperature_summaries. Another pitfall here would be naming the new array temp_summaries — does temp mean temporary or temperature? 
    * Don’t make assumptions about how something works. Do not write a comment to clarify a weird library function call unless you are certain you understand what’s happening.

### Comprehensive
* Leave no lingering questions.
    * If you read a line of code out of context and find yourself asking “why would this code be written like this?” or “why is this necessary?” or “how does this work?”, that line of code needs to be rewritten or commented.
* Unit test coverage should approach 100%.
    * Unit tests are very small tests that verify that a certain subsection of your code works as expected. You should write enough unit tests so that each line of your program is covered by at least one test case, and each edge case in your program is covered by a test case.
    * Creating a unit test suite will allow you to make changes to your program without worrying about breaking something you didn’t expect. If you have a comprehensive unit test suite, you can simply run it after making a change to make sure everything still works fine. Although the initial cost of writing unit tests is high, the future cost of debugging when random things break is much higher.

### Compact
* You should write as few comments as possible.
    * If you find yourself writing a comment, first try to see if you can rewrite the code instead to make it clearer. Can you rename some variables/functions to make your program more communicative?
* Your code should be DRY
    * **D**on’t **R**epeat **Y**ourself
    * If you find yourself copying and pasting blocks of code and making very small adjustments to them, see if you can make those blocks more generic by using loops, functions, or inheritance.

## Conclusion

Now that you know how to:

1. Pick out a good idea with a problem to solve
2. Create acceptance criteria
3. Define the minimum viable product
4. Manage your project
5. Choose your technologies
6. Implement your project with clean code

...nothing is holding you back! Now, it's time to start thinking about what you might want to construct for the 2021 HackBU Hackathon or our end-of-semester show-and-tell!

We're looking forward to seeing what you create :)
