# Tic Tac Toe - Part 2

If you made it to part 2, then you were able to achieve this output:

![](https://img-c.udemycdn.com/redactor/raw/article_lecture/2025-01-04_01-03-40-88b01d440cf9704ec8e0b5f51e627563.png)

The next step is to let the players take turns on the board:

![](https://img-c.udemycdn.com/redactor/raw/article_lecture/2025-01-04_01-03-40-d703122b753052611d78646a025ab25c.gif)

Inside the workbook, `Scanner` was declared as a `class` variable. That's because you'll need to access `Scanner` from more than one place inside the class.


```java
public class TicTacToe {

       Scanner scan = new Scanner(System.in);

       public static void main(String[] args) {
          //...
       }
```

Task 3: Taking turns
--------------------

The maximum number of turns is 9. Set up a `for` loop that runs 9 times and prints the counter.

![](https://img-c.udemycdn.com/redactor/raw/article_lecture/2025-01-04_01-03-40-261385ecad2f688870f3ae43b853671c.png)

Each run represents a turn, such that X goes first.

![](https://img-c.udemycdn.com/redactor/raw/article_lecture/2025-01-04_01-03-40-c14ad373a845fc3d3a0edb9aa0263282.png)

**Hint:** `X` plays when the counter is even, whereas `O` plays when the counter is odd. Set up a condition that alternates between printing `Turn: X` and `Turn: O`.

![](https://img-c.udemycdn.com/redactor/raw/article_lecture/2025-01-04_01-03-41-a20279e3b49c1c611a84293f27bc8b76.png)

Task 4: Write a function
------------------------

Write a function that asks the user to choose a spot. As you write the function, call it for each turn.

```java
if (X turn) {
    Task 4: call askUser(board).
} else {
    Task 4: call askUser(board).
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

![](https://img-c.udemycdn.com/redactor/raw/article_lecture/2025-01-04_01-03-41-2a80c830c53f838499e4b86e03b748d0.gif)

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

![](https://img-c.udemycdn.com/redactor/raw/article_lecture/2025-01-04_01-03-41-7d68af9e31c137e460085e1a150abe68.gif)

## Task 4: Revisited
-----------------

We can't let the player pick a spot that's already taken.

![](https://img-c.udemycdn.com/redactor/raw/article_lecture/2025-01-04_01-03-41-e8542e68bdab7b9aa1b3960542a02b6a.gif)

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

![](https://img-c.udemycdn.com/redactor/raw/article_lecture/2025-01-04_01-03-41-23b25767d8bf28c624bd6dfa52d31b66.gif)

The player tried to pick a spot that was already taken (`0 0`). The game prompted them to pick another spot.

Good Luck!
----------
##### Your Path to Cloud-Native Engineering (After Learning Java)
###### 1. Develop Java Web Applications With Spring Boot → [Spring Boot Bootcamp](https://www.udemy.com/course/the-complete-spring-boot-development-bootcamp/?couponCode=SPRING_BOOTCAMP)
###### 2. Containerize and Deploy Web Applications with Docker → [Docker Bootcamp](https://www.udemy.com/course/docker-bootcamp-conquer-docker-with-real-world-projects/?couponCode=DOCKER_BOOTCAMP)
###### 3. Orchestrate Cloud Native Applications with Kubernetes → [Kubernetes Bootcamp](https://kubernetestraining.io/)