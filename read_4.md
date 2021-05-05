# JavaScript
JavaScript is a cross-platform, object-oriented scripting language used to make webpages interactive (e.g., having complex animations, clickable buttons, popup menus, etc.).  There are also more advanced server side versions of JavaScript such as Node.js, which allow you to add more functionality to a website than downloading files.

## Some facts of JavaScript
  - JavaScript borrows most of its syntax from Java, C, and   C++, but it has also been influenced by Awk, Perl, and    Python.
  - JavaScript is case-sensitive and uses the Unicode character set. For example, the word Früh (which means "early" in German) could be used as a variable name.
  But, the variable früh is not the same as Früh because JavaScript is ***case sensitive***.

## Comments
  - **single line comment**: it done by just add ``` // ```
  at the beggening of the line i.g ``` // a one line comment ```  
  - **Multi-line comment**: it done by just add ``` /* */ ```
  and the text gose between the stars symbol i.g ```/* a one line comment */  ```    

### Declarations
  JavaScript has three kinds of variable declarations:

  1. ``` var ```: Declares a variable, optionally initializing it to a value.
  2. ``` let ```: Declares a block-scoped, local variable, optionally initializing it to a value.
  3. ``` const ```: Declares a block-scoped, read-only named constant.

### Variables
You use variables as symbolic names for values in your application.
 - There is some rols applied to variables name:
    ```
    - must start with a letter, underscore (_), or dollar sign ($).
    - Subsequent characters can also be
     digits (0–9). 
    ```

### Declaring variables
You can declare a variable in two ways:
  ```
  - With the keyword var. For example,
  var x = 42.
  This syntax can be used to declare both local and global variables, depending on the execution context.
  - With the keyword const or let. For example,
   let y = 13. This syntax can be used to declare
    a block-scope local variable.
  ```

### Operators
JavaScript has both binary and unary operators, and one special ternary operator.

 1. **binary operator**: An operator requires two operands, one before the operator and one after the operator:
    - i.g: ``` 3 + 4 ``` the ``` + ``` is the operator
 2. **unary operator**: An operator requires a single operand, either before or after the operator:
    - i.g : ``` x++ or ++x```

### Assignment operators
An assignment operator assigns a value to its left operand based on the value of its right operand. 
  - i.g: ``` x = y ```
  - **Addition assignment**: i.g ``` x += y ``` Meaning ```x = x + y```.

   and the same thing is applied to the rest of mathmatical operators```-, *, /, %, ** ```.

### Comparison operators
A comparison operator compares its operands and returns a logical value based on whether the comparison is true.
 - ```Equal (==)```: Returns true if the operands are equal.
 - ```Not equal (!=)```: Returns true if the operands are not equal.
 - ```Strict equal (===)```: Returns true if the operands are equal and of the same type.
 - ```Strict not equal (!==)```: eturns true if the operands are of the same type but not equal, or are of different type.
 - ```Greater than (>)```: Returns true if the left operand is greater than the right operand.
 - ```Greater than or equal (>=)```: Returns true if the left operand is greater than or equal to the right operand.
 - ```Less than (<)```: Returns true if the left operand is less than the right operand.
 - ```Less than or equal (<=)```: Returns true if the left operand is less than or equal to the right operand.

### Logical operators
 Logical operators are typically used with Boolean (logical) values; when they are, they return a Boolean value.
 - ```Logical AND (&&)```: Returns expr1 if it can be converted to false; otherwise, returns expr2. Thus, when used with Boolean values, && returns true if both operands are true; otherwise, returns false.
 - ```Logical OR (||)```: Returns expr1 if it can be converted to true; otherwise, returns expr2. Thus, when used with Boolean values, || returns true if either operand is true; if both are false, returns false.
 - ```Logical NOT (!)```: Returns false if its single operand that can be converted to true; otherwise, returns true.

### String operators
 the concatenation operator ```(+)``` concatenates two string values together, returning another string that is the union of the two operand strings.
    - i.g 
   ```
      console.log('my ' + 'string'); 
      // console logs the string "my string".
   ```
### Control flow
The control flow is the order in which the computer executes statements in a script.
- ```if...else statment```: it's a statment which can control the flow of a program
  - **if...else** structure :
  ```
    if (condition) {
      some sode
  } else {
      some code
  }
  ```
  or
  ```
    if (condition) {
        some sode
    } else if(condition) {
        some code
    }else{
      some code
    }
  ```