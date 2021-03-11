# Error Handling & Debugging

#### ORDER OF EXECUTION
To find the source of an error, it helps to know how scripts are processed. 
The order in which statements are executed can be complex; some tasks 
cannot complete until another statement or function has been run

### EXECUTION CONTEXTS 
The JavaScript interpreter uses the concept of execution contexts. 
There is one global execution context; plus, each function creates a new 
new execution context. They correspond to variable scope. 

### EXECUTION CONTEXT 
1. GLOBAL CONTEXT 
Code that is in the script, but not in a function. 
There is only one global context in any page.
2. FUNCTION CONTEXT 
Code that is being run within a function. 
Each function has its own function context.
3. EVAL CONTEXT (NOT SHOWN) 
Text is executed like code in an internal function 
called eva l {) (which is not covered in this book). 

## VARIABLE SCOPE 
The first two execution contexts correspond with the 
notion of scope (which you met on p98):

1. GLOBAL SCOPE 
If a variable is declared outside a function, it can 
be used anywhere because it has global scope. 
If you do not use the var keyword when creating 
a variable, it is placed in global scope. 
2. FUNCTION-LEVEL SCOPE 
When a variable is declared within a function, 
it can only be used within that function. This is 
because it has function-level scope.

## EXECUTION CONTEXT & HOISTING 
Each time a script enters a new execution context, there are two phases 
of activity

1. PREPARE 
* The new scope is created 
* Variables, functions, and arguments are created 
* The value of the this keyword is determined 

2. EXECUTE 
* Now it can assign values to variables 
* Reference functions and run their code 
* Execute statements 

### UNDERSTANDING SCOPE 
n the interpreter, each execution context has its own va ri ables object. 
It holds the variables, functions, and parameters available within it. 
Each execution context can also access its parent's v a ri ables object.

### UNDERSTANDING ERRORS 
If a JavaScript statement generates an error, then it throws an exception. 
At that point, the interpreter stops and looks for exception-handl ing code

### ERROR OBJECTS 
Error objects can help you find where your mistakes are 
and browsers have tools to help you read them. 

### HOW TO DEAL WITH ERRORS 
1. DEBUG THE SCRIPT TO FIX ERRORS 
If you come across an error while writing a script 
(or when someone reports a bug), you will need to 
debug the code, track down the source of the error, 
and fix it. 
2.  HANDLE ERRORS GRACEFULLY 
You can handle errors gracefully using try, catch, 
throw, and f i na 1 ly statements. 


### A DEBUGGING WORKFLOW
Debugging is about deduction: eliminating potential causes of an error. 
**WHERE IS THE PROBLEM?** 
First, should try to can narrow down the area where 
the problem seems to be. In a long script, this is 
especially important. 

1. Look at the error message, it tells you: 
* The relevant script that caused the problem. 
* The line number where it became a problem for 
the interpreter. (As you will see, the cause of 
the error may be earlier in a script; but this is the 
point at which the script could not continue.) 
* The type of error (although the underlying cause 
of the error may be different). 
2. Check how far the script is running. 
Use tools to write messages to the console to tell 
how far your script has executed. 
3. Use breakpoints where things are going wrong. 
They let you pause execution and inspect the values 
that are stored in variables


**WHAT EXACTLY IS THE PROBLEM?** 
Once you think that you might know the rough area 
in which your problem is located, you can then try to 
find the actual line of code that is causing the error. 
1. When you have set breakpoints, you can see if the 
variables around them have the values you would 
expect them to. If not, look earlier in the script. 
2. Break down I break out parts of the code to test 
smaller pieces of the functionality. 
* Write values of variables into the console. 
* Calrfunctions from the console to check if they 
are returning what you would expect them to. 
* Check if objects exist and have the methods I 
properties that you think they do. 
3. Check the number of parameters for a function, or 
the number of items in an array. 

### BROWSER DEV TOOLS & JAVASCRIPT CONSOLE 
The JavaScript console will tell you when there is a problem with a script, 
where to look for the problem, and what kind of issue it seems to be. 

### HOW TO LOOK AT ERRORS IN CHROME 
The console will show you when there is an 
error in your JavaScript. It also displays the line 
where it became a problem for the interpreter. 

### WRITING FROM THE SCRIPT TO THE CONSOLE

Browsers that have a console have a console object, which has several 
methods that your script can use to display data in the console. 
The object is documented in the Console API. 

#### WRITING TABULAR DATA
#### WRITING ON A CONDITION 
Using the console. `assert()` 
method, you can test if a 
condition is met, and write to the 
console only if the expression 
evaluates to false

#### BREAKPOINTS 
You can pause the execution of a script on any 
line using breakpoints. Then you can check the 
values stored in variables at that point in time

### TRY, CATCH, FINALLY 
If you know that you may get an error, you can handle 
it gracefully using the try, catch, finally statements. 
Use them to give your users helpful feedback


