1. Some developers may believe JavaScript has problems because of its asynchronous nature, loose typing, and the web platform it runs on.

   First, JavaScript being asynchronous can make the order of code harder to understand. For example, code with `setTimeout`, event listeners, `fetch`, or promises may not run from top to bottom in the simple way beginners expect. A developer might think one line finishes before the next part runs, but the browser may wait for a user action, a network request, or a timer. This can cause bugs where values are not ready yet, or code runs later than expected.

   Second, JavaScript is loosely typed, so variables can change types easily. This can be helpful, but it can also create unexpected results. For example, `"1" + 2` becomes `"12"` instead of `3` because JavaScript treats it as string concatenation. This can make debugging harder because the code may still run, but the result is not what the developer expected.

   Third, JavaScript runs on the web platform, which means it has to work with browsers, HTML, CSS, user input, network requests, and many different devices. The browser environment is powerful, but it also adds complexity. A web page can be affected by loading order, browser differences, caching, DOM updates, and user actions. Because of this, JavaScript bugs are not always just about the language itself; they can also come from the environment where the code is running.


2. I think JavaScript was made loosely typed because it was designed to be easy and fast to use for web pages. The original purpose of JavaScript was not to be a large, 
   strict programming language for huge applications. It was made to help developers quickly add behavior to websites. Loose typing made the language more flexible and 
   beginner-friendly because developers did not need to declare exact types for every variable.

   I also think asynchronous features were added because web pages need to respond to many things at the same time. A website cannot freeze while waiting for a file to download, a server to respond, or a user to click a button. Asynchronous behavior allows JavaScript to handle events, timers, and network requests without blocking the whole page. This is very important for the web because users expect websites to stay responsive.


3. A compiled language is usually translated into machine code or another lower-level form before the program runs. This means the code is often checked and converted first, 
   and then the compiled program is executed. Languages like C or C++ are commonly compiled.

   An interpreted language is usually executed more directly by another program, such as an interpreter or runtime. Instead of producing a separate executable file first, the code can be read and run while the program is executing.

   JavaScript is usually considered an interpreted language, but modern JavaScript engines are more complicated than that. Browsers often use techniques like just-in-time compilation to make JavaScript run faster. So, in a basic explanation, JavaScript is interpreted, but modern JavaScript engines also compile parts of the code while running.

   One benefit of JavaScript being this way is that it is easy to test and run quickly in the browser. Developers can write code, refresh the page, and immediately see the result. This makes web development faster and more interactive. A drawback is that some errors may only appear while the code is running, and JavaScript may allow confusing behavior because of type conversion and runtime execution.


4. I think the professor is focusing on vanilla JavaScript because it helps us understand the foundation before using frameworks. Frameworks like React, Vue, or Angular 
   are useful, but they are built on top of JavaScript. If we do not understand basic JavaScript, DOM manipulation, events, callbacks, objects, arrays, and asynchronous behavior, then using a framework can feel like memorizing tools without understanding what is happening underneath.

   Mastering  vanilla JavaScript first helps us debug better. When something breaks in a framework, the problem may still come from basic JavaScript concepts like scope, type conversion, functions, or asynchronous code. If we know vanilla JavaScript well, we can understand framework code more deeply and not just copy examples.

   The drawback of not learning a framework is that many modern web projects use frameworks, so we may feel less prepared for real industry projects at first. Frameworks also help organize large applications and make teamwork easier. However, I think learning vanilla JavaScript first is still valuable because it gives us the core knowledge. After that, learning a framework should be easier and more meaningful.


5. This lab relates to my project because our project is also a web-based application, so JavaScript is important for making the page interactive. The concepts in this lab, 
   such as functions, objects, arrays, callbacks, debugging, fetch requests, and event listeners, can all appear in our project.

   For example, if our project has buttons, forms, user input, or dynamic content, we need JavaScript to handle those actions. If the user clicks a button, we may need an event listener. If we need to load data, we may need to use `fetch`. If we store information like products, game symbols, or user choices, we may use objects and arrays.

   The debugging part is also useful. In a team project, bugs can happen easily, especially when different people write different parts of the code. Knowing how to use breakpoints, watch expressions, and the Network tab can help me find problems more clearly instead of guessing. For my own project, I can use these skills to check variable values, understand why a function gives the wrong output, and make sure data is being loaded correctly.