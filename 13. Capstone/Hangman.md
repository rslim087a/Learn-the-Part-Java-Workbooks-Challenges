# Hangman

Hangman is a word-guessing game. It keeps asking the user to guess characters until:

1.  They guess every character correctly (win).

2.  They miss 6 guesses (loss).

**Example output**

![](https://img-c.udemycdn.com/redactor/raw/article_lecture/2025-01-04_00-09-05-c890d38b4e63a7bdc7bebd6fa9e422ae.gif)

**Why is hangman your capstone project?**
-----------------------------------------

-   It's hard.

-   It will effectively test your ability to apply concepts from Module one. 

-   It will challenge you to get creative and do some research. As a developer, it's important that you practice finding resources online. 

**Downloaded the updated resources.**
-------------------------------------

Your capstone project should contain the following folders:

![](https://img-c.udemycdn.com/redactor/raw/article_lecture/2025-01-04_00-09-05-692716c97b6ef93918dc1323df726ec1.png)

## Tips before you start
-------------------------------

-   If you struggle building hangman, that's good! That means you will learn a lot by trying to solve it.

-  As you're building hangman, you're likely going to get bugs (unexpected results). The best way to fix bugs is to use breakpoints.

3.  You don't have to go through this alone. The [**community**](https://discord.com/invite/uUGJcvzKmn) is a great place to ask questions.

**Instructions**
================

Because this is your capstone project, the instructions are less detailed. Unlike the workbooks and challenges, the instructions will only tell you what the task is. They will not explain nor guide you towards completing the task.

Finally, I encourage you to read all of the instructions before starting your code. I left some helpful hints in the end.

## **a) Download the starter project**
-----------------------------------

In `Java Bootcamp Resources` -> `Module 1` -> `Casptone Project`, you can find `hangman`. **Open** it.

## **b) Choose a random word**
---------------------------

In the starter project, I left you an array of words.

`public static String[] words = {"ant", "baboon", "badger", "bat", "bear","beaver", "camel", "cat", "clam", "cobra", "cougar", "coyote", "crow", "deer", "dog", "donkey", "duck", "eagle", "ferret", "fox", "frog", "goat", "goose", "hawk", "lion", "lizard", "llama", "mole", "monkey", "moose", "mouse", "mule", "newt", "otter", "owl", "panda", "parrot", "pigeon", "python", "rabbit", "ram", "rat", "raven","rhino", "salmon", "seal", "shark", "sheep", "skunk", "sloth", "snake", "spider", "stork", "swan", "tiger", "toad", "trout", "turkey","turtle", "weasel", "whale", "wolf", "wombat", "zebra"};`

Your game must choose a random word from this list of words.

The placeholders '`_`' in your game must reflect the number of characters in that word.

![](https://img-c.udemycdn.com/redactor/raw/article_lecture/2025-01-04_00-09-05-2a8a2e5b3c5b9c0ef7f59907a235c25a.png)

## **c) Show the gallows**
-----------------------

At every turn, you need to show the gallows.

In your starter project, you'll find an array: `String[] gallows`. Each `String` in the array reflects the number of times the user guessed incorrectly.

```java
 public static String[] gallows = {
    "+---+\n" +
    "|   |\n" +
    "    |\n" +
    "    |\n" +   //if the user didn't miss any guesses.
    "    |\n" +
    "    |\n" +
    "=========\n",

    "+---+\n" +
    "|   |\n" +
    "O   |\n" +   //if the user missed one guess.
    "    |\n" +
    "    |\n" +
    "    |\n" +
    "=========\n",

    "+---+\n" +
    "|   |\n" +
    "O   |\n" +    //if the user missed two guesses.
    "|   |\n" +
    "    |\n" +
    "    |\n" +
    "=========\n",

    " +---+\n" +
    " |   |\n" +
    " O   |\n" +   //if the user missed three guesses.
    "/|   |\n" +
    "     |\n" +
    "     |\n" +
    " =========\n",

    " +---+\n" +
    " |   |\n" +
    " O   |\n" +
    "/|\\  |\n"+   //if the user missed four guesses.
    "     |\n" +
    "     |\n" +
    " =========\n",

    " +---+\n" +
    " |   |\n" +
    " O   |\n" +
    "/|\\  |\n" +  //if the user missed five guesses.
    "/    |\n" +
    "     |\n" +
    " =========\n",

    " +---+\n" +
    " |   |\n" +
    " O   |\n" +
    "/|\\  |\n" +   //if the user missed six guesses.
    "/ \\  |\n" +
    "     |\n" +
    " =========\n"};
```

You need to show the gallows at every turn. This should be your output when the user misses two guesses.

![](https://img-c.udemycdn.com/redactor/raw/article_lecture/2025-01-04_00-09-05-6596ead0b07eaed3e006ba0e65476866.png)

## **d) Show the missed guesses**
------------------------------

You need to keep track of every incorrect guess the user made. This helps the user not make the same mistake twice.

![](https://img-c.udemycdn.com/redactor/raw/article_lecture/2025-01-04_00-09-05-58fae46740a8aaf69630ae556853dc83.png)

## **e) Replace placeholders with correct guesses**
------------------------------------------------

When the user guesses correctly, replace the matching placeholders.

![](https://img-c.udemycdn.com/redactor/raw/article_lecture/2025-01-04_00-09-05-9868a525a32823051e499f4c484f053a.png)

## **f) If the user wins:**
------------------------

Stop the game.

**Example output of a winning game:**

![](https://img-c.udemycdn.com/redactor/raw/article_lecture/2025-01-04_00-09-06-4bbb4902928c42bf442a481c8cf61c2a.gif)

## **g) If the user loses:**
-------------------------

Stop the game.

**Example output of a losing game:**

![](https://img-c.udemycdn.com/redactor/raw/article_lecture/2025-01-04_00-09-06-302b4aa0731a9b07700fdf062241b3b9.gif)

## **h) Aesthetics**
-----------------

-   Add one `\n` after printing the word/placeholders.

-   Add two `\n` after printing the misses.

-   Add one `\n` after the guess.

## Possible Design and Hints
-------------------------

**1\. Hints**

Look up how to:

  -   Convert a `String` to an array of characters.

  -   Get the index of a character in a `String`.

  -   Loop through characters in a `String`.

  -   check if two arrays are equal to each other.

 **2\. Possible design**

There are many ways to build Hangman. Here's a possible design for your functions:

-   `randomWord()`: returns a random word from the list of random words.

-   `checkGuess()`: returns `true` if the user guessed a letter from the word correctly.

-   `updatePlaceholders()`: updates the placeholders when the user makes a correct guess.

-   `printPlaceholders()`: prints the placeholders.

-   `printMissedGuesses()`: prints guesses that the user missed.

## Good luck!
----------
##### **Go From Zero to DevOps Master**: *[Java → Spring Boot → Docker → Kubernetes](https://rslim087a.github.io/zero-devops-roadmap/)*