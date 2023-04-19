# Hangman

Hangman is a word-guessing game. It keeps asking the user to guess characters until:

1.  They guess every character correctly (win).

2.  They miss 6 guesses (loss).

**Example output**

![](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2Fd8b52dae-3a97-4c72-9add-b07bf7aa1a14?alt=media&token=b24fd192-87ec-4d76-89b5-d4e804f99811)

**Why is hangman your capstone project?**
-----------------------------------------

-   It's hard.

-   It will effectively test your ability to apply concepts from Module one. 

-   It will challenge you to get creative and do some research. As a developer, it's important that you practice finding resources online. 

**Downloaded the updated resources.**
-------------------------------------

Your capstone project should contain the following folders:

![](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2Fff69f142-8e9d-442c-bb4a-7850cfd047ef?alt=media&token=d4fd607e-cd02-4379-bb57-c8bc44c8fe68)

If you're missing one of the folders, download the updated resources from the [**Github Repo**](https://github.com/rslim087a/Java-Bootcamp-Resources).

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

![](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F0b84a717-bb03-4339-9181-643d905e3a7d?alt=media&token=bbc2ad5a-9a16-419f-ba60-5a2acb5b0a6d)

## **c) Show the gallows**
-----------------------

At every turn, you need to show the gallows.

In your starter project, you'll find an array: `String[] gallows`. Each `String` in the array reflects the number of times the user guessed incorrectly.

```java
 public static String[﻿] gallows = {
    "+---+\n" +
    "|   |\n" +
    "    |\n" +
    "    |\n" +   //if the user didn't miss any guesses.
    "    |\n" +
    "    |\n" +
    "=========\n"﻿,

    "+---+\n" +
    "|   |\n" +
    "O   |\n" +   //if the user missed one guess.
    "    |\n" +
    "    |\n" +
    "    |\n" +
    "=========\n"﻿,

    "+---+\n" +
    "|   |\n" +
    "O   |\n" +    //if the user missed two guesses.
    "|   |\n" +
    "    |\n" +
    "    |\n" +
    "=========\n"﻿,

    " +---+\n" +
    " |   |\n" +
    " O   |\n" +   //if the user missed three guesses.
    "/|   |\n" +
    "     |\n" +
    "     |\n" +
    " =========\n"﻿,

    " +---+\n" +
    " |   |\n" +
    " O   |\n" +
    "/|\\  |\n"﻿+   //if the user missed four guesses.
    "     |\n" +
    "     |\n" +
    " =========\n"﻿,

    " +---+\n" +
    " |   |\n" +
    " O   |\n" +
    "/|\\  |\n" +  //if the user missed five guesses.
    "/    |\n" +
    "     |\n" +
    " =========\n"﻿,

    " +---+\n" +
    " |   |\n" +
    " O   |\n" +
    "/|\\  |\n" +   //if the user missed six guesses.
    "/ \\  |\n" +
    "     |\n" +
    " =========\n"﻿}﻿;
```

You need to show the gallows at every turn. This should be your output when the user misses two guesses.

![](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F50c85efb-9154-4b9c-a4cb-8b5fdc8428c5?alt=media&token=4d7d951d-74fd-4f3d-8b97-fe7bfc42a2af)

## **d) Show the missed guesses**
------------------------------

You need to keep track of every incorrect guess the user made. This helps the user not make the same mistake twice.

![](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2Fa9d499b3-f8d4-4537-a101-a277c2c4bc9d?alt=media&token=3b80e0f0-9abe-4d47-a0c0-d1f9e6803cdf)

## **e) Replace placeholders with correct guesses**
------------------------------------------------

When the user guesses correctly, replace the matching placeholders.

![](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F0fa8f2d0-6d8f-4d7a-98a3-143da5d0c7a2?alt=media&token=43d50f19-5084-4f93-91a1-7789f289dd23)

## **f) If the user wins:**
------------------------

Stop the game.

**Example output of a winning game:**

![](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2Fc452b407-23a8-4398-819b-ab380267e275?alt=media&token=1c0ddf2d-7ebf-42e0-b23e-5f81947583f0)

## **g) If the user loses:**
-------------------------

Stop the game.

**Example output of a losing game:**

![](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2Fa4f85720-1398-443d-bd3e-5dc67fd10a57?alt=media&token=5bde33a5-ee9f-4a8a-87bd-415f4b00c3d2)

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
##### Subscribe to our [YouTube Channel](https://www.youtube.com/@RayanSlim087?sub_confirmation=1) and Discover More Valuable Content!