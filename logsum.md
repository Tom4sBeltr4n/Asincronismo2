(remember to read "repoinfo.txt" before working on this)
# Class logs
## Class 2
By itself, a given programming language is synchronous, i. e: every task must be developed at a given time and no other task can be developed at the same time. However, as technology evolved, concepts and resources were added. Some of these additions allow programmers to write programs which can work asynchronously. Among the languages which can be executed asynchronously we can find JavaScript. 

For example, a concept called the event loop gives JavaScript concurrent features. It checks if a task has been completed or not while it runs. Once it runs, other tasks may receive its return value and process it. However, a third type of task happens while the first mentioned task type runs. However, parallel processing isn't available in JavaScript. Another JavaScript characteristic is non-blocking, that is, tasks handle program control after a while return. 

Some of the tools JS uses to manifest is features are callbacks, promises and async functions. 
- Callbacks are functions (A) that are defined at a certain scope, and are used as an argument of a function (B) in the same scope or lower. They are part of the logic of B and may run inside. Recall that if foo and bar are functions, `foo(bar)` is different from `foo(bar())`. In the first case, bar is used as a callback or argument, while in the second one the return value of `bar()` is used as argument. That value may be, for example, a number
- Promises: added in ES6, this is a non-blocking asynchronous function that acomplish a certain code block somewhen during runtime
- Async functions: added in ES8, this is a simple way of using asynchronous and non-blocking code

Other concepts exist, but these 3 are the main.



# Glossary:
- Asynchronous: multiple things ocurring at the same time
- Concurrent: Interruptability (processor waits until one task is done and does some others while waiting. Not actively doing one of them, just waiting till it's done, then doing the second one)
- Parallelism: Independability (two threads working simultaneously)
