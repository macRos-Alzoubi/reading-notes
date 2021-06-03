# Error Handling & Debugging

JavaScript can be hard to learn and everyone makes
mistakes when writing it. This chapter will help you learn
how to find the errors in your code. It will also teach you how
to write scripts that deal with potential errors gracefully.

When writing a long script, nobody gets everything right in their first attempt. The error
messages that a browser gives look cryptic at first, but they can help you determine what
went wrong in your JavaScript and how to fix it. In this chapter you will learn about:

  - ## THE CONSOLE & DEV TOOLS

    Tools built into the browser that help you hunt for errors.

  - ## COMMON PROBLEMS

    Common sources of errors, and how to solve them.

  - ## HANDLING ERRORS

    How code can deal with potential errors gra cefully.

## ORDER OF EXECUTION

  To find the source of an error, it helps to know how scripts are processed.
The order in which statements are executed can be complex; some tasks
cannot complete until another statement or function has been run.

## EXECUT.ION CONTEXTS

  The JavaScript interpreter uses the concept of **execution contexts**.
There is one global execution context; plus, each function creates a new
new execution context. They correspond to variable scope.

Every statement in a script lives in one of three
execution contexts:

  - ### GLOBAL CONTEXT

    Code that is in the script, but not in a function.
    There is only one global context in any page.

  - ### FUNCTION CONTEXT

    Code that is being run within a function.
    Each function has its own function context.

  - ### EVAL CONTEXT

    Text is executed like code in an internal function
    called `eval()`

### VARIABLE SCOPE

  The first two execution contexts correspond with the
notion of **scope**

  - ### GLOBAL SCOPE

    If a variable is declared outside a function, it can
be used anywhere because it has global scope.
If you do not use the var keyword when creating
a variable, it is placed in global scope.

  - ### FUNCTION-LEVEL SCOPE

    When a variable is declared within a function,
    it can only be used within that function. This is
    because it has function-level scope.


## UNDERSTANDING ERRORS

If a JavaScript statement generates an error, then it throws an **exception**.
At that point, the interpreter stops and looks for **exception-handling** code.

## ERROR OBJECTS

Error objects can help you find where your mistakes are
and browsers have tools to help you read them.

When an Er ror object is created, it will contain the
following properties:

 - ### `name` => Type of execution

 - ## `message` => Description

 - ## `fileName` => Name Of The Javascript File

 - ## `lineNumber` => Line number of error

There are seven types of built-in error objects in
JavaScript. You'll see them on the next two pages:

  - ### Some i.g

    - ### `Error`

      Generic error - the other errors are all based upon this error.

    - ### `Syntax Error`

      Syntax has not been followed.

    - ### `Ref erenceError`

      Tried to reference a variable that is not declared/within scope.

## HOW TO DEAL WITH ERRORS

Now that you know what an error is and how the browser treats them,
there are two things you can do with the errors.

  1. ### DEBUG THE SCRIPT TO FIX ERRORS

     If you come across an error while writing a script
     (or when someone reports a bug), you will need to
     debug the code, track down the source of the error,
     and fix it.

  2. ### HANDLE ERRORS GRACEFULLY

     You can handle errors gracefully using try, catch,
     throw, and f i na 1 ly statements.

     Sometimes, an error may occur in the script for a
    reason beyond your control. For example, you might
    request data from a third party, and their server
    may not respond. In such cases, it is particularly
    important to write error-handling code.

## HANDLING EXCEPTIONS

If you know your code might fail, use try, catch, and finally.
Each one is given its own code block.

  - ### `try`

    First, you specify the code that you t hink might throw an
    exception within the try block.

    If an exception occurs in this section of code, control is
    automatically passed to the corresponding catch block.

    The try clause must be used in this type of error handling code,
    and it should always have either a `catch`, `finally`, or both.

  - ### `catch`

    If the try code block throws an exception, catch steps in with an
    alternative set of code.

    It has one parameter: the error object. Although it is optional,
    you are not handling the error if you do not catch an error.

    The ability to catch an error can be very helpful if there is an issue
    on a live website.

  - ### `finally`

    The contents of the fi na 11 y code block will run either
    way - whether the try block succeeded or failed.

    It even runs if a return keyword is used in the try or catch block.
    It is sometimes used to clean up after the previous two clauses.


  ### THROWING ERRORS

  If you know something might cause a problem for your script, you can
  generate your own errors before the interpreter creates them.

  To create your own error, you use the following line:

  `throw new Error('message') ;`

  This creates a new Error object (using the default Error object). The parameter is the message you
  want associated with the error. This message should be as descriptive as possible.

