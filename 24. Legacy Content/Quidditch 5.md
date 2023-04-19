# Quidditch – Part 5

**Goal**: write unit tests for the simulation.

The first step in **Test-Driven Development** is to identify meaningful test cases. `requirements.txt` identifies the following test cases for the simulation:

- Test if it can find the placeholder in each play.
- Test if it can replace the placeholder in each play.
- If the placeholder is `<chaser>`, test if a team's score updates by `QUAFFLE_POINTS`.
- If the placeholder is `<seeker>`, test if a team's score updates by `SNITCH_POINTS`.

## Task 1
---
Create a method that runs before every test. Inside the method, set up the game object as you did `main()`.

## Task 2
---
### 1. Create a test that fails

Inside `GameTest.java`, write a unit test named `getPlaceholderTest`. The test asserts that `game.getPlaceholder("<chaser> gets the next pass")` returns **`chaser`**.

Inside `Game.java`, write code to make the test fail.

```java
/**
 * Function name: getPlaceholder
 * @param play (String)
 * @return (String)
 * 
 * Inside the function:
 *  1. Returns "hello".
 */
```
### 2. Make the test pass

```java
/**
 * Function name: getPlaceholder
 * @param play (String)
 * @return (String)
 * 
 * Inside the function:
 *  1. Returns a substring between two < > characters.
 */
```
**Hint**: research how to get a `String` between two characters on Stack Overflow. Then, visit the documentation to get more information about the methods being proposed: [**Documentation**](https://docs.oracle.com/en/java/javase/11/docs/api/java.base/java/lang/String.html#substring(int))


### 3. Refactor
If possible, refactor the code you researched.

## Task 3
---
### 1. Create a test that fails

Write a unit test named `replacePlaceholderTest`. The test asserts that `game.replacePlaceholder("<chaser> gets the next pass", "chaser", "Katie"))` returns **`Katie gets the next pass`**.

Inside `Game.java`, write code to make the test fail.

```java
    /** 
     * Function name: replacePlaceholder
     * @param play
     * @param placeholder
     * @param value
     * @return (String)
     * 
     * Inside the function:
     *  1. returns "Hello"
     */
```
### 2. Make the test pass

```java
    /** 
     * Function name: replacePlaceholder
     * @param play
     * @param placeholder
     * @param value
     * @return (String)
     * 
     * Inside the function:
     *  1. Replaces the placeholder in a play with a value
     */
```
**Hint**: research how to replace part of a `String` with a value.

### 3. Refactor
If possible, refactor the code you researched.

## Task 4
---

### 1. Create a test that fails

Write a unit test named `quaffleScoreTest`. 

- Inside the unit test:
   -  get the `GRYFFINDOR` team and call the method `game.quaffleScore(team)` twice.
   -  assert that `game.getScore(team)` returns a score of 20 for `GRYFFINDOR`.

- Inside `Game.java`, write code to make the test fail.

```java
    /**
     * Function name: quaffleScore
     * @param team
     * 
     * Inside the function:
     *  do nothing
     */
```

### 2. Make the test pass

```java
    /**
     * Function name: quaffleScore
     * @param team
     * 
     * Inside the function:
     *  1. Update the team's points by `QUAFFLE_POINTS`. <---
     */
```

### 3. Refactor

Refactor if necessary
## Task 5
---

### 1. Create a test that fails

Write a unit test named `catchSnitchTest`. 

- The unit test calls the method `game.catchSnitch(Team)` once for `SLYTHERIN`.

- The test asserts `game.getScore(team)` returns a score of 150 for `SLYTHERIN`.

Inside `Game.java`, write code to make the test fail:
```java
    /**
     * Function name: catchSnitch
     * @param team
     * 
     * Inside the function:
     *  do nothing
     */
```
### 2. Make the test pass
```java
    /**
     * Function name: catchSnitch
     * @param team
     * 
     * Inside the function:
     *  1. Update the team's points by `SNITCH_POINTS`. <---
     */
```
### 3. Refactor
Refactor if necessary.

## Task 6
---
Run every test in `GameTest.java`. If they all pass, you can continue to task 7.

![Screen Shot 2021-07-15 at 9.27.42 PM.png](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2Fc27c9804-f4c4-4cac-aad2-7622248bfa4a?alt=media&token=82442fa8-ceb7-47dd-8fed-bdee9e34565b)

## Task 7
---
Inside `Game.java`, create a method `simulate(String play)` that returns a `String`.

1. From the play, retrieve the `placeholder`.
2. Get a random team from the `HashMap`.
   - **See Task 8.** 
3. Create an `if - else if - else` statement that checks if the placeholder equals:
 
  - `Team.POSITION_CHASER`:
       - call `quaffleScore`.
       - Get a random chaser from the team.
       - Replace the placeholder and return the simulated play.
  
  - `Team.POSITION_SEEKER`:
       - call `catchSnitch`.
       - Replace the placeholder and return the simulated play.  

  - `Team.POSITION_KEEPER`:
       - Replace the placeholder and return the simulated play.  

## Task 8

Create a method that returns a random team from the `HashMap`.
```java
    /**
     * Function name: getRandomTeam()
     * @return (Team)
     * 
     *  1. converts scoreBoard to keySet.
     *  2. converts keyset to array (easier to index).
     *  3. returns a random team from the array of teams. 
     */
```
Use the following syntax for **1** and **2**: `scoreBoard.keySet().toArray()`. 

Create a function named `random` and call it for **3**. 
```java
/**
 * Function name: random
 * @param range
 * @return int
 * 
 * Inside the function:
 *  1. Returns a number between 0 and one less the range
 */
``` 
## Good Luck!
--------
##### Subscribe to our [YouTube Channel](https://www.youtube.com/@RayanSlim087?sub_confirmation=1) and Discover More Valuable Content!