## What is Javascript?
- JavaScript (JS) is a lightweight, interpreted, or just-in-time compiled programming language with first-class functions. JavaScript is a prototype-based, multi-paradigm, single-threaded, dynamic language, supporting object-oriented, imperative, and declarative (e.g. functional programming) styles
- JavaScript is used mainly for enhancing the interaction of a user with the webpage. In other words, you can make your webpage more lively and interactive, with the help of JavaScript. JavaScript is also being used widely in game development and Mobile application development.

- There are 3 main ways of declaring variables in javascript which are `let`, `const`, `var`
- Then you can pass in value e.g `let company="shipt";`  You can retrieve the value by calling the variable name `company`


### Functions
#### Functions are a way of packaging functionality that you wish to reuse. It's possible to define a body of code as a function that executes when you call the function name in your code. This is a good alternative to repeatedly writing the same code. 
> function reverse(nums){
    let res=0;
    while(nums>0){
        res=res*10+(nums%10);
        res=parseInt(res/10);
    }
    return res;
}

*Notes- Thats how to reverse an integer*

- You can call this above function anywhere, hence reusable

- There is a difference between assignment operator `(=)`, equality operator `(==)` and strict equality operator `(===)`
- The assignment operator assigns a value to a variable or whatever `let num=1`
- The equality operator is used to compare different values `return 1=='1'`   This returns true
- The strict equality operator makes sure they are of the same data type `return 1==='1'` would return false but `return '1'==='1'` would return true

-You can concatenating strings as `str1.concat(str2)` with str1 and str2 representing the variables that hold the values or you could do `let name ="Jane"+"Nunes"`