# Sprint Challenge - JavaScript Fundamentals

**Read these instructions carefully. Understand exactly what is expected _before_ starting this Sprint Challenge.**

This challenge allows you to practice the concepts and techniques learned over the past week and apply them in project. This Sprint explored JavaScript Fundamentals. During this Sprint, you studied array methods, this keyword, prototypes, and class syntax. In your challenge this week, you will demonstrate proficiency by completing a range of JavaScript problems.

This is an individual assessment. All work must be your own. Your challenge score is a measure of your ability to work independently using the material covered through this sprint. You need to demonstrate proficiency in the concepts and objectives introduced and practiced in preceding days.

You are not allowed to collaborate during the sprint challenge. 

## Introduction

The index.js file contains all of your challenges. Please review it in full before answering the questions. If you complete the stretch goals please leave them in your file but commented out so that they do not affect the MVP tasks 

In meeting the minimum viable product (MVP) specifications listed below, you should have all tests passing. You can console.log to check your work and ensure you are submitting the correct results 

### Commits

Set up codegrade early and commit your code regularly and meaningfully. 

## Interview Questions
### (please edit this file and write your answer below each question.)
Demonstrate your understanding of this week's concepts by answering the following free-form questions.

Edit this document to include your answers after each question. Make sure to leave a blank line above and below your answer so it is clear and easy to read.

1. Explain the differences between `.map`, `.reduce` and `.filter` and describe a use case for each. 

.map() - this method is useful for creating a new array from an existing array. It does NOT manipulate existing array and it needs a return keyword. With this method one can manipulate the existing array and perform an operation on each element. For example, if I have a dataset of a passenger names of a cruise ship and the data is dirty where the passenger names are all lowercase, I can use .map() to manipulate passenger names so that theyre gramatically correct.

.filter() - this method also returns a new array but does not manipulate the original array. It simply filters out results into a new array. In other words, if the condition is true, it will include the item into the new array. If false, it will be excluded. Using the cruise ship example from above, if i wanted to give a child discount for passengers 12 and younger, i can use filter() to return an array with the name of passengers who are 12 and younger. 

.reduce() - this method also does not return a new array; however, it returns a single value. It is used for addition and multiplication purposes. For example, if I wanted to add the number of passengers from fiscal year 2018 through 2021, I can use .reduce on that data to add up the number of people buy tickets for my cruise ship business. 

2. Explain the difference between a callback and a higher order function.

A higher order function is a function that receives other functions as a parameter. Whereas a callback is a function that is intended to be passed into other functions as arguments. Higher order functions receives a callback, and callbacks are passed into higher orders. 

3. Explain what a closure is.

Closure is being able to reference a specific variable or values outside of a scope or curly braces. For example, an inner function is able to reference a variable in an outer function to order to run a program. When a function is called, a function needs information in order to run. A closure is NOT when a function is self contained where it depends on its own arguments. However, when theres data being referenced outside of the scope of the function, closure is used to feed that outside information into the function.

4. Describe the four principles of the 'this' keyword.
This is a keyword that references another value in an object. The four principles are the following:

1)Window Binding - if no other rules apply, 'this' defaults to the window (unless youre in strict mode it returns undefined). When used on the console, the window object gets returned. 

2)Implicit Binding - Applies when youre using a method. When the method is invoked, the object 'this' is referring to is to the left of the dot. 

3)Explicit Binding- We explicitly tell javascript what 'this' is being referred to. We use these methods to for explicit binding: 
.call() . apply() .bind(). 

.call() will invoke the function immediately and arguments are passed one by one. We can also use Call() to invoke a method which allows us to "borrow" a method from one object and then use it on another object.

.apply() is similar in that both immediately invoke a function in scope of first argument; however, call() is limited if you dont know the number of arguments. Apply() takes an array of arguments. 

.bind() also lets you pass arguments one by one but will not invoke the function immediately. This returns a new function that can be invoked later.

4)New Binding - 
When a function is invoked with the new keyword, the this is bound to the new object being constructed. 'This' points to the new object thats is being created. By using the new keyword, a new object is constructed and 'this' points to it. 




5. Why do we need super() in an extended class?

When we are making child classes, super is needed because it is what parent.call does. It is used to access and call functions on an object's parent. Without it one cannot make a child class that inherits Parent attributes. Extend in class syntax tells super what to super to. Overall, it is reference to the parent class (super class). It is also helpful to use in order to reduce repeat code. 

You are expected to be able to answer questions in these areas. Your responses contribute to your Sprint Challenge grade. 

## Instructions

### Task 1: Set up Project

Using VSCode and Command Line:


1. Fork the repo
2. Go into canvas and connect your reop to codegrade
3. Clone your forked version of the repo
4. DO NOT CREATE A BRANCH. You will be pushing your changes to the main/master today
5. cd into your repo
6. open the terminal in your vs code and type `npm install`
7. next type `npm run test` in your terminal
8. Complete your work making regular commits to main/ master your codegrade score will update each time you make a push.


### Testing & Debugging

Open a second terminal inside of your project by clicking on the split terminal icon
![alt text](assets/split_terminal.png "Split Terminal")

Inside of your second terminal type `npm start` 
![alt text](assets/npm_start.png "type npm start")

You will be running your tests in one terminal and debugging in the other. As you work on your code you should make use of `console.log` to check your progress and debug.
![alt text](assets/tests_debug_terminal_final.png "your terminal should look like this")

### Task 2: Project Requirements (MVP)

You must complete all tasks inside of `index.js` and answer the questions above.

In your solutions, it is essential that you follow best practices and produce clean and professional results. Schedule time to review, refine, and assess your work and perform basic professional polishing including spell-checking and grammar-checking on your work. It is better to submit a challenge that meets MVP than one that attempts too much and does not.

## Resources
 
 [Sprint Challenge Study Guide](https://www.notion.so/lambdaschool/Unit-1-Sprint-3-Study-Guide-033a9a00659a4ef98c12eb97e49a6110)

## Submission format

Please submit your project via codegrade by following [these instructions](https://lambdaschool.notion.site/lambdaschool/Lambda-School-Git-Flow-Step-by-step-269f68ae3bf64eb689a8328715a179f9) See part 2, submitting an assignment with codegrade
