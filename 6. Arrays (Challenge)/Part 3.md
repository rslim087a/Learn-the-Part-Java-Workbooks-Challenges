# Tic Tac Toe -- Part 3

If you made it here, then your game lets a player pick a spot on the board:

![](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2Fcd16f8f8-3534-4caa-8b2d-29e9aff4caf3?alt=media&token=d05bb1e2-bb47-4c02-998c-22d2c71500ce)

It also doesn't let them pick a spot that's already taken.

![](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2Fc9dff6ad-e8f4-4a7a-919f-eea057008c52?alt=media&token=2f5e190b-89df-4d46-b59c-bd1b368e2953)

Onto the most exciting part! You will write code that determines the winner.

The `checkWin()` function
-------------------------

This function has to check for a win in every row:

![](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F624c34d7-6248-449a-8833-8996fe970907?alt=media&token=5677380f-b534-4203-94fc-4a0db35f9ce6)

every column:

![](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F455e475b-0681-4a2b-a024-15f957f77674?alt=media&token=193247f8-6694-41b2-a3e6-442ee611bd58)

the left diagonal:

![](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F1c536df1-14a5-4394-8292-100448ace363?alt=media&token=0f72e92d-4ffe-4dbc-87f6-f5657309caba)

and the right diagonal:

![](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F36a66a47-bafb-4fa8-b154-3aa779ddaf1d?alt=media&token=e66ed809-1df0-491b-a36c-0b6143321efe)

## Task 6: Write the function
--------------------------

1. Create a function called checkWin.

```java
/**
 * Function name - checkWin <-------
 * @param board (char[][])
 * @return count (int)
 *
 * Inside the function:
 *   1. checkRows(): Check every row for a straight X/O  (Task 7)
 *   2. checkColumns(): Check every column for a straight X/O  (Task 8)
 *   3. checkLeft(): Check the left diagonal for a straight X/O  (Task 9).
 *   4. checkRight(): Check the right diagonal for a straight X/O  (Task 10).
 */
```

2. Parameters: The function takes one parameter: char[][] board.

```java
/**
 * Function name - checkWin
 * @param board (char[][]) <--------
 * @return count (int)
 *
 * Inside the function:
 *   1. checkRows(): Check every row for a straight X/O  (Task 7)
 *   2. checkColumns(): Check every column for a straight X/O  (Task 8)
 *   3. checkLeft(): Check the left diagonal for a straight X/O  (Task 9).
 *   4. checkRight(): Check the right diagonal for a straight X/O  (Task 10).
 */
```

**3**. Return value: The function returns a count.

```java
/**
 * Function name - checkWin
 * @param board (char[][])
 * @return count (int) <----------
 *
 * Inside the function:
 *   1. checkRows(): Check every row for a straight X/O  (Task 7)
 *   2. checkColumns(): Check every column for a straight X/O  (Task 8)
 *   3. checkLeft(): Check the left diagonal for a straight X/O  (Task 9).
 *   4. checkRight(): Check the right diagonal for a straight X/O  (Task 10).
 */
```

Tasks 7 - 10 are function calls that return an int. 
```java
/**
 * Function name - checkWin
 * @param board (char[][])
 * @return count (int)
 *
 * Inside the function:
 *   1. checkRows(): Check every row for a straight X/O  (Task 7) <————
 *   2. checkColumns(): Check every column for a straight X/O  (Task 8) <————
 *   3. checkLeft(): Check the left diagonal for a straight X/O  (Task 9). <————
 *   4. checkRight(): Check the right diagonal for a straight X/O  (Task 10). <————
 */
```
Copy their definitions inside your class.

```java
public static int checkRows(char[][] board) {
    int count = 0;
    return count;
}


public static int checkColumns(char[][] board) {
    int count = 0;
    return count;
}


public static int checkLeft(char[][] board) {
    int count = 0;
    return count;
}


public static int checkRight(char[][] board) {
    int count = 0;
    return count;
}
```

Call each function inside checkWin().

```java
public static int checkWin(char[][] board) {    
    int rows = checkRows(board); 
    
    // Math.abs returns the absolute value of a given number, removing any negative sign. 
    if (Math.abs(rows) == 3) return rows; // If the block of code consists of only one line, you can omit the curly braces.
    
    int columns = checkColumns(board);
    if (Math.abs(columns) == 3) return columns;  
    
    int leftDiagonal = checkLeft(board);
    if (Math.abs(leftDiagonal) == 3) return leftDiagonal; 
    
    int rightDiagonal = checkRight(board);
    if (Math.abs(rightDiagonal) == 3) return rightDiagonal;
    
}
```

## Task 7


Call `checkWin` from your for loop in main. The loop should break if the returned count is 3 or -3.
```
     if (returned count == 3) {
        // 1. print: X wins
        // 2. break the loop
      } else if (returned count == -3) {
        // 1. print: O wins
        // 2. break the loop
       }
```

## Task 8: Checking every row
--------------------------

Tasks 7 - 10 are function calls that receive and return `int`.

```java
/**
 * Function name - checkWin
 * @param board (char[][])
 * @return count (int)
 *
 * Inside the function:
 *   1. checkRows(): Check every row for a straight X/O  (Task 7) <——
 *   2. checkColumns(): Check every column for a straight X/O  (Task 8)
 *   3. checkLeft(): Check the left diagonal for a straight X/O  (Task 9).
 *   4. checkRight(): Check the right diagonal for a straight X/O  (Task 10).
 */
```

