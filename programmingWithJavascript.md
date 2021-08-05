## Expressions and operators
### Javscript has different types of operators
- Assignment Operator `=` :An assignment operator assigns a value to its left operand based on the value of its right operand. `let var = 15`
  - Addition assignment `+=`: This adds and assign to a variable `let var+=15`
  - Subtraction assignment `-=`: This subtracts and assigns to a variable `let var-=15`
  - Remainder assignment `%=` : The remainder assignment operator (%=) divides a variable by the value of the right operand and assigns the remainder to the variable. `let var%=15`
- Comparison Operator `== || ===`: A comparison operator compares its operands and returns a logical value based on whether the comparison is true. `return 5==='5'` returns false because they are different data types
- Logical Operators: Logical operators are typically used with Boolean (logical) values; when they are, they return a Boolean value. However, the && and || operators actually return the value of one of the specified operands, so if these operators are used with non-Boolean values, they may return a non-Boolean value. `&&`-AND, `||`-OR, `!`-NOT.
- String operator: The concatenation operator (+) concatenates two string values together, returning another string that is the union of the two operand strings. `let school= "pivot "+"tech"`
- Conditional (ternary) operator: This works depending on a outcome `condition ? val1 : val2`. If the condition is true, val1 is used else val2



## Expressions
### An expression is any valid unit of code that resolves to a value. There are two types of expressions: with side effects (for example: those that assign value to a variable) and those that in some sense evaluate and therefore resolve to a value. The expression x = 7 is an example of the first type. This expression uses the = operator to assign the value seven to the variable x. The code 3 + 4 is an example of the second expression type. This expression uses the + operator to add three and four together without assigning the result, seven, to a variable.

### Primary Expressions
- this
Use the this keyword to refer to the current object. In general, this refers to the calling object in a method. Use this either with the dot or the bracket notation:
> this['propertyName']
this.propertyName

## Functions
#### Functions are one of the fundamental building blocks in JavaScript. A function in JavaScript is similar to a procedure—a set of statements that performs a task or calculates a value, but for a procedure to qualify as a function, it should take some input and return an output where there is some obvious relationship between the input and the output.

### Function Declaration
- A function definition (also called a function declaration, or function statement) consists of the function keyword, followed by: name of the function, a list of parameters to the function, enclosed in parentheses and separated by commas, the JavaScript statements that define the function, enclosed in curly brackets, {...}.
>function divide(m, n){
    let div=m/n;
    return div;
}

### Function Expression
- Such a function can be anonymous; it does not have to have a name. For example, the function divide could have been defined as:
>let divide=function(m,n){
    let div=m/n;
    return div;
}

### Calling functions
- Defining a function does not execute it. Defining it names the function and specifies what to do when the function is called.

- Calling the function actually performs the specified actions with the indicated parameters. For example, if you define the function divide, you could call it as follows:
> divide(8,2);

### Function Scope
- A function defined in the global scope can access all variables defined in the global scope. A function defined inside another function can also access all variables defined in its parent function, and any other variables to which the parent function has access.

### Nested functions and closures
- The inner function can be accessed only from statements in the outer function.
- The inner function forms a closure: the inner function can use the arguments and variables of the outer function, while the outer function cannot use the arguments and variables of the inner function.

## Control Flow
- Refers to the way the computer executes statement in a script
- Code is run in order from the first line in the file to the last line, unless the computer runs across the (extremely frequent) structures that change the control flow, such as conditionals and loops. 
Example:
>if (field==empty) {
    promptUser();
} else {
    submitForm();
}
- if field is not empty, it skips and goes to submit form