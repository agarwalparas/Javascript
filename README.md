# Javascript Concepts

## Table of contents
- [Variable Refrence](#variable-refrence)
- [Variable Scope](#variable-scope)
- [Context](#context)
- [this](#this)
- Function Chaining(#Function-Chaining)
- Functions(#functions)
- Prototypes(#prototypes)
- [Hoisting](#hoisting)

## Variable Refrence

For More [Refrence](https://www.educative.io/collection/page/5679346740101120/5707702298738688/5685265389584384)
- For finding values, make a memory chart of variable, value, memory and then do modifications in that table according to code execution. This will help you to know exact values of variables and the result. To understand this go to above link
- Re-assignmnent a value to variable will make new entry in memory chart with new address
- If Nested object property is assigned to a new variable then that new variable holds the address of that property. Any changes to new variable will change to the object itself

## Variable Scope

For More [Refrence](https://scotch.io/tutorials/understanding-scope-in-javascript#toc-scope-in-javascript)
- Scope refers to the visibility of variables. They are of two types Global , Local
- For var => Declaration outside function have global scope , Inside function has local scope.
- For let and const => Declaration outside function have global scope , Inside function blocks ie if/else, for they have only block scope
- let are not hoisted whereas var are hoisted

## this
For more https://www.educative.io/courses/step-up-your-js-a-comprehensive-guide-to-intermediate-javascript/7nA1nGn3V6A
- Use rules from this page to apply for different types of function invocations
- If multiple rules apply the recent will take place like 
- 1- new (this as new obj)
- 2- apply,call,bind (this as obj pass to bind,callor apply)
- 3- fn call as method (this as the left obj from dot)
- 4- free function invocation(this as global window fn)

## Function-Chaining
FOr more https://medium.com/technofunnel/javascript-function-chaining-8b2fbef76f7f
Eg
var Obj = {
  result: 0,
  addNumber: function(a, b) {
    this.result = a + b;
    return this;
  },

  multiplyNumber: function(a) {
    this.result = this.result * a;
    return this;
  },
 
  divideNumber: function(a) {
    this.result = this.result / a;
    return this;
  }
}

Obj.addNumber(10, 20).multiplyNumber(10).divideNumber(10);


## functions
Read more https://medium.com/@ajmeyghani/javascript-functions-a-pocket-reference-d42597ceb496

## prototypes
Read more https://medium.com/@ajmeyghani/javascript-prototypes-a-pocket-reference-d88f550ffce3

## Context
For More [Refrence](https://scotch.io/tutorials/understanding-scope-in-javascript#toc-lexical-scope)
- It is used to refer this.