`checkRows():` will check every row for a straight X or straight O:
 - In each row, add 1 to `count` if there's an X. 
 - Subtract 1 if there's an O.

![](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2Fa6bf9e15-3738-466c-816a-dc7beefddf3b?alt=media&token=76aeac14-202e-4cca-b948-e58755109d84)

If `count` isn't 3 or -3, reset it and move to the next row.

![](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F44d2d787-bf89-4fc1-b88f-4733fc685843?alt=media&token=ad3c800f-fbcb-476f-b093-cf89678e54e3)

A count of 3 means X won (conversely, a count of -3 means O won).

![](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F22a7348f-bb85-4558-bb03-611aeb85517b?alt=media&token=e9d1d70b-afbc-4b76-b93a-85f6f0cfdc0e)

If `count` is 3 **OR** -3, break the `checkWin` function by returning `count`.

![](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F9cad9f3a-2133-405f-8a82-542389285633?alt=media&token=a1441bc7-77e1-4b63-baf6-1d78a0bd401b)

Notice that the game stops after a win.

## Task 9: Checking every column
-----------------------------

```java
/**
 * Function name - checkWin
 * @param board (char[][])
 * @return count (int)
 *
 * Inside the function:
 *   1. checkRows(): Check every row for a straight X/O  (Task 7) 
 *   2. checkColumns(): Check every column for a straight X/O  (Task 8) <———
 *   3. checkLeft(): Check the left diagonal for a straight X/O  (Task 9).
 *   4. checkRight(): Check the right diagonal for a straight X/O  (Task 10).
 */
```
`checkColumns()`:  will check every column for a straight X or straight O:
-   The outer loop picks a column. The inner loop will index each row for that column.
-   When looking at the image below, think of `i` and `j`.

![](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2Fab7708fb-fde2-4c0b-b431-1c8f076360dd?alt=media&token=323ef4d3-5a85-4000-9be4-266c7290f50f)

A player wins if one of the columns results in a `count` of 3 or -3:

![](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F37b30b0f-cbc2-41ef-a119-ff62c51bc0fe?alt=media&token=d01fef80-a188-4225-9f12-4a2711c488e3)

Test every column before you move to Task 9.

## Task 10: Checking the left diagonal
----------------------------------

If none of the rows or columns result in a count of 3 or -3, reset the count to 0.

```java
/**
 * Function name - checkWin
 * @param board (char[][])
 * @return count (int)
 *
 * Inside the function:
 *   1. checkRows(): Check every row for a straight X/O  (Task 7) 
 *   2. checkColumns(): Check every column for a straight X/O  (Task 8) 
 *   3. checkLeft(): Check the left diagonal for a straight X/O  (Task 9). <———
 *   4. checkRight(): Check the right diagonal for a straight X/O  (Task 10).
 */
```
`checkLeft()`: will check the left diagonal for a straight X or O:
-   Do you see a pattern in the indices?
-   You don't need a nested loop. Use a single `for` loop.

![](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2Fa300009e-ddb2-497a-a78a-bb31bc4ee5b6?alt=media&token=cbcba0e8-d872-4ca2-a0b9-7c451332f38b)

**Output**:

![](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F0a037bcc-3cae-4344-8347-80f1d2a86910?alt=media&token=9c96feb4-d9be-423e-9668-fbce66a5ea27)

## Task 11: Checking the right diagonal
------------------------------------

If none of the rows, columns, or left diagonal result in a win, reset the count to 0.

Now, check the right diagonal for a straight X or O.

```java
/**
 * Function name - checkWin
 * @param board (char[][])
 * @return count (int)
 *
 * Inside the function:
 *   1. checkRows(): Check every row for a straight X/O  (Task 7) 
 *   2. checkColumns(): Check every column for a straight X/O  (Task 8) 
 *   3. checkLeft(): Check the left diagonal for a straight X/O  (Task 9). 
 *   4. checkRight(): Check the right diagonal for a straight X/O  (Task 10). <———
 */
```

`checkRight():` will check the right diagonal for a straight X or O:

-   You don't need a nested loop. Use a single `for` loop.
-   The pattern here is a bit tricky:

    -   2 - **0** = **2**
    -   2 - **1** = **1**
    -   2 - **2** = **0**

Compare the bolded numbers from the hint to the indices below:

![](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F08641a78-c14b-44f7-97e4-59d3f55eba65?alt=media&token=d9d090bb-f92b-42f9-bbd0-dd0de185dd9c)

**Output**:

![](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2Fc5a8d128-408b-43de-91c8-53bdfe8a0000?alt=media&token=141058d6-a1ee-4f71-bef7-22c47ccb40a3)

## Task 11: What if it's a tie?
----------------------------

If the game goes all nine turns and nobody wins, print: "it's a tie!".

## Task 12: Test your code!
------------------------

Test your code for every type of win:

-   straight row

-   straight column

-   left diagonal

-   right diagonal.

Test each case for X and O. Also, see if your code works in the event of a tie.

If everything works, you have my sincere congratulations! Tic tac toe is not an easy project, and going through this challenge is a strong testament to your growth.

Good Luck!
----------
##### Subscribe to our [YouTube Channel](https://www.youtube.com/@RayanSlim087?sub_confirmation=1) and Discover More Valuable Content!
