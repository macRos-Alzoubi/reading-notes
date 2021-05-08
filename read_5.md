# Loops and iteration
**Loops** offer a quick and easy way to do something repeatedly.

There are many different kinds of loops, but they all essentially do the same thing: they repeat an action some number of times,The various loop mechanisms offer different ways to determine the start and end points of the loop. There are various situations that are more easily served by one type of loop over the others.

### The statements for loops provided in JavaScript are:
 - **for statement**:

 A  ***for*** loop repeats until a specified condition evaluates to ***false***. The JavaScript for loop is similar to the Java and C ***for*** loop.
  - A ***for*** statement looks as follows:
    ```
    for ([initialExpression]; [conditionExpression]; [incrementExpression])
    statement
    ```
  - When a ***for*** loop executes, the following occurs:
      1. The initializing expression ***initialExpression***, if any, is executed. This expression usually initializes one or more loop counters, but the syntax allows an expression of any degree of complexity. This expression can also declare variables.
      2. The ***conditionExpression*** expression is evaluated. If the value of ***conditionExpression*** is true, the loop statements execute. If the value of ***condition*** is false, the ***for*** loop terminates. (If the ***condition*** expression is omitted entirely, the ***condition*** is assumed to be true.)
      3. The ***statement*** executes. To execute multiple statements, use a block statement (```{ ... }```) to
      4. If present, the update expression ***incrementExpression*** is executed.
      5. Control returns to **Step 2**.
    - **i.g**:
    ```
    for (let step = 0; step < 5; step++) {
    // Runs 5 times, with values of step 0 through 4.
    console.log('Walking east one step');
    }
    ```

- **do...while statement**

  **The do...while** statement repeats until a specified condition evaluates to false.
  A **do...while** statement looks as follows:
  ```
  do
  statement
  while (condition);
  ```
  ***statement*** is always executed once before the condition is checked. (To execute multiple statements, use a block statement (```{ ... }```) to group those statements.).

  The **do...while** statement executes at least once even if the condition is false.
    - **i.g**:
    ```
    let i = 0;
    do {
    i += 1;
    console.log(i);
    } while (i < 5);
    ```
- **while statement**

A ***while*** statement executes its statements as long as a specified condition evaluates to ***true***. A ***while*** statement looks as follows:
```
 while (condition)
 statement
```
 - **How it works**:

 If the ***condition*** becomes ***false***, ***statement*** within the loop stops executing and control passes to the statement following the loop.

 The condition test occurs before ***statement*** in the loop is executed. If the condition returns ***true***, ***statement*** is executed and the ***condition*** is tested again. If the condition returns ***false***, execution stops, and control is passed to the statement following ***while***.

 - i.g: 
 The following ***while*** loop iterates as long as ***n*** is less than ***3***:
 ```
  let n = 0;
  let x = 0;
  while (n < 3) {
    n++;
    x += n;
  }
 ```