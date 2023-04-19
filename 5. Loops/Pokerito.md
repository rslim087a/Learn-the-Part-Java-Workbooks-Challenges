# Pokerito (it's almost Poker!)

Pokerito is like Poker, but the rules are a lot simpler.

-   The dealer will give you one card

![](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2Fd9be7ac9-f456-42df-9e7c-248d17831daa?alt=media&token=3e607649-6193-42c9-b04c-af486e93c260)

-   and the computer one card.

![](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2Fd345c805-5042-4a89-801c-9a92f9067f17?alt=media&token=42f7795e-a14b-4bf0-b0d0-100a5c6c1b49)

-   Then, the dealer will draw five cards (the river).

![](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F80881562-ad47-4fa1-a428-209da223e4de?alt=media&token=b0910eec-327c-4428-9868-f59e3998152c)

-   The player with the most river matches wins. If the matches are equal, everyone's a winner!

**Final Output:**

![](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2Faccfda26-38de-48ec-b322-10c950820536?alt=media&token=826227de-4bd5-4588-83be-44f4f404105c)

Launch the workbook
-------------------

From `Java Bootcamp Resources` -> `Module 1` -> `5. Loops`, open Pokerito.

## Task 1
------


Create the function: `randomCard`.

```java
    /**
     * Function name -- randomCard
     * @return (String)
     *
     * Inside the function:
     *   1. Gets a random number between 1 and 13.
     *   2. Returns a card that matches the random number.
     */
```

Inside your folder, there's a `cards.txt` file. There, you can find all the cards in `String` format.

```
           1﻿:      "   _____\n"﻿+
                   "  |A _  |\n"﻿+
                   "  | ( ) |\n"﻿+
                   "  |(_'_)|\n"﻿+
                   "  |  |  |\n"﻿+
                   "  |____V|\n"﻿;
           ...
```

There are 13 cards that go from Ace (**1**) to King (**13**). Use `switch` to return a card that matches the random number.

```java
    /**
     * Function name -- randomCard
     * @return (String)
     *
     * Inside the function:
     *   1. Gets a random number between 1 and 13.
     *   2. Returns a card that matches the random number. <-----
     */
```

Call the function and print the return value.

![](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F6ec7e022-3457-4ee9-8cd3-4eec1f8c531c?alt=media&token=fb25b28b-e83a-433f-b03c-630b786e6f9e)

Keep running your function. If it gives you a random card each time, then you're good to go!

## Task 2
------

Start the game by explaining the rules.

`Let's play Pokerito. Type anything when you're ready.`

`It's like Poker, but a lot simpler.`

` - There are two players, you and the computer.`

` - The dealer will give each player one card.`

` - Then, the dealer will draw five cards (the river)`

` - The player with the most river matches wins!`

` - If the matches are equal, everyone's a winner!`

` - Ready? Type anything if you are.`

![](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F6f3dfdbd-9c2c-499e-8d97-9951f10407e6?alt=media&token=fa11ab3d-c2f6-4f48-bcb4-86a4807930ee)

## Task 3
------

Once the user "is ready", present them with a card. Also, show them the computer's card.

```
       /*Task 3: Present the user with a card

         Here's your card:
         <show card>
         <new line>
         Here's the computer's card:
         <show computer's card>

       */
```

![](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F411f4751-308d-4c58-9f65-9750b46f1838?alt=media&token=62df56f0-c31a-4f65-b72a-02ebd482a725)

## Task 4
------

Print: `Now, the dealer will draw five cards. Press enter to continue.`

Use a `for` loop to draw a card every time the user presses enter. You must draw a total of 5 cards and print the order of each one.

![](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F4495930a-560f-4dc9-b65e-67db79c4d1eb?alt=media&token=b86f229b-b09e-4548-bcd1-42f513f8de23)

## Task 5
------

1.  Count how many times your card matches with the river.

2.  Count how many times the computer's card matches with the river.

Then:

-   print: `Your number of matches: <yourMatches>`

-   print: `Computer number of matches: <computerMatches>`

If you have more matches, print: `You win!`. If the computer has more matches, print: `The computer wins!`. If the matches are equal, print: `everyone wins!`.

**Example:**
```
Here's your card: 
    _____ 
   |﻿9    |
   |o o o|
   |o o o|
   |o o o|
   |____9|

Here's the computer's card: 
    _____ 
   |7    |
   | o o |
 ﻿  |o o o|
   | o o |
   |____7|
```

```
Now, the dealer will draw five cards. Press enter to continue﻿.
```

```
Card 1

    _____ 
   |7    |
   ﻿| o o |
   |o o o|
   | o o |
   |____7|

Card 2

    _____ 
   ﻿|6    |
   | o o |
   | o o |
   | o o |
   |____6|

Card 3

    _____ 
 ﻿  |6    |
   | o o |
   | o o |
   | o o |
   |____6|

Card 4

    _____ 
   |7    |
   ﻿| o o |
   |o o o|
   | o o |
   |____7|

Card 5

    _____
   |2 ﻿   |
   |  o  |
   |     |
   |  o  |
   |____Z|
```

```
Your number of matches: 0
Computer number of matches: 2
Computer wins!
```

## Good luck!
----------
##### Subscribe to our [YouTube Channel](https://www.youtube.com/@RayanSlim087?sub_confirmation=1) and Discover More Valuable Content!