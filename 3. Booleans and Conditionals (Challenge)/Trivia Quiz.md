# Trivia Quiz

The quiz will ask multiple-choice questions about common trivia. It tracks the user's answers and prints their final score.

![](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2Feea146f3-f410-495d-904e-2e05917bad8b?alt=media&token=7b5decbe-64ea-4deb-8420-795e0ff871b9)

## Open the challenge

From `Java Bootcamp Resources`, launch `Challenge 3`.

![Screen Shot 2022-10-16 at 7.18.41 PM.png](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2Fb13da05c-82d6-4d42-84c1-734dc0a4dda9?alt=media&token=6e3254de-84a6-4761-9377-3671d5d4f594)

## 1\. Store each answer.
----------------------

Add code that picks up the user's answer. Use the comments to guide your code.

```
        System.out.﻿println﻿(﻿"1. Which country held the 2016 Summer Olympics?"﻿)﻿;
        System.out.﻿println﻿(﻿"\ta) China\n\tb) Ireland\n\tc) Brazil\n\td) Italy\n"﻿)﻿;
        //store ans﻿wer 1
```


## 2\. Check each answer.
----------------------

The correct answers are:

-   Question 1: **c**

-   Question 2: **a**

-   Question 3: **d**

-   Question 4: **a** OR **b** is correct

Update the user's score by 5 points for each correct answer.

## 3\. Print a final message.
--------------------------

If `score` is 15 or higher, `print`:

> Wow, you know your stuff!

If `score` is < than 15 but greater than or equal to 5:

> Not bad!

otherwise:

> better luck next time.

## Run your code.
--------------

Enter the correct answer to each question.

-   Question 1: **c**

-   Question 2: **a**

-   Question 3: **d**

-   Question 4: **a** OR **b**.


```
1. Which country held the 2016 Summer Olympics?
    	a) China
    	b) Ireland
    	c) Brazil
    	d) Italy
c

2. Which planet is the hottest?
    	a) Venus
    	b) Saturn
    	c) Mercury
    	d) Mars
a

3. What is the rarest blood type?
    	a) O
    	b) A
    	c) B
    	d) AB-Negative

d

4. Which one of these characters is friends with Harry Potter?
    	a) Ron Weasley
    	b) Hermione Granger
    	c) Draco Malfoy

a

Your final score is: 20/20
Wow, you know your stuff!
```

## Running test cases
------------------

**Test case 1**

Enter the following answers:

-   Question 1: **b**

-   Question 2: **c**

-   Question 3: **d**

-   Question 4: **c**

Your output should reflect a score of 5/20. It should also print:

> Not bad!

**Test case 2**

Enter the wrong answers to each question:

-   Question 1: **b**

-   Question 2: **c**

-   Question 3: **a**

-   Question 4: **c**

Your output should reflect a score of 0/20. It should also print:

> Better luck next time!

## Good luck!
----------
##### Subscribe to our [YouTube Channel](https://www.youtube.com/@RayanSlim087?sub_confirmation=1) and Discover More Valuable Content!