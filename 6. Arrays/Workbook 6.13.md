# Workbook 6.13

From the `Java Bootcamp Resources`, open **`Workbook 6.13`**.

![6.13.png](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F22a18d30-cbde-4721-bebb-c202362e306a?alt=media&token=58e5d0d3-933e-41d5-bf73-a103b1abc303)

## Task 1

Create a 2D array of `double` values that can hold **3 rows** and **5 elements** per row.

## Task 2
Populate your 2D array with values from the following table:

![](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F6782067b-3b9e-4155-af8a-6fc5859eb456?alt=media&token=8e7c06a8-994e-498d-b855-ea8a5494b831)

For the sake of exercise, do it the *long* way (indexing elements one by one).
```java
prices[x][x] = 12.99
prices[x][x] = 8.99
//....
``` 

## Task 3

Print the prices of each row using this format:

```java
    System.out.println("Baking: " + prices[0][0] + " " + prices[0][1] + " "...);
```

### Result
![](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F4e6538fb-c766-42cb-b859-d5916065d865?alt=media&token=43e44b2a-d1ff-4dc6-9628-4079e93ed5f3)

## Task 4

Define the array in a single line.

```java
double[][] prices = {
    {12.99, 8.99, 9.99, 10.49, 11.99},
    {0.99, 1.99, 2.49, 1.49, 2.99},
    {8.99, 7.99, 9.49, 9.99, 10.99}
};
```

## Visualizing the Runtime

After you solve this workbook, I still recommend watching the video solution on Udemy.

![13.png](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2Fc3ca5f2d-675b-4aa8-a169-31c5d50c2822?alt=media&token=57073634-441f-41ed-973e-016715695ea8)

It will show you how to visualize the runtime using Visual Studio Code.

----------
##### Subscribe to our [YouTube Channel](https://www.youtube.com/@RayanSlim087?sub_confirmation=1) and Discover More Valuable Content!