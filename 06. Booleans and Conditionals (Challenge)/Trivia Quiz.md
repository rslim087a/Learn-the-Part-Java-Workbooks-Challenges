# Trivia Quiz

The quiz will ask multiple-choice questions about common trivia. It tracks the user's answers and prints their final score.

![](https://img-c.udemycdn.com/redactor/raw/article_lecture/2025-01-04_03-26-32-2385e223461c2c1b226c98dd0577e560.gif)

## Open the challenge

From `Java Bootcamp Resources`, launch `Challenge 3`.

![Screen Shot 2022-10-16 at 7.18.41 PM.png](https://img-c.udemycdn.com/redactor/raw/article_lecture/2025-01-04_03-26-32-aa312d19f7b1508d332ec2e375df32c9.png)

## 1\. Store each answer.
----------------------

Add code that picks up the user's answer. Use the comments to guide your code.

```
        System.out.println("1. Which country held the 2016 Summer Olympics?");
        System.out.println("\ta) China\n\tb) Ireland\n\tc) Brazil\n\td) Italy\n");
        //store answer 1
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
##### **Go From Zero to DevOps Master**: *[Java → Spring Boot → Docker → Kubernetes](https://rslim087a.github.io/zero-devops-roadmap/)*