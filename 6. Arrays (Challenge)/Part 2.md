# Tic Tac Toe - Part 2

If you made it to part 2, then you were able to achieve this output:

![](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F9e1ba1b4-2425-415a-85e7-29de7165c6ee?alt=media&token=3c371e8a-6329-40bf-907f-3ae233feae0f)

The next step is to let the players take turns on the board:

![](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F10d21001-253e-45f2-9dcb-5ba6c8dbf0f1?alt=media&token=280aadac-6d53-4dba-b804-55ea95245ba1)

Inside the workbook, `Scanner` was declared as a `class` variable. That's because you'll need to access `Scanner` from more than one place inside the class.


```java
public class TicTacToe {

       Scanner scan = new Scanner(System.in);

       public static void main(String[] args) {
          ﻿//...
     ﻿  }
```

Task 3: Taking turns
--------------------

The maximum number of turns is 9. Set up a `for` loop that runs 9 times and prints the counter.

![](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2Fe1f6561d-4f56-45f2-ae01-754503a1f7cf?alt=media&token=036a3546-12b9-4690-9b08-86b30fb780c1)

Each run represents a turn, such that X goes first.

![](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F39b1dee0-77ae-4da3-917d-33aa0ca8399c?alt=media&token=a14cd8ed-96e7-47e4-9823-707c06303027)

**Hint:** `X` plays when the counter is even, whereas `O` plays when the counter is odd. Set up a condition that alternates between printing `Turn: X` and `Turn: O`.

![](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2Fa3b86a73-b641-4f22-a247-38d01ee3f645?alt=media&token=fa61bbba-0a62-4bd6-9125-7f1372c7292c)

Task 4: Write a function
------------------------

Write a function that asks the user to choose a spot. As you write the function, call it for each turn.

```java
if (﻿X turn) {
    Task 4﻿: call askUser﻿(board)﻿.
} else {
    Task 4﻿: call askUser﻿(board)﻿.
}
```

1\. Function name: The name of the function is `askUser()`. It lets the player choose a spot on the board.

```java
/**
 * Function name -- askUser <-------
 * @param board (char[][] board)
 * @return spot (int[])
 *
 * Inside the function
 *     1. Asks the user: - pick the row and column:
 *     2. If the spot is taken, ask the user to choose again.
 *     3. Return the row and column in an int[] array.
 *
 */
```

2\. Parameters: The function takes one parameter: `char[][] board`.

```java
/**
 * Function name -- askUser
 * @param board (char[][] board) <--------
 * @return spot (int[])
 *
 * Inside the function
 *  1. Asks the user: - pick the row and column:
 *  2. If the spot is taken, ask the user to choose again.
 *  3. Return the row and column in an int[] array.
 *
 */
```

**3**. Return value: The function returns the spot. It will be an array that holds two numbers: the row and column.

```java
/**
 * Function name -- askUser
 * @param board (char[][] board)
 * @return spot (int[]) <-------
 *
 * Inside the function
 *  1. Asks the user: - pick the row and column:
 *  2. If the spot is taken, ask the user to choose again.
 *  3. Return the row and column in an int[] array.
 *
 */
```

Inside the function:

-   Ask the player to pick a spot on the grid and return it

```java
/**
 * Function name -- askUser
 * @param board (char[][] board)
 * @return spot (int[])
 *
 * Inside the function <---
 *  1. Asks the user: - pick a row and column number: <---
 *  2. If the spot is taken, ask the user to choose again.
 *  3. Return the row and column in an int[] array. <---
 *
 */
```

![](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2Fb09715c0-efc6-46a7-b31d-dde1da1f4ea0?alt=media&token=30fdd100-9846-4a59-915f-6e87db26c580)

The user will write their numbers **beside** each question. Then, store both numbers in the `int[]` array.

Ignore the second step for now. You can move on to task 5.

```java
/**
 * Function name -- askUser
 * @param board (char[][] board)
 * @return spot (int[])
 *
 * Inside the function
 *  1. Asks the user: - pick a row and column number:
 *
 *     *****  Ignore this step for now *****
 *  2. If the spot is taken, ask the user to choose again.
 *     *****  Ignore this step for now *****

 *  3. Return the row and column in an int[] array.
 *
 */
```

## Task 5: Populate the board
--------------------------

The function call returns the player's spot. Use that return value to index the board and populate it. Then, print the board:

![](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2Fed6c8f02-a925-43f9-bcff-b10263ce51cf?alt=media&token=3913fad2-893e-485e-99cf-de0660bf169c)

## Task 4: Revisited
-----------------

We can't let the player pick a spot that's already taken.

![](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F39433009-5560-47c2-87d6-0b1272616a6c?alt=media&token=da1f7e39-ff72-46a4-958f-15c82c9ac18d)

Inside the function:

-   Check if the spot on the board is taken. If so, prompt the user to choose again.

```java
/**
 * Function name -- askUser
 * @param board (char[][] board)
 * @return spot (int[])
 *
 * Inside the function <------
 *  1. Asks the user: - pick a row and column number:
 *  2. If the spot is taken, ask the user to choose again. <----
 *  3. Return the row and column in an int[] array. 
 *
 */
```

Hint: use a `while` loop! **Final output:**

![](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F7834d5bb-ad3a-45a1-961e-690c00f44a0c?alt=media&token=46e789e9-bb12-40e4-928c-4e31cf9c0510)

The player tried to pick a spot that was already taken (`0 0`). The game prompted them to pick another spot.

Good Luck!
----------
##### Subscribe to our [YouTube Channel](https://www.youtube.com/@RayanSlim087?sub_confirmation=1) and Discover More Valuable Content!