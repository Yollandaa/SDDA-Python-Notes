# Multi Thread and Async
## What happens when you use the async function
- Event loop: Behind async function
- Every aync function returns a coroutine
- Stacking happens when a function calls another function
    - Works like a call stack: LIFO/FILO
    - Things get popped out of the stack -> function returns or finishes
    - To infinitely grow a stack -> do not return | recurion
    - Stack overflow
- illustration of how stacks work : http://latentflip.com/loupe/?code=ZnVuY3Rpb24gYWRkKHgpewogICAgdmFyIGQgPSB4ICsgMQogICAgcmV0dXJuIGQKfQoKZnVuY3Rpb24gc3VtKGEsIGIpewogICAgdmFyIGMgPSBhZGQoYSkgKyBhZGQoYikKICAgIHJldHVybiBjCn0KCi8vIHByaW50CmNvbnNvbGUubG9nKHN1bSgzLCA1KSk%3D!!!

## Asynchronous Code
```js
// Async | Schedule |request
setTimeOut(function sleep() { console.log("Success")}, 2000)

// Sync
console.print("Hi")
console.print("Hi")
console.print("Hi")
console.print("Hi")
console.print("Hi")
```
- After 2 sec execute the code (scheduling) -> doesn't mean it will immediently print. | This is in the callback queue
- Event loop Waits for the call stack to be empty
- "Success" is only printed out when the sync code is done -> stack is empty

### In python
- We have a stack
- A pause area -> when we encounter pause we move it to the pause area, and then back
- We use create_task() to make use of the event loop.
- We use the wait -> to wait for all the tasks to finish | we don't know which one is the longest
- Only use the gather function when you are calling multiple api's

