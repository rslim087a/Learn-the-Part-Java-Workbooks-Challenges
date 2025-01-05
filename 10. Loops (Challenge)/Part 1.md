# Blackjack

Blackjack is the most popular table game at casinos. You're going to build a simple version of Blackjack.

**Part 1: Starting the game**

-   In Blackjack, the player plays against the dealer.

-   The dealer gives the player two cards faceup.

-   The dealer also starts with two cards. But, only one of the dealer's cards is faceup. The other is facedown.

![](https://img-c.udemycdn.com/redactor/raw/article_lecture/2025-01-04_02-14-07-e2cd2da094cfeb1f9b86aec53075080d.gif)

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

![](https://img-c.udemycdn.com/redactor/raw/article_lecture/2025-01-04_02-14-07-146f4d5526e2d7b928888087b8f64cdc.gif)

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

![](https://img-c.udemycdn.com/redactor/raw/article_lecture/2025-01-04_02-14-07-e98ebd84f5280a9070109f0a48b2a327.gif)

## Task 4
------

When the game starts, the dealer will give you two cards faceup. Get the code to deal you two random cards and print them:

```
-- Get two random cards.
-- Print them: (﻿new line﻿) You get a (﻿new line﻿) <random card> and a <random card>
```

![](https://img-c.udemycdn.com/redactor/raw/article_lecture/2025-01-04_02-14-08-4c04de312b2df64b72dce3d83cac1f89.gif)

## Task 5
------

After you print your cards, print the hand value. The hand value is the sum of your card values.

```java
your total is: <hand value>
```

In blackjack, the face cards (Jack, Queen, and King) have values of 10.

**Hint**: look into `Math.min`.

**Example output:**

![](https://img-c.udemycdn.com/redactor/raw/article_lecture/2025-01-04_02-14-08-6f1f435b4c2efd59b0bc0290b882b652.gif)

## Task 6
------

The dealer gets two cards as well. Print the dealer's first card, and print the next one facedown. You can find the `String` for a facedown card being returned from a function called: `faceDown()`.

```
1. print:

 (new line) The dealer shows (new line) <random card> and
 has a card facing down (new line) <facedown card>;

2. print:
 (new line) The dealer's total is hidden
```

That's all for part 1. Your final output should appear as follows:

![](https://img-c.udemycdn.com/redactor/raw/article_lecture/2025-01-04_02-14-08-d8db3808d87937f2272208633a0b385e.gif)

## Good luck!
----------
##### Your Path to Cloud-Native Engineering (After Learning Java)
###### 1. Develop Java Web Applications With Spring Boot → [Spring Boot Bootcamp](https://www.udemy.com/course/the-complete-spring-boot-development-bootcamp/?couponCode=SPRING_BOOTCAMP)
###### 2. Containerize and Deploy Web Applications with Docker → [Docker Bootcamp](https://www.udemy.com/course/docker-bootcamp-conquer-docker-with-real-world-projects/?couponCode=DOCKER_BOOTCAMP)
###### 3. Orchestrate Cloud Native Applications with Kubernetes → [Kubernetes Bootcamp](https://kubernetestraining.io/)