# 99-bottles-of-oop
Notes from The Book
> "Quick green excuses all sin."  
> -- *Kent Beck* in *Test-Driven Development by Example*  
## List of Transformations
By priority:  
```assembly
    ({}–>nil)               ;   no code at all->code that employs nil
    (nil->constant)
    (constant->constant+)   ;   a simple constant to a more complex constant
    (constant->scalar)      ;   replacing a constant with a variable or an argument
    (statement->statements) ;   adding more unconditional statements.
    (unconditional->if)     ;   splitting the execution path
    (scalar->array)
    (array->container)
    (statement->recursion)
    (if->while)
    (expression->function)  ;   replacing an expression with a function or algorithm
    (variable->assignment)  ;   replacing the value of a variable.
```


### Flocking Rules
The three **flocking rules** are:  
1. Select things that are most alike.  
2. Find the smallest difference between these.  
3. Make the simplest change to remove the difference.

While changing the code, keep in mind to use only one of the following:  
  1. parse the new code;  
  2. parse and exec;  
  3. parse, exec and use the result;  
  4. delete useless code.  
  
Additional rules to keep in mind:  
* Change one and only one line of code, whenever possible.  
* Run tests after every small change.  
* In case of test failure, undo changes and make better ones.  
