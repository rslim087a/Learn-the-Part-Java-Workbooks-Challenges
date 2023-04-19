# Global Superstore 4

**Prerequisite**: You wrote the solution for part 3.


## Task 1
-----
The `run()` method inside a `Runnable` is `void`. If you need to return a value:

- use `Callable` because its `call()` method returns a value.

- Modify your threads to invoke `FutureTasks` instead of `Runnables`. Then, use the `get()` method to retrieve the value from each task.

```
>>: Please enter your name to access the Global Superstore dataset: Rayan

>>: Thank you Rayan. The average sales for Global Superstore are:

>>: Average Furniture Sales: 9799.21280813723
>>: Average Technology Sales: 9854.096986549781
>>: Average Office Supplies Sales: 9540.319577001303
>>: Total Average: 9651.778039610392
```
## Good Luck!
--------
##### Subscribe to our [YouTube Channel](https://www.youtube.com/@RayanSlim087?sub_confirmation=1) and Discover More Valuable Content!