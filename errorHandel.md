# Error Handling & Debugging 

1. Order of execution :  To find the source of an error, it helps to know how scripts are processed. The order in which statements are executed can be complex; some tasks cannot complete until another statement or function has been run

2. EXECUTION CONTEXTS :The JavaScript interpreter uses the concept of execution contexts. There is one global execution context; plus, each function creates a new execution context. They correspond to variable scope. 

------------------------------------------------


1. Global context Code that is in the script, but not in a function. There is only one global context in any page.
2. FUNCTION CONTEXT Code that is being run within a function. Each function has its own function context.
3. Eval contex  Text is executed like code in an internal function called eval()


---------------------------------------------

* VARIABLE SCOPE The first two execution contexts correspond with the notion of scope
  * GLOBAL SCOPE If a variable is declared outside a function, it can be used anywhere because it has global scope. If you do not use the var keyword when creating a variable, it is placed in global scope.
  * FUNCTION-LEVEL SCOPE When a variable is declared within a function, it can only be used within that function. This is because it has function-level scope.


-------------------------------------------------
## The Stack 
 
Js interpreter process the code line by line 
when we call a function and inside this function we call another function the first function will waiting untll function number two finish 

### EXECUTION CONTEXT & HOISTING

Each time a script enters a new execution context 

1. PREPARE
   * The new scope is created
   * Variables, functions, and arguments are created
   * The value of the this keyword is determined
2. EXECUTE
   * Now it can assign values to variables
   * Reference functions and run their code
   * Execute statements


---------------------------------------------


###  ERROR OBJECTS

1. Error Generic error - the other errors are all based upon this error
2. Syntax Error Syntax has not been followed
3. ReferenceError Tried to reference a variable that is not declared/within scope
4. TypeError An unexpected data type that cannot be coerced
5. Range Error Numbers not in acceptable range
6. URI Error encodeURI ().decodeURI(),and similar methods used incorrectly
7. Eval Error eval() function used incorrectly


---------------------------------------------


##### HOW TO DEAL WITH ERRORS
1. DEBUG THE SCRIPT TO FIX ERRORS
2. HANDLE ERRORS GRACEFULLY



-----------------------------------------------------
##### A DEBUGGING WORKFLOW
1. WHERE IS THE PROBLEM?
2. WHAT EXACTLY IS THE PROBLEM?


##### BROWSER DEV TOOLS & JAVASCRIPT CONSOLE
1. right click on browser page chose inspect element it will showen on the right side of your browser  then find the console 



you can use `console.log()` to show the data in the console 



###### Handling exception 
using `try { //code } catch(exception){consol.log(exception)} finally{always executed}`



## DEBUGGING TIPS
1. ANOTHER BROWSER
2. SEARCH
3. VALIDATION TOOLS
4. VALIDATION TOOLS
5. CODE PLAYGROUNDS
6. STRIP IT BACK
7. EXPLAINING THE CODE



# Summary 
------------------------------
* If you understand execution contexts (which have two stages) and stacks, you are more likely to find the error in your code.
* Debugging is the process of finding errors. It involves a process of deduction.
* The console helps narrow down the area in which the error is located, so you can try to find the exact error.
* JavaScript has 7 different types of errors. Each creates its own error object, which can tell you its line number and gives a description of the error.
* If you know that you may get an error, you can handle it gracefully using the try, catch, finally statements. Use them to give your users helpful feedback.

