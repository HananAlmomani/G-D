# Error Handling & Debugging

*ORDER OF EXECUTION*
To find the source of an error, it helps to know how scripts are processed.
The order in which statements are executed can be complex; some tasks
cannot complete until another statement or function has been run: 

*EXECUTION CONTEXTS*
The JavaScript interpreter uses the concept of execution contexts.
There is one global execution context; plus, each function creates a new
new execution context. They correspond to variable scope. 

*EXECUTION CONTEXT & HOISTING*
PREPARE:

* The new scope is created
* Variables, functions, and arguments are created
* The value of the this keyword is determined


EXECUTE 
Now it can assign values to variables
* Reference functions and run their code
* Execute statements

*UNDERSTANDING SCOPE*
In the interpreter, each execution context has its own variables object.
It holds the variables, functions, and parameters available within it.
Each execution context can also access its parent's variables object. 


*UNDERSTANDING ERRORS*
If a JavaScript statement generates an error, then it throws an exception.
At that point, the interpreter stops and looks for exception-handling code. 

![errors](https://www.wpoven.com/blog/wp-content/uploads/2019/12/404-error-not-found.png)

**HOW TO DEAL WITH ERRORS**
* DEBUG THE SCRIPT TO FIX ERRORS
If you come across an error while writing a script
(or when someone reports a bug), you will need to
debug the code, track down the source of the error,
and fix it. 

* HANDLE ERRORS GRACEFULLY
You can handle errors gracefully using try, catch,
throw, and finally statements.

**THROW ERROR FOR NaN**
If you try to use a string in a
mathematical operation (other
than in addition), you do not get
an error, you get a special value
called NaN (not a number). 

![nan](https://miro.medium.com/max/638/0*tIhJtvjaWFB7cKNm)




