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

![](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F91169998-c75d-4134-b91c-560e5a85ebfd?alt=media&token=794d92c5-1547-4195-9f3b-5b5ecea5794c)

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

![](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2Fdd2570dc-cb51-4b5d-8d60-567413c367f5?alt=media&token=99fc526b-a267-40fd-a1ab-72b1cc76ab61)

If it feels like you're playing a real game of rock-paper-scissors, then you're finished!

## Good luck!
----------
##### Subscribe to our [YouTube Channel](https://www.youtube.com/@RayanSlim087?sub_confirmation=1) and Discover More Valuable Content!