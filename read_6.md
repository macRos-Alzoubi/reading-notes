# Functions
A JavaScript function is a block of code designed to perform a particular task.
A function is executed when "something" invokes it (calls it).

### -JavaScript Function Syntax
A JavaScript function is defined with the ```function``` keyword, followed by a **name**, followed by parentheses **()**.

Function **names** can contain **letters**, **digits**, **underscores**, and dollar signs (same rules as variables).

The parentheses may include parameter names separated by **commas**:
(parameter1, parameter2, ...)

The code to be executed, by the function, is placed inside curly brackets: **{}**
  - i.g 
  ```
  function name(parameter1, parameter2, parameter3) {
  // code to be executed
  }
  ```

    1. Function **parameters** are listed inside the parentheses **()** in the function definition.
    2. Function **arguments** are the **values** received by the function when it is invoked.
    3. **NOTE**: Inside the function, the **arguments (the parameters)** behave as ***local variables***.

### -Function Invocation
The code inside the function will execute when "something" **invokes** (calls) the function:
  - When an event occurs (when a user **clicks** a button)
    - i.g:
    ```
    document.addEventListener('click', e =>{
      //Some code
    };
    ```
  - When it is **invoked** (called) from JavaScript code
    - i.g:
    ```
    let sum = getSum(12,24);
    ```
  - Automatically (self invoked)

### -Function Return
When JavaScript reaches a ```return``` statement, the function will stop executing.

If the function was invoked from a statement, JavaScript will **"return"** to execute the code after the invoking statement.

Functions often compute a **return value**. The return value is **"returned"** back to the **"caller"**:
  - i.g:
  ```
  //Calculate the product of two numbers, and return the result
  var x = myFunction(4, 3);   // Function is called
  return value will end up in x

  function myFunction(a, b) {
    return a * b;             // Function returns the product of a and b
  }
  ```
### -Why Functions?
  1. **Code Reusability**:

  We can reuse code: Define the code once, and use it many times.
  We can use the same code many times with different arguments, to produce different results.

  2. **Code Organization**:

  We can organize our code and make it cleaner.

### -The () Operator Invokes the Function
We can call a **function** by just typing the function **name** followed by **()** and the **argument list** if any.
**NOTE**:
Calling a function without **()** will return the **function object** instead of the **function result**.

### -Functions Used as Variable Values
Functions can be used the same way as you use **variables**,in all types of **formulas**, **assignments**, and **calculations**.
  - **i.g**:
  ```
  //Instead of using a variable to store the return value of a function
  var x = toCelsius(77);
  var text = "The temperature is " + x + " Celsius";
  //You can use the function directly, as a variable value
  var text = "The temperature is " + toCelsius(77) + " Celsius";
  ```

### -Local Variables
Variables declared within a JavaScript function, become **LOCAL** to the function.

Local variables can only be accessed from within the function.
  -**i.g**:
  ```
  // code here can NOT use carName

  function myFunction() {
    var carName = "Volvo";
    // code here CAN use carName
  }

  // code here can NOT use carName
  ```
**NOTE**:
  - Since **local variables** are only recognized inside their functions, **variables** with the same name can be used in **different functions**.
  - Local variables are created when a function starts, and deleted when the function is completed.
