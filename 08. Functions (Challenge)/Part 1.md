# **Rock paper scissors**

![](https://img-c.udemycdn.com/redactor/raw/article_lecture/2025-01-04_03-04-28-72828fadc53aeb47032cc694bb0bf76e.gif)

## Open the challenge
------------------

From `Java Bootcamp Resources`, open the **`Challenge 4`** folder.

![Screen Shot 2022-10-20 at 9.59.00 PM.png](https://img-c.udemycdn.com/redactor/raw/article_lecture/2025-01-04_03-04-29-837ae6fb6f36e27de6854974f95ea98c.png)


## Task 1: See if the user wants to play
-------------------------------------

Use `Scanner` to pick up the user's response.

`>>Let's play Rock Paper Scissors.`

`>>When I say 'shoot', Choose: rock, paper, or scissors.`

`>>`

`>>Are you ready? Write 'yes' if you are`

## Task 2: Set up the game.
------------------------

```
- if the answer is yes:
   -- print: Great!
   -- print: rock - paper - scissors, shoot!
   -- pick up user's choice.
   -- get the computer choice (can be done after task 3).
   -- get the result (can only be done after task 4)
   -- print everything (can only be done after task 5).
- else:
   -- print: Darn, some other time...!
```

Here, the user would enter rock paper or scissors. Using `Scanner`, pick up their choice.

```
- if the answer is yes:
   -- print: Great!
   -- print: rock - paper - scissors, shoot!
   -- pick up user's choice. <----------
   -- get the computer choice (can be done after task 3).
   -- get the result (can only be done after task 4)
   -- print everything (can only be done after task 5).
- else:
   -- print: Darn, some other time...
```
There are more instructions for the if statement. You cannot do them until you finish tasks 3, 4, and 5.

```
- if the answer is yes:
   -- print: Great!
   -- print: rock -- paper -- scissors, shoot!
   -- pick up user's choice.
   -- get the computer choice (can be done after task 3). <------
   -- get the result (can only be done after task 4) <-------
   -- print everything (can only be done after task 5). <--------
- else:
   -- print: Darn, some other time...
```

So, you're left with the `else` block. If the user doesn't enter "yes", print: **Darn, some other time...!**

```
- if the answer is yes:
   -- print: Great!
   -- print: rock -- paper -- scissors, shoot!
   -- pick up user's choice.
   -- get the computer choice (can be done after task 3).
   -- get the result (can only be done after task 4)
   -- print everything (can only be done after task 5).
- else﻿: <---------------
   -- print: Darn, some other time...
```

## **Task 3: Generate a random choice**
------------------------------------

You'll write a function that picks randomly between rock paper scissors.

- Function name:

```java
/**
 * Function name: computerChoice <--------
 * @return a choice (String).
 *
 * Inside the function:
 *   1. Picks a random number between 0 and 2.
 *   2. if 1: return the choice 'rock'
 *      if 2: return the choice 'paper'
 *      if 3: return the choice 'scissors'
 */
```

- Parameters: The function takes no parameters.

- Return type:

```java
/**
 * Function name: computerChoice
 * @return a choice (String). <------
 *
 * Inside the function:
 *   1. Picks a random number between 0 and 2.
 *   2. if 0: return the choice 'rock'
 *      if 1: return the choice 'paper'
 *      if 2: return the choice 'scissors'
 */
```

Inside the function, generate a random number between 0 and 2. Based on the result, return rock, paper or scissors.

```java
/**
 * Function name: computerChoice
 * @return a choice (String).
 *
 * Inside the function: <----------
 *   1. Picks a random number between 0 and 2.
 *   2. if 0: return the choice 'rock'
 *      if 1: return the choice 'paper'
 *      if 2: return the choice 'scissors'
 */
```

Call the function and store the computer choice.

```
- if the answer is yes:
   -- print: Great!
   -- print: rock -- paper -- scissors, shoot!
   -- pick up user's choice.
   -- get the computer choice (can be done after task 3). <------------
   -- get the result (can only be done after task 4)
   -- print everything (can only be done after task 5).
- else:
   -- print: Darn, some other time...
```

## Test your code
--------------

Add two temporary print statements.

```
- if the answer is yes:
   -- print: Great!
   -- print: rock -- paper -- scissors, shoot!
   -- pick up user's choice.
   -- get the computer choice (can only be done after task 3﻿)

     System.out.println("\nYou chose:        " + yourChoice); <---------
     System.out.println("The computer chose: " + computerChoice); <--------

   -- get the result          (can only be done after task 4)
   -- print everything        (can only be done after task 5).
- else:
   -- print: Darn, some other time...
```

The end result should print your choice and the computer's choice.

![](https://img-c.udemycdn.com/redactor/raw/article_lecture/2025-01-04_03-04-29-798ea8c5cfe6765b1105de37149a34fe.gif)

Run it a few more times, and make sure the computer is picking randomly.

## Good luck!
----------
##### **Go From Zero to DevOps Master**: *[Java → Spring Boot → Docker → Kubernetes](https://rslim087a.github.io/zero-devops-roadmap/)*