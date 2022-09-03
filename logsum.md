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


## Class 3 
Note: the notes from this class also come from a [class](https://platzi.com/clases/1798-javascript-navegador/26016-asincronia/) from another [course](https://platzi.com/cursos/javascript-navegador/) which I'd already taken
Last class, we mentioned the Event Loop. The Event Loop is part of the JavaScript Runtime Environment, which also includes the Memory Heap (storage of variables and functions), callback queue, APIs and Call Stack (where every new tasks are stored, from last called function or task until the first one ever, which is the Global Object). The APIs, the Callback Queue and the Event Loop are part of the browser. 

The way the JSRE works is that if it finds something that it piles tasks into the Call Stack. When any of the tasks can't be executed by JS directly (is executed by an API or somthing similar, mainly APIs), it delegates the task to the appropriate component  _and keeps on working_ on the other tasks it finds in the Call Stack. The browser will parallel-work on the task that was delegated to it. Once done, it will place the return value on the Callback Queue. Items on the Callback Queue will be delivered to the main thread of execution once the Call Stack is empty. This "delivery" process is done by the __*Event Loop*__. The Event Loop is like a stan (extremely annoying fan) that constantly asks the Callback Queue if it is done with its work. If it's not, then it will continue asking. If it is, it will deliver the Callback Queue return to the Call Stack. 

In addition to these elements, we can also find the Micro-Task Queue. Here is where promises are executed. Likewise, the JS Environment includes APIs (Application Program Interface). These allow JS to interact with other programs, which can extend JS' functionality. 



# Glossary:
- Asynchronous: multiple things ocurring at the same time
- Concurrent: Interruptability (processor waits until one task is done and does some others while waiting. Not actively doing one of them, just waiting till it's done, then doing the second one)
- Parallelism: Independability (two threads working simultaneously)
