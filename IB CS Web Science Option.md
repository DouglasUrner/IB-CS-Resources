IB CS Web Science Option
========================

My idea for this option is to teach web application development using an object oriented language (JavaScript or Ruby are my first thoughts) with a database backend. I would like to model several possibilities and then let students pursue their own choice of tools. For example a student could develop in Meteor or use Ruby on Rails.

## History

## Programming Models

### Object Oriented Programming

### Functional Programming

## Database Concepts

### Database Models

* [Relational]() –
* [Document](http://en.wikipedia.org/wiki/Document-oriented_database) –
* [Graph](http://en.wikipedia.org/wiki/Graph_database) –
* []() –


* [ACID](http://en.wikipedia.org/wiki/ACID)
* [CAP](http://en.wikipedia.org/wiki/CAP_theorem)

## Resources

### General Purpose Tools

#### Browsers

#### Editors

A good editor is an essential tool for programmers. There are many choices and feelings about the "best" editor tend to run strong. Pick on that you like and ignore the drama.

The essential requirement of a programmer's editor is that "what you see is what ends up on disk." The file you save should look exactly like the file that you're looking at in the editor. This is very different from word processors like Microsoft Word that show you the final presentation of the document and save the file in a very different format than what appears on the screen as you are editing the file. This requirement is important because the file you are editing will become the input to another program – for example a compiler or a web browser. The code you are typing is what you want the next program in the process to see and extra information added by a word processor would confuse the program that will be interpreting what you write.

Programmer's editors also include features, such as syntax coloring and automatic indenting, to make typing code easier.

The lists are in alphabetical order. It is worth knowing at least one very well and having a passing familiarity with several others.

##### Free Editors (including ones included with your OS):


* [Atom](http://atom.io) –
* [Emacs]() – emacs has been around for a long time, since the days when detractors could reasonably complain that its name was not a contraction of "editing macros" but an acronym for "Eight Megs And Constantly Swapping" (eight megs as in eight megabytes of main memory in the computer). Many editors (and command history mechanisms base their keyboard commands on those used by emacs.)
* [Vi]() – vi is the Berkeley Unix visual (screen oriented, as opposed to line oriented) editor written by Bill Joy as a front end for his line oriented ex editor. Vi was part of the first BSD Unix release in 1978. If a screen oriented application doesn't implement emacs key bindings, it is a good bet that it will implement vi key bindings. Vi has been rewritten a number of times (nvi and [vim](http://www.vim.org)).

##### Commercial Editors

* [Sublime Text]() –

##### Integrated Development Environments (IDEs)

#### Debuggers

#### Source Code Management (SCM) Systems

Source code management (SCM) systems or revision control systems or whatever you choose to call them, are important tools for software developers. A SCM system enables you to manages the changes you (either individually or as part of a team) make to a body of source code. This makes it possible for you to make changes, see what has changed, back out of changes, reproduce older versions – all very useful tricks, especially when the code is in production.

##### Git

Git is widely used and the tools are supported on all of the major OSes used by developers. There is a Windows version too. Git supports distributed collaboration which makes it suitable for large scale open source projects. Many of these projects are hosted on GitHub which also provides tools for issue tracking and the ability to host a web site.

* [Git](http://git-scm.com) –
* [Pro Git](http://git-scm.com/book/en/v2) – reference book for Git users.
* [GitHub](https://github.com) –
* [How to Use Git and GitHub](https://www.udacity.com/course/ud775) –

#### Testing

### Languages

_"A language that doesn't affect the way you think about programming, is not worth knowing"_ ~ Alan Perlis (as quoted by Peter Norvig in [Teach Yourself Programming in Ten Years](http://norvig.com/21-days.html))

By definition the first langage you learn affects the way you think about programming – it has to, unless you somehow manage to learn the language without learning how to program… This also means that, like natural languages, you are really not a fully literate person (in any language) until you have (at least) enough experience in another language to have it impact how you think about programming.

#### HTML

#### CSS

#### JavaScript

AKA ECMA-262

##### JavaScript Fundamentals

###### JavaScript 101 – Just enough to get something useful done.

###### Understanding Scope – Because Javascript does some weird stuff

Once you know about variables, it is time to learn about scope. Roughly speaking a variable's scope tells you where and when in the program the variable has meaning.

JavaScript does several odd (at least if you know another language or two) things with scope:

* There are two scopes: global and function. Unlike many other languages there is no block scope – JavaScript doesn’t give you new scope when you open up a pair of curlies.
* Variables declared with `var` are "sensible" in their scope, variables declared in a function have function scope, variables declared outside of a function have global scope.
* Variables can be declared implicitly by assigning to them. Those variables have __global__ scope – even when you declare them inside of a function! This __never__ turns out well – especially in big projects.
* Variables "come to life" when they are declared – this means, for example, that even though a variable has function scope, it is not __defined__ (meaningful) in the function until is is declared. This means that a variable can be tested (without causing an error) before it is declared.


* [JavaScript Scope](http://www.w3schools.com/js/js_scope.asp) – Start here, most days this will get you through most of the quirks of scope in JavaScript. Don't just read it, try the code. Think of some weird things and try them out. Play until you feel like you are understanding things – or until you have a question that you can't sort out. Ask a few of your peers, then if you are still unsure ask Google, then ask me.
* [What You Need To Know About JavaScript Scope](http://www.smashingmagazine.com/2009/08/01/what-you-need-to-know-about-javascript-scope/) –
* [Again With the Module Pattern – Reveal something to the world](http://christianheilmann.com/2007/08/22/again-with-the-module-pattern-reveal-something-to-the-world/) –
* [jQuery: Extending bind() to define context of execution (scope)](http://www.sanghvilabs.com/2009/02/04/jquery-extending-bind-to-define-context-of-execution-scope/) –
* [Javascript Closures](http://jibbering.com/faq/notes/closures/) – Not for the faint of heart.

##### Other Interesting JavaScript Articles & Resources

* [JavaScript](https://developer.mozilla.org/en-US/docs/Web/JavaScript) – language reference, tutorials, and other resources from the Mozilla Developer Network (MDN).
* [Learning JavaScript Design Patterns](http://addyosmani.com/resources/essentialjsdesignpatterns/book/) – free online copy of the book by the same title.
* [3 ways to define a JavaScript class](http://www.phpied.com/3-ways-to-define-a-javascript-class/) –
* [Using Objects to Organize Your Code](http://rmurphey.com/blog/2009/10/15/using-objects-to-organize-your-code/) –
* [JavaScript Module Pattern: In-Depth](http://www.adequatelygood.com/JavaScript-Module-Pattern-In-Depth.html) –
* [Immediately-Invoked Function Expression (IIFE)](http://benalman.com/news/2010/11/immediately-invoked-function-expression/) –
* [A brief introduction to closures](http://skilldrick.co.uk/2010/11/a-brief-introduction-to-closures/) –
* [Closures explained with JavaScript](http://skilldrick.co.uk/2011/04/closures-explained-with-javascript/) –
* [ECMA-262-3 in detail. Chapter 5. Functions.](http://dmitrysoshnikov.com/ecmascript/chapter-5-functions/#question-about-surrounding-parentheses) –
* [JavaScript MVC](http://alistapart.com/article/javascript-mvc) –
* [Eloquent JavaScript](http://eloquentjavascript.net) –
* [Introduction to Object-Oriented JavaScript](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Introduction_to_Object-Oriented_JavaScript) –
* []() –

#### Online Classes

##### Udacity

* [Intro to HTML and CSS](https://www.udacity.com/course/ud304) –
* [JavaScript Basics](https://www.udacity.com/course/ud804) –
* [Web Development](https://www.udacity.com/course/cs253) –
* [Object-Oriented JavaScript](https://www.udacity.com/course/ud015) –
* [Intro to jQuery](https://www.udacity.com/course/ud245) –
* [Intro to AJAX](https://www.udacity.com/course/ud110) –
* [Website Performance Optimization](https://www.udacity.com/course/ud884) –
* [HTML5 Game Development](https://www.udacity.com/course/cs255) –


#### JavaScript Frameworks
* [jQuery]()
* [Meteor](https://www.meteor.com)
  * [Building large, modular apps in Meteor](http://tech.exponential.io/meteor/building-large-modular-apps-meteor/) – ideas for how to organize a large Meteor application.
  * [Build a File Upload Package](https://www.eventedmind.com/feed/meteor-build-a-file-upload-package) – video tutorial series that builds a file upload package for use in Meteor applications. [Source code](https://github.com/EventedMind/meteor-build-a-file-upload-package) for the package is on GitHub
* [Node.js]()
* [Lineman.js](http://linemanjs.com) – command line JavaScript tools for the client side of client-server application models.

### PHP

### [MongoDB](https://www.mongodb.org)

MongoDB is an open-source document database. It is one of a class of databases referred to as a [NoSQL](http://en.wikipedia.org/wiki/NoSQL) database. MongoDB is the default underlying database for Meteor.

* [Mongo Manual](http://docs.mongodb.org/manual/) –
* []() –
* []() –
* [6 Rules of Thumb for MongoDB Schema Design: Part 1](http://blog.mongodb.org/post/87200945828/6-rules-of-thumb-for-mongodb-schema-design-part-1) –
* [6 Rules of Thumb for MongoDB Schema Design: Part 2](http://blog.mongodb.org/post/87892923503/6-rules-of-thumb-for-mongodb-schema-design-part-2) –
* [6 Rules of Thumb for MongoDB Schema Design: Part 3](http://blog.mongodb.org/post/87200945828/6-rules-of-thumb-for-mongodb-schema-design-part-1) –


### Ruby on Rails

#### Ruby

#### Rails

### Maria DB / MySQL
