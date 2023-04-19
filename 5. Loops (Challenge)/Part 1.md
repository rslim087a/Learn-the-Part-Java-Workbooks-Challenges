# Blackjack

Blackjack is the most popular table game at casinos. You're going to build a simple version of Blackjack.

**Part 1: Starting the game**

-   In Blackjack, the player plays against the dealer.

-   The dealer gives the player two cards faceup.

-   The dealer also starts with two cards. But, only one of the dealer's cards is faceup. The other is facedown.

![](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F49d4c97e-1a8e-4a9a-bd2a-030102212f91?alt=media&token=727ec955-62e1-4cfc-b074-07022eec4730)

**Part 2: During the game**

-   First, it's the player's turn. The player can decide to **hit** or **stay**.

    -   **hit**: draw another card.

    -   **stay**: do nothing.

-   If the player decides to hit, and their hand value exceeds 21, they go **bust** (lose).

-   Once the player decides to stay, the dealer reveals the hidden card.

-   Then, the dealer must **hit** until their cards total up to 17. At 17 points or higher, the dealer must stay.

-   You win if your hand value is higher than the dealer's hand.

-   You win if the dealer goes bust (exceeds 21)

-   You lose if the dealer's hand value is higher than yours.

**Full output:**

![](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2Fc81f4e58-142d-4747-8a98-c363480dcf07?alt=media&token=eaedf962-f3aa-4089-9f36-213562e1158a)

## Launch the challenge
--------------------

From `Java Bootcamp Resources` -> `Module 1` -> `5. Loops`, open `Challenge 5`.

## Task 1
------
Define the `drawRandomCard` function.

```java
    /**
     * Function name -- drawRandomCard
     * @return (int)
     *
     * Inside the function:
     *   1. Gets a random number between 1 and 13.
     *   2. Returns a card.
     */
```

## Task 2
------

Make a function that receives a card number and returns the `String` drawing. You can grab the cards from `cards.txt`. Use the doc comment inside the workbook as a guide.

## Task 3
------

Write code that waits for the user to press enter.

![](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F27a6512b-c2ca-4541-919f-1bfb6ef57539?alt=media&token=1896e076-78ba-4813-9a3d-4247a1ba85b1)

## Task 4
------

When the game starts, the dealer will give you two cards faceup. Get the code to deal you two random cards and print them:

```
-- Get two random cards.
-- Print them: (﻿new line﻿) You get a (﻿new line﻿) <random card> and a <random card>
```

![](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F7b49ec9b-774c-43cc-8962-5788a71d5df9?alt=media&token=75ccec2e-370f-432b-874c-dad2148c8f3b)

## Task 5
------

After you print your cards, print the hand value. The hand value is the sum of your card values.

```java
your total is: <hand value>
```

In blackjack, the face cards (Jack, Queen, and King) have values of 10.

**Hint**: look into `Math.min`.

**Example output:**

![](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2Ff2f3655b-bbe9-4d1b-9657-51dbbf4549e3?alt=media&token=4d6b8516-8860-4931-b0f0-6741b7eeed6d)

## Task 6
------

The dealer gets two cards as well. Print the dealer's first card, and print the next one facedown. You can find the `String` for a facedown card being returned from a function called: `faceDown()`.

```
1. print:

 (﻿new line﻿) The dealer shows (﻿new line﻿) <random card> and
 has a card facing down (﻿new line﻿) <facedown card>﻿;

2. print:
 (﻿new line﻿) The dealer's total is hidden
```

That's all for part 1. Your final output should appear as follows:

![](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F427749b6-4fd7-4cf3-824a-c72d6a28640c?alt=media&token=826ac8b9-47c9-42f5-9c31-f31312350f39)

## Good luck!
----------
##### Subscribe to our [YouTube Channel](https://www.youtube.com/@RayanSlim087?sub_confirmation=1) and Discover More Valuable Content!