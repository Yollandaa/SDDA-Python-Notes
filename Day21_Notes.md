# ASYN API
- we use await when we calling annother async function, we know the function we are calling takes sometime.
- await -> has the power to continue execution | 
- When things are dependent on each other I can't parallelize
- When you call await you get the actual return value, but without await you get the co-routine which gather uses as a parameter
- Box -> co-routine | We use gather for boxes
- await -> opens the box

## Quiz
- We use create_task() to make use of the event loop. Scheduling is done right there.
- Why is the request library bad to use?
    - Because it does stuff in synchronous instead of asynchronous
    - Memory management - Error
- We opt for mock-api -> It is free, allows us to modify the data (size and contents).
- Event loop flow -> 
    - Gets invoked when we call asyncio.run()
    - A pause area -> goes to the call stack when it is empty
    - If you do not await the other functions in the main function they get cutted off the event loop, become zombies.
    - A call stack works in the LIFO, and how a stack grows
    - Whatever is in the stack is called blocking -> does not allow event loop
    - If call stack is busy nothing can be added to id, event loop is waiting
    - can avoid blocking by writing good quality code.
- we use separate await tasks -> we are waiting for the longest one to complete.
- Gather mantains the order of 
- all magic methods are dunder methods, but not the other way around.
