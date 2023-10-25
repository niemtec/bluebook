Exception handling uses `try`, `catch`, and `finally` to try actions that might not succeed, handle failures when you decide it’s reasonable to do so and to clean up resources afterwards.
Exceptions are generated using the `throw` keyword.
Sometimes exceptions are thrown not by the method that your code uses, but by another method further down the call stack — that’s when CLR will unwind the stack looking for a method with a `catch` block for that exception type and execute the first one it finds. (The error “bubbles up” until it is caught)

If no error handling has been implemented, the program will terminate the process and display a message to the user.

Once an exception occurs in the `try` block, the flow of control jumps to the first associated exception handler that is present anywhere in the call stack.
> Don't catch an exception unless you can handle it and leave the application in a known state. If you catch `System.Exception`, re-throw it using the `throw` keyword at the end of the `catch` block.

`catch` blocks can also define an exception variable which can be used to obtain more information about the error. 
