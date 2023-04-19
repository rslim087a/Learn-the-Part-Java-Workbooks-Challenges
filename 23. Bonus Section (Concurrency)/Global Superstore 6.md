# Global Superstore 6

**Goal**: enforce thread safety by locking critical sections of your code.

## Setup
----
Please launch **Workbook 6** inside the Concurrency folder.

## Task 1
-----
Create a function that follows the doc comment. 
```java
    /**
     * Function name: increment
     * @param file
     * 
     * Inside the function:
     *   1. Runs through every line in the file.
     *   2. Maps each element in the stream to a quantity value.
     *   3. Increments sampleSize and quantitySold.
     */
```
The function runs through every line in the file that gets passed in: 

```java
    /**
     * Function name: increment
     * @param file
     * 
     * Inside the function:
     *   1. Runs through every line in the file. <-----
     *   2. Maps each element in the stream to a quantity value.
     *   3. Increments sampleSize and quantitySold.
     */
```

Use this line of code to obtain the Path:

```java
Path path = Paths.get(Thread.currentThread().getContextClassLoader().getResource(file).toURI());
```
Then, use the `Files` class to read every line in the file path as a stream of elements.

The first operation in the stream pipeline should map every element to a quantity value.

```java
    /**
     * Function name: increment
     * @param file
     * 
     * Inside the function:
     *   1. Runs through every line in the file. 
     *   2. Maps each element in the stream to a quantity value. <-----
     *   3. Increments sampleSize and quantitySold.
     */
```

The terminal operation is a `void` `forEach` that increments `sampleSize` and `quantitySold`:

- `sampleSize++;`
-  `quantitySold += quantity;`

## Task 2
----- 
Use multiple threads to execute the following tasks:

- `increment(files[0]);`

- `increment(files[1]);`

- `increment(files[2]);`

After each task finishes (at the end of the increment function), print `sampleSize` and `quantitySold`. 

The correct values are: 
```
Sample size: 1522889
Quantity sold: 8818065
```
But your application is not thread-safe, so your values should be incorrect.

## Task 3
----- 
Employ a locking mechanism that ensures "critical code" is accessed on thread at a time. 

## Task 4
----- 
If you got the correct values, remove your print statements at the end of `increment`. Then, add the following code to `main()`:

            System.out.println("The sample size is: " + sampleSize);
            System.out.println("The quantity sold is: " + quantitySold);

**Final output:**

`>>: The sample size is: 1522889`

`>>: The quantity sold is: 8818065`

## Good Luck!
--------
##### Subscribe to our [YouTube Channel](https://www.youtube.com/@RayanSlim087?sub_confirmation=1) and Discover More Valuable Content!