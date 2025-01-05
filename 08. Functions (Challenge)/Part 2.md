# **Rock paper scissors part 2**

Part 2 will determine a winner.

## Task 4: the game result
-----------------------

1\. Function name:

```java
/**
 *  Function name: result   <-------
 *  @param yourChoice (String)
 *  @param computerChoice (String)
 *  @return result (String).
 */
```

2\. Parameters:

```java
/**
 *  Function name: result -
 *  @param yourChoice (String)  <-------
 *  @param computerChoice (String) <-------
 *  @return result (String).
 */
```

3\. Return value:

```java
/**
 *  Function name: result
 *  @param yourChoice (String)
 *  @param computerChoice (String)
 *  @return result (String). <--------
 */
```

Set up a series of `if - else if - else` statements according to the scenarios below:
```java
/**
 *
 * Function name: result - It returns the result of the game.
 *  @param yourChoice (String)
 *  @param computerChoice (String) 
 *  @return result (String) 
 * 
 * Inside the function:
 *   1. result is "You win" if:
 * 
 *       You: "rock"      Computer: "scissors"
 *       You: "paper"     Computer: "rock"
 *       You: "scissors"  Computer: "paper"
 * 
 *   2. result is "You lose" if:
 * 
 *       Computer: "rock"      You: "scissors"
 *       Computer: "paper"     You: "rock"
 *       Computer: "scissors"  You: "paper"
 * 
 *   3. result is "It's a tie" if:
 * 
 *       Your choice equals computer choice.
 *   
 *   4. Otherwise, print "INVALID CHOICE" and exit the program.
 *    
 *       
 */
```

Call the function and print the result.

```
- if the answer is yes:
  -- print: Great!
  -- print: rock -- paper -- scissors, shoot!
  -- pick up user's choice.
  -- get the computer choice.
  -- System.out.println("\nYou chose:        " + yourChoice);
  -- System.out.println("The computer chose: " + computerChoice);

  -- get the result              <------------
  -- System.out.println(result); <------------

  -- print everything        (can only be done after task 5).
- else:
  -- print: Darn, some other time...!
```

Before you move to task 5, this is a good place to test your code. The end result should print your choice, the computer's choice, and the result.

![](https://img-c.udemycdn.com/redactor/raw/article_lecture/2025-01-04_03-02-54-858c903e326b26540c6b07f5f4b95ee0.gif)

Run it a few more times. It should keep returning the correct result.

## Task 5: print everything at once
--------------------------------

Remove all your print statements from `main()`. Then, create the following function:

1\. Function name:

```java
/**
 * Name: printResult  <--------
 * @param yourChoice (String)
 * @param computerChoice (String)
 * @param result (String)
 *
 * Inside the function:
 *  1. prints everything:
 *      -- prints: You chose:          <your choice>
 *      -- prints: The computer chose: <computer choice>
 *      -- prints:                     <result>
 */
```

2\. Parameters:

```java
/**
 * Name: printResult
 * @param yourChoice (String) <------
 * @param computerChoice (String) <------
 * @param result (String)  <-------
 *
 * Inside the function:
 *  1. prints everything:
 *      -- prints: You chose:          <your choice>
 *      -- prints: The computer chose: <computer choice>
 *      -- prints:                     <result>
 */
```

3\. Return value: `void`.

4\. Inside the function:

```java
/**
 * Name: printResult
 * @param yourChoice (String)
 * @param computerChoice (String)
 * @param result (String)
 *
 * Inside the function:  <------
 *  1. prints everything:
 *      -- prints: You chose:          <your choice>
 *      -- prints: The computer chose: <computer choice>
 *      -- prints:                     <result>
 */
```

Back in the `if` statement, call `printResult()` and you're done!

```
- if the answer is yes:
   -- print: Great!
   -- print: rock -- paper -- scissors, shoot!
   -- pick up user's choice.
   -- get the computer choice.
   -- get the result.
   -- print everything <------
- else:
   -- print: Darn, some other time...!
```

## Run your code
-------------

![](https://img-c.udemycdn.com/redactor/raw/article_lecture/2025-01-04_03-02-54-6ae56e3b12b1efb6e535251fe4f63cd4.gif)

If it feels like you're playing a real game of rock-paper-scissors, then you're finished!

## Good luck!
----------
##### Your Path to Cloud-Native Engineering (After Learning Java)
###### 1. Develop Java Web Applications With Spring Boot → [Spring Boot Bootcamp](https://www.udemy.com/course/the-complete-spring-boot-development-bootcamp/?couponCode=SPRING_BOOTCAMP)
###### 2. Containerize and Deploy Web Applications with Docker → [Docker Bootcamp](https://www.udemy.com/course/docker-bootcamp-conquer-docker-with-real-world-projects/?couponCode=DOCKER_BOOTCAMP)
###### 3. Orchestrate Cloud Native Applications with Kubernetes → [Kubernetes Bootcamp](https://kubernetestraining.io/)