## Arrow Functions In JavaScript: Simplified

# Introduction
Arrow functions are now quite commonly used by JavaScript developers. Even if you are just getting started with JS, I'm sure you have heard of them. They may seem intimidating at first and it's completely normal to find yourself avoiding them. However, once you understand them well, you will realize that they just make life easier! With this blog, I aim to make you reach that level of understanding. So, let's get started!

# What are Arrow Functions?
Arrow functions in JavaScript are a modern way to write function declarations. Arrow functions were introduced in JS back in 2015, as a part of JavaScript's ECMAScript Specification 6 (ES6) upgrade. They are nameless functions. Here is the syntax for a single line arrow function

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1659201187548/MtZ6aVhMi.png align="left")

# How Are They Different From Regular Functions?
There are two ways in which they are different:
1. Shorter Code: this can happen in three ways: omitting the brackets around our parameter, not writing "return" and not writing curly braces around the functions

2. 'this' is different: The 'this' keyword works differently in arrow functions. It depends on the object that ** defined ** the function, not the one that called it

Let's discuss these two in detail


## Shorter Code
Arrow functions allow us to write functions in a short and concise manner. What is written in 3 lines of code in regular functions can possibly written in just 1 in arrow functions. 

### Look Mama, No return Keyword or Curly Braces!
A good example of this is when we have to write a single lined function without any parameters. Here's a comparison between the two:
![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1659188982644/36RyEFSid.png align="left")
![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1659188943584/ZtG-tFTwW.png align="left")

### Look Mama, No return Keyword or Parentheses or Curly Braces!!
We are able to achieve this in single-lined functions that have exactly one parameter
![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1659195567322/72jjkFffd.png align="left")
![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1659195643637/JRJ6KPlic.png align="left")

### Look Mama, No... Ummm... No... Nevermind 😔
*there's a twist though!*


When we have to write multi-line functions with more that just a single parameter, arrow functions look quite similar to regular functions. We aren't able to omit the curly braces, the parentheses and the return keyword. Here's an example

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1659198727372/goku8rrNG.png align="left")

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1659198762074/BN5VIxxFC.png align="left")

Yep, quite alike aren't they? But things aren't always the way the look. Now "this" is where the twist comes in!

## "this" Is What You Came For


![6oeqfi.jpg](https://cdn.hashnode.com/res/hashnode/image/upload/v1659199709015/as9_YOB39.jpg align="left")
"this" is a keyword in JavaScript which refers to an object. Which object? Well, that depends on where it is being used. For this blog we'll just discuss how it works differently in arrow functions as compared to regular functions.

### "this" In Regular Functions
![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1659200086439/8Up5RiS0c.png align="left")
In regular functions, "this" depends on which object **calls** the function. This object can be a button, a document, a window etc. So the meaning of "this" can be different for different functions. This can cause errors and get programmers scratching their heads

### "this" In Arrow Functions

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1659200319186/r2MfKzYP9.png align="left")

Arrow functions solve this problem. This is because (pun not intended 😆 ) the meaning of "this"  is simply dependent on the object that **defines** the function, NOT the one that calls it. The value of "this" is inherited from the parent scope.

### Let's See Them In Action
Below is a comparison (taken from w3 schools)
Regular function: output changes from [Object Window] to [object HTMLButtonElement] when the button is clicked because the caller of the func changes from "window" to "button"
Arrow functions: output remains the same as caller doesn't matter

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1659200413067/chw8jBtT3.png align="left")

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1659200423362/BjhFF0WS2.png align="left")

# Summary
Let's summarize the stuff in this blog
- Arrow functions are a modern way of writing functions in JavaScript
- They help us to write functions concisely
- Parentheses, "return" and curly braces are not required for single lined functions which have exactly one parameter
- Return statements and curly braces are not required for single lined functions which have either no parameters or more than just one parameter . They thus save time and make the code look cleaner 
- They help in reducing the confusion caused by the varying meaning of "this"

# That's A Wrap!
![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1659201062675/SQoVP6Qym.png align="left")
Thank you so much for reading this blog to the end! I really value and appreciate your time and I hope you learnt something new and helpful via this blog!

## Special Thanks
I would like to specially thank my sister, [Bhumika Saxena](https://twitter.com/bhumika_0311) for proofreading, reviewing and approving my blog.



