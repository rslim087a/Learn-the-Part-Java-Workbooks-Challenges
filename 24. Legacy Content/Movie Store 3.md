# Movie Store – Part 3
----

> **Test-Driven Development**: write tests before writing code.

Unit testing results in modular code. Modular code is:
- easy to test.
- immune to bugs.
- easy to understand.
- scalable.

## Task 1: Unit Testing

### 1. Create a test that fails
----
Write a unit test named `sellMovieTest`. Inside, sell `The Godfather` and check if the store still contains the movie.  **Hint:** use `assertFalse`.


Inside `Store.java`, write code to make the test fail.

    /**
     * Function name: sellMovie
     * @param name (String)
     * 
     * Inside the function:
     *    //nothing
     */

### 2. Make the test pass
------


    /**
     * Function name: sellMovie
     * @param name (String)
     * 
     * Inside the function:
     *   1. loop runs through the size of the ArrayList.
     *   2. removes the movie that matches the name passed in. 
     */


### 3. Refactor
-----
Can `sellMovie` be simpler?

**Yes**. `removeIf` is a better way to remove elements. It removes elements that "match a predicate". In other words, elements for which the returned `boolean` is `true`.

```
ArrayList.removeIf(Lambda Expression)
```
The lambda expression for `removeIf`:
1. receives each element as a parameter.
2. has an arrow that points to code.
3. returns a `boolean`.

![Screen Shot 2021-07-02 at 2.55.08 PM.png](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F27c71cdb-a45e-4e7d-93dc-9463e1971f06?alt=media&token=edaa2b50-650c-409b-8c3b-239f841b7e6b)

**Important**: As you refactor, run the unit test to make sure there aren't bugs.


### 4. Refactor
-----

Can `sellMovie` be simpler? 

   - **Yes**. If the code is one line, you can omit the curly brackets and the `return` keyword. Java knows you intend to return a `boolean`.

![Screen Shot 2021-07-02 at 3.03.56 PM.png](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F1b2d2073-fe15-4b11-9ce7-3fcd4ba7a5fe?alt=media&token=1f044262-dbb1-4442-bf15-55d56162a4ae)

**Important**: As you refactor, run the unit test to make sure there aren't bugs.

### 5. Refactor
-----

Can `sellMovie` be simpler?  **No**. Refactoring complete.

## Good Luck
--------
##### Subscribe to our [YouTube Channel](https://www.youtube.com/@RayanSlim087?sub_confirmation=1) and Discover More Valuable Content!