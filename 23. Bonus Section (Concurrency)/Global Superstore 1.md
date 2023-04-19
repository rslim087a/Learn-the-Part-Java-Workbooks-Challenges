# Global Superstore – Part 1

Please launch **Workbook 1** inside the Concurrency folder.

## Task 1
---
Inside the `data` directory, a CSV file stores ~1,000,000 records. The `main()` method already contains boilerplate code that locates the `Path` of the csv file.

```java
Path path = Paths.get(Thread.currentThread().getContextClassLoader().getResource(SALES).toURI());
```
Create a function based on the following Doc Comment:

```java
    /**
     * Function name: average
     * @param path (Path)
     * @param category (String)
     * @return Double
     * 
     * Inside the function:
     *   1. Runs through every line from the CSV file as a stream.
     *   2. Maps every element in the stream to an array of three values.
     *   3. Filters every value by the @param category
     *   4. Maps every element in the stream to a double (price * quantity).
     *   5. Applies the terminal operation average.
     *   6. Returns the average as double.
     * 
     */
```
The function receives two parameters and returns a `Double` average.

```java
    /**
     * Function name: average
     * @param path (Path) <--------
     * @param category (String) <--------
     * @return Double <--------
     * 
     * Inside the function:
     *   1. Runs through every line from the CSV file as a stream.
     *   2. Maps every element in the stream to an array of three String values.
     *   3. Filters every value by the @param category
     *   4. Maps every element in the stream to a double (price * quantity).
     *   5. Applies the terminal operation average.
     *   6. Returns the average as double.
     * 
     */
```
**Hints for 1, 2, 6:**

- You can run through all lines as a stream of elements using: `Files.lines(path)`. This line throws a checked exception so place it in a `try` block.
- You can skip the first element using `.skip(element number)`.
- You can "split" each String into an array of String values.

-  The terminal operation `average()` returns an `OptionalDouble`. Use `getAsDouble` to return a `Double`. 

In the event of an exception, print its message and return `0.`.
## Task 2
---

Create a function based on the following Doc Comment:

```java
    /**
     * Function name: totalAverage
     * @param path
     * @return Double
     * 
     * Inside the function:
     *   1. Runs through every line from the CSV file as a stream.
     *   2. Maps every element in the stream to an array of three values.
     *   3. Maps every element in the stream to a double (price * quantity)
     *   4. Applies the terminal operation average
     *   5. Returns the average as double.
     * 
     */
```
In the event of an exception, print its message and return `0.`.


## Task 3
---

- Call the `average` method for `"Furniture"`, `"Technology"`, and `"Office Supplies"`.
- Call the `totalAverage` method.

After calling your methods, copy the following at the  end of your `main()` method.


```java
     Scanner scan = new Scanner(System.in);
     System.out.print("Please enter your name to access the Global Superstore dataset: ");
     String name = scan.nextLine();
     System.out.println("Access Denied. We apologize for the inconvenience. Have a good day " + name + ".");
     scan.close();
```

## Task 4
---

Run your code:

![Screen Shot 2021-09-20 at 4.00.57 PM.png](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F3b77637f-9f5a-45d0-a7e8-885fbf68d46f?alt=media&token=c8f1d1a7-dd74-400d-b72d-2b019493f7f7)

**Not good!** The calculations are blocking the `main()` thread. The user has to wait a few seconds before they can answer the question. Blocking the `main()` thread negatively affects user experience.

## Task 5
----
The calculations are time-intensive. Run each calculation on another thread.

## Task 6
----
Run the app

![Untitled.gif](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F940e4ead-9f4a-4b6e-8b10-1fc58141a8df?alt=media&token=4285471c-20ca-4969-9a42-d27393b0d338)

Now the application is drastically faster. The calculations aren't blocking the `main` thread anymore. As the user interacts with the app, the calculations happen in the background. 

## Task 7
-----
Compare your code with the solution: `Solution: Global Superstore 1`.

## Good Luck!
--------
##### Subscribe to our [YouTube Channel](https://www.youtube.com/@RayanSlim087?sub_confirmation=1) and Discover More Valuable Content!