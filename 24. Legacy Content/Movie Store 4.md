# Movie Store – Part 4
----
> **Test-Driven Development**: write tests before writing code.

Unit testing results in modular code. Modular code is:
- easy to test.
- immune to bugs.
- easy to understand.
- scalable.

## Task 1

### 1. Create a test that fails
------
Write a unit test named `rentMovieTest`. `rentMovieTest` asserts the movie at index 1 isn't available after rental. 

Inside `Store.java`, write code to make the test fail.

```java
 /**
  * Function name: rentMovie
  * @param name (String)
  * 
  * Inside the function:
  *    //nothing
  */
```

### 2. Make the test pass
-----
Write code inside `Store.java` to make the test pass.
```java
 /**
  * Function name: rentMovie
  * @param name
  * 
  * Inside the function:
  *   1. Loop runs through every element
  *   2. Set the matching element's availability to false.
  * 
  */
```
### 3. Refactor
-----
Can the code be simpler? 

**Yes**. It's doing too much work. Copy its indexing logic into another method named `getMovieIndex`. 

``` java
/**
 * Function name: getMovieIndex 
 * @param name (String) 
 * @return (int)
 * 
 * Inside the function:
 *     1. returns index if it finds a movie. 
 *     2. returns -1000 otherwise.
 * 
 */
```
### 4. Refactor
-----
Can the code be simpler? 

Yes. `IntStream` offers a more elegant approach to retrieve an index. Use `IntStream` to run through a pipeline of functions.

![Screen Shot 2021-07-02 at 5.32.36 PM.png](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F6cd75f83-67b9-4d64-8af5-febce972c430?alt=media&token=ef39ee56-c9d7-477d-be24-0c5cec6f0984)

1. `range`: goes from 0 until the size.


2. `filter`: filters elements that match the predicate. The lambda expression receives each index inside the range and returns a boolean.

3. `findFirst`: returns the first element that matches the predicate and terminates the pipeline. If it can't find anything, the pipeline continues to `orElse`.

4. `orElse`: returns a random value. `orElse` terminates the pipeline no matter what.
 
 **Important**: As you refactor, run the unit test to make sure there are no bugs.

### 5. Refactor
-----
Can the code be simpler? **No**.


## Task 2

### 1. Create a test that fails
------

Write a unit test named `returnMovieTest`. `returnMovieTest` asserts that a movie is available after return. 

Inside `Store.java`, write code to make the test fail.
```java
    /**
     * Function name: returnMovie
     * @param name (String)
     * 
     * Inside the function:
     *    //nothing
     */
```
### 2. Make the test pass
-----
```java
    /**
     * Function name: returnMovie
     * @param name
     * 
     * Inside the function:
     *   1. Set the movie's availability to true.
     */
```
### 3. Refactor
-----
Can `returnMovie` be simpler? **No**. The code should be one line.

## Task 3

### 1. Create a test that fails
------
Write a unit test named `movieNotInStock`. This unit test expects the code throw an IllegalStateException:

```java
  @Test(expected = IllegalStateException.class) <----
  public void movieNotInStock() {

  }
```
Inside the unit test, rent "The Godfather". Then, sell "The Godfather". Your test should fail because it expects an `IllegalStateException`.

### 2. Make the test pass
-----
Throw an `IllegalStateException` from `sellMovie` if the movie is already rented. 
     
### 3. Refactor
-----
Can `sellMovie` be simpler? No.

## Task 4: Run every test

If every test passes, your code is free of bugs.

![Screen Shot 2021-07-09 at 9.14.51 PM.png](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F00144856-ad61-430a-8b82-fd13eb1fe747?alt=media&token=e7f99cf8-49a5-45f5-be41-0ea966a526bb)

## Final Remarks
-------
Compare your old code to the new code.

**Old code**:  a giant method that performs too many tasks. The method is impossible to unit test and is vulnerable to bugs.


![old vs new.gif](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2Fbf87a5ac-588b-4d25-b3a0-1f062c9bc81a?alt=media&token=f7d766ad-4748-4c12-9bec-6bce40415a2b)

**New code:** more polished. Each method performs one task (modular) and is easy to test. 

Therein lies the benefit of **Test Driven Development!**

--------
##### Subscribe to our [YouTube Channel](https://www.youtube.com/@RayanSlim087?sub_confirmation=1) and Discover More Valuable Content!