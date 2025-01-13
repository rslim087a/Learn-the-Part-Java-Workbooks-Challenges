# Blackjack (part 2)

In part 1, you wrote the logic for starting the game.

![](https://img-c.udemycdn.com/redactor/raw/article_lecture/2025-01-04_02-17-56-f64571187f7dcded6c963119737241f3.gif)

In part 2, you will write the logic for playing the game. Recall:

-   First, it's the player's turn. The player can decide to **hit** or **stay**.

    -   **hit**: draw another card.

    -   **stay**: do nothing.

-   If the player decides to hit, and their hand value exceeds 21, they go **bust** (lose).

-   Once the player decides to stay, the dealer reveals the hidden card.

-   Then, the dealer must **hit** until their total gets to 17. At 17 points or higher, the dealer's turn ends.

-   You win if your hand value is higher than the dealer's hand.

-   You win if the dealer goes bust (exceeds 21)

-   You lose if the dealer's hand value is higher than yours.

**Final output:**

![](https://img-c.udemycdn.com/redactor/raw/article_lecture/2025-01-04_02-17-57-68a1f51207930ee744ecd8267f6661ee.gif)

## Task 7
------

Make a function that asks the user to hit or stay.

```java
/**
 *  Function name -- hitOrStay
 *  @return (String)
 *
 * Inside the function:
 *   1. Asks the user to hit or stay.
 *
 *   2. If the user doesn't enter "hit" or "stay"
 *       Run a while loop
 *       During each run, println: Please write 'hit' or 'stay'
 *
 *   3. Returns the user's option
 */
```

If the user doesn't enter "hit" or "stay", keep asking them to try again by printing:

`"Please write 'hit' or 'stay'"`

The condition for this while loop is kind of tricky. I recommend using a while loop that runs forever and breaking it when it's appropriate. Test your function by calling it from `main()`.

![](https://img-c.udemycdn.com/redactor/raw/article_lecture/2025-01-04_02-17-57-fa090f9aa33b03d5c7accfb57352cd50.gif)

## Task 8
------

In Task 8, you will keep asking the player to hit or stay. In other words, make a `while` loop that runs forever. Then, call your function inside the `while` loop. Every time the player hits, draw a new card and calculate their new total. Then, print:

- `(new line) You get a (new line) <show new card>`

- ` your new total is <total>`

![](https://img-c.udemycdn.com/redactor/raw/article_lecture/2025-01-04_02-17-57-a4b897c0dc377d305de09269f901826d.gif)

-   Once the player 'stays', break the loop.

![](https://img-c.udemycdn.com/redactor/raw/article_lecture/2025-01-04_02-17-57-03e2d36dcf6cd6dad26729dcbac48c12.gif)

## Task 9
------

While the player is hitting, if they go bust (total exceeds 21) print: `"Bust! Player loses"`. Then, shut down the game with `System.exit(0)` (`System.exit(0)` terminates execution).

![](https://img-c.udemycdn.com/redactor/raw/article_lecture/2025-01-04_02-17-58-b11cc3d38b602519a05ef527974897cb.gif)

## Task 10
-------

After the player chooses to stay, it becomes the dealer's turn. First, reveal the dealer's hidden card.

Print:

- `(new line) Dealer's turn`

- `(new line) The dealer's cards are (new line) <dealer card 1> (new line) and a (new line) <dealer card 2>`

![](https://img-c.udemycdn.com/redactor/raw/article_lecture/2025-01-04_02-17-58-ea836c69c95c61d095ec92a1301e7001.gif)

## Task 11
-------

The dealer must keep "hitting" until their total gets to 17.
Every time the dealer hits, print:

- `(new line) Dealer gets a (new line) <show new card>`

- `(new line) Dealer's total is <dealer's total>`

At 17 points or higher, end the dealer's turn.

![](https://img-c.udemycdn.com/redactor/raw/article_lecture/2025-01-04_02-17-58-bc1020afffe1565237aa3799458b7d38.gif)

## Task 12
-------

If the dealer's total is higher than 21, print: `"Bust! Dealer loses"` and end the game with `System.exit(0)`.

![](https://img-c.udemycdn.com/redactor/raw/article_lecture/2025-01-04_02-17-58-cd1534b9e77c31c0bc391c2a5a68b589.gif)

## Task 13
-------

If at this point, the program didn't terminate, compare the dealer and player's hand values.

-   If the player's hand value is higher, print: `Player wins!`

-   Otherwise, print: `Dealer wins!`.

**Final output:**

![](https://img-c.udemycdn.com/redactor/raw/article_lecture/2025-01-04_02-17-58-eae6a245eba0e4c3f440167680b9b718.gif)

## Good luck!
----------
##### **Go From Zero to DevOps Master**: *[Java → Spring Boot → Docker → Kubernetes](https://rslim087a.github.io/zero-devops-roadmap/)*