# Workbook 6.14

From the `Java Bootcamp Resources`, launch **`Workbook 6.14`**.

![Untitled4.png](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F0be59cd8-2530-47bf-a94d-e64d6b524dbd?alt=media&token=04fa90fd-74ee-4efa-9081-6c6b4f9d3546)

## Task 1

This function returns a random number between 0 and 99. Copy it into your class.

```java
    public static int randomNumber() {
        double randomNumber = Math.random()*100;
        return (int)randomNumber;
    }
```

## Task 2

Write a function that prints the contents of an `int[][]` array.

```java
/**
 * Function name: print2DArray
 * @param array ( int[][] )
 *
 * 
 * 
 *       
 *      
 *      
 */
```
The function uses a nested loop. The inner loop prints each row in one line.

```java
/**
 * Function name: print2DArray
 * @param array ( int[][] )
 *
 * Inside the function:
 *  1. Nested loop:
 *      - Inner Loop: System.out.print(array[i][j] + " ");
 *      
 */
```

After the inner loop runs to completion, print a new line. 
```java
/**
 * Function name: print2DArray
 * @param array ( int[][] )
 *
 * Inside the function:
 *  1. Nested loop:
 *      - Inner Loop: System.out.print(array[i][j] + " ");
 *      - After the Inner Loop Completes: System.out.print("\n");
 */
```

Call `print2DArray` for the following array.
```java
int[][] array = {
    {48, 56, 56, 76, 0, 81, 51, 81, 99, 70},
    {38, 52, 73, 6, 10, 56, 1, 71, 47, 9},
    {85, 35, 47, 98, 91, 25, 69, 52, 2, 93}
};
```
### Result
![](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2Fbd0137b7-9cfb-4754-99aa-f29d693674c0?alt=media&token=684e824a-1ddd-488e-8ed9-a2055166cd2b)

Delete the array if you achieve the result.

## Task 3

Create a 2D array with **100 rows** and **10 columns**. Then call `print2DArray`.

![](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F20005e86-d942-4c64-83f3-16dca224a1ac?alt=media&token=07731bcd-1d78-44ea-aac9-482be5031085)

## Task 4

Use a nested loop to populate the array with random numbers before calling: `print2DArray`.

![](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2Fc8de9e35-1104-4e7c-86bb-d602fa547168?alt=media&token=e7d53e94-da88-4fca-8d4b-8818cab10849)

## Visualizing the Runtime

After you solve this workbook, I still recommend watching the video solution on Udemy.

![14.png](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F51dc4e34-50eb-485c-8f10-79eadcb3329c?alt=media&token=3e38268e-b361-4224-8c86-6480d5b02a46)

It will show you how to visualize the runtime using Visual Studio Code.

----------
##### Subscribe to our [YouTube Channel](https://www.youtube.com/@RayanSlim087?sub_confirmation=1) and Discover More Valuable Content!