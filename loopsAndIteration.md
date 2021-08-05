## Loops
### Loops allow us to do a process repeatedly
>for(let i=0; i<5; i++>){
    return i;
}
- That returns 1 to 5 and stops at 5. That way we can repeat that process in a loop

- There are many different kinds of loops, but they all essentially do the same thing: they repeat an action some number of times.

#### The various loop mechanisms offer different ways to determine the start and end points of the loop. There are various situations that are more easily served by one type of loop over the others.
- For loops: A for loop repeats until a specified condition evaluates to false. Just like the example above.
>`for ([initialExpression]; [conditionExpression]; [incrementExpression])`
  statement

- do...while loop: The statement is always executed once before the condition is checked. If condition is true, the statement executes again. At the end of every execution, the condition is checked. When the condition is false, execution stops, and control passes to the statement following do...while.
> do
  statement
while (condition);

- For..in: The for...in statement iterates a specified variable over all the enumerable properties of an object. For each distinct property, JavaScript executes the specified statements. A for...in statement looks as follows:
> for (variable in object)
  statement

- For..of: The for...of statement creates a loop Iterating over iterable objects (including Array, Map, Set, arguments object and so on), invoking a custom iteration hook with statements to be executed for the value of each distinct property.
> for (variable of object)
  statement