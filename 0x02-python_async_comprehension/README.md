Async Comprehension
This project contains tasks for learning to use asynchronous comprehensions in Python 3.

Tasks To Complete
 0. Async Generator
0-async_generator.py contains an asynchronous coroutine called async_generator that takes no arguments and meets the following requirements:

The coroutine will loop 10 times, each time asynchronously wait 1 second, then yield a random number between 0 and 10.
Use the random module.
 1. Async Comprehensions
1-async_comprehension.py contains a script that meets the following requirements:

Import async_generator from the previous task and then write a coroutine called async_comprehension that takes no arguments.
The coroutine will collect 10 random numbers using an async comprehensing over async_generator, then return the 10 random numbers.
 2. Run time for four parallel comprehensions
2-measure_runtime.py contains a script that meets the following requirements:

Import async_comprehension from the previous file and write a measure_runtime coroutine that will execute async_comprehension four times in parallel using asyncio.gather.
measure_runtime should measure the total runtime and return it.
