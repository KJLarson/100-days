---
layout: post
title: "Day 9: JavaScript Anonymous Functions"
date: 2019-06-04
---

**Today's Progress:** I had been working on the freeCodeCamp Javascript Algorithms And Data Structures Certification before I started the 100 Days of Code challenge. I made it through the Basic JavaScript section without too many problems, but then it started becoming more difficult for me once I hit ES6 and arrow functions/anonymous functions. I tried working on the exercises a couple times, but kept getting stuck on the thought "Why would you want to use anonymous functions? What's the point of them? They just make things confusing." So, rather than keep working on it, I found myself starting other projects. I worked on the Responsive Web Design Certification even though I was already much more comfortable and familiar with the content of that course. I also started my MacBook Pro keyboard, which I worked on for the last 2 days.

Well, today I decided I needed to tackle anonymous functions, as I really want to improve my JavaScript skills. I watched some videos as well as did some reading.

**Helpful Information:** Here is some stuff that helped me understand the topic better:

*[jfriend00 writes on Stackoverflow](https://stackoverflow.com/a/10273250):*

"I use anonymous functions for three reasons:

1. If no name is needed because the function is only ever called in one place, then why add a name to whatever namespace you're in.
2. Anonymous functions are declared inline and inline functions have advantages in that they can access variables in the parent scopes. Yes, you can put a name on an anonymous function, but that's usually pointless if it's declared inline. So inline has a significant advantage and if you're doing inline, there's little reason to put a name on it.
3. The code seems more self-contained and readable when handlers are defined right inside the code that's calling them. You can read the code in almost sequential fashion rather than having to go find the function with that name."

*[Andrew Ensley wrote on the same Stack Overflow quetion](https://stackoverflow.com/a/10282936):*

"I prefer named functions myself, but for me it comes down to one question:

*Will I use this function anywhere else?*

If the answer is yes, I name/define it. If not, pass it as an anonymous function.

If you only use it once, it doesn't make sense to crowd the global namespace with it. In today's complex front-ends, the number of named functions that could have been anonymous grows quickly (easily over 1000 on really intricate designs), resulting in (relatively) large performance gains by preferring anonymous functions.

However, code maintainability is also extremely important. Each situation is different. If you're not writing a lot of these functions to begin with, there's no harm in doing it either way. It's really up to your preference."

[*Helen Emerson wrote:*](http://helephant.com/2012/07/14/javascript-function-declaration-vs-expression/#function-operator-is-an-expression)

"The function operator can be used anywhere that it’s valid to use an expression. For example you can use the function operator when a variable is being assigned, when a parameter is being passed to a function or in a return statement. This is possible because the function operator is always invoked at runtime.

Function declarations are different. They are run before any of the other code is executed so the functions do not have to be declared before the code that calls them.

Function declarations can’t be used to create anonymous functions because they require the function to have a name. The function declaration uses the function name to add it as a variable in the current scope. "

**Thoughts:** I wouldn't say I completely understand anonymous functions now, but maybe a little better than I did. I'll have to come back to them again.

**Resources I Looked At:**
* [16.3: ES6 Arrow Function - Topics of JavaScript/ES6](https://www.youtube.com/watch?v=mrYMzpbFz18) by The Coding Train
*  Stack Overflow: [What are the benefits to using anonymous functions instead of named functions for callbacks and parameters in JavaScript event code?](https://stackoverflow.com/questions/10273185/what-are-the-benefits-to-using-anonymous-functions-instead-of-named-functions-fo)
* [Javascript function declarations vs function operators](http://helephant.com/2012/07/14/javascript-function-declaration-vs-expression/#function-operator-is-an-expression) by Helen Emerson
* [Three reasons I avoid anonymous JS functions like the plague](https://hackernoon.com/three-reasons-i-avoid-anonymous-js-functions-like-the-plague-7f985c27a006) by Justin Fuller

**Links to work:** No live work today.
