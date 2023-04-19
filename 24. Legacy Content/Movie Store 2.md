# Movie Store – Part 2

> **Test-Driven Development**: write tests before writing code.

Unit testing results in modular code. Modular code is:
- easy to test.
- immune to bugs.
- easy to understand.
- scalable.

## Task 1: `@Before`
------
> `@Before` runs a method before each test.

- Create a `void` method named `setup`, and annotate it with `@Before`.
- Inside the function, set `store` equal to a new object of the `Store` class.

## Task 2: Unit Testing
### 1. Create a test that fails
---

Inside `@Before`, add two `Movie` objects. 
   ```java
   store.addMovie(new Movie("The Shawshank Redemption", "Blue-Ray", 9.2));
   store.addMovie(new Movie("The Godfather", "Blue-Ray", 9.1));
   ```

Inside `Store.java`, create an `addMovie` method.

```java
 /**
  * Function name: addMovie
  * @param movie 
  * 
  * Inside the function:
  *   1. adds a movie object
  */
```

Write a unit test named `moviedAdded`. Inside, use `assertTrue` to assert the `store`.`contains(new Movie("The Godfather", "Blue-Ray", 9.1)`.


Inside `Store.java`, write code to make the test fail.

```java
    /**
     * Function name: contains
     * @param movie
     * @return (boolean)
     * 
     * Inside the function:
     *    1. checks if movies list contains() movie.
     */
 ```


### 2. Make the test pass 

**Hint**: `contains()` needs *your* `equals` method to effectively compare `Movie` objects. See lesson: the `equals()` method.

```java
 public boolean equals(Object obj) {    

     // return false if parameter is null.
        
     // return false if parameter isn't instance of Movie class.

     // typecast the object to Movie.
        
     // compare fields from both objects and return the result.

  }
```

### 3. Refactor
--- 
Can the code be simpler? **No**. Refactoring complete.

## Good Luck
--------
##### Subscribe to our [YouTube Channel](https://www.youtube.com/@RayanSlim087?sub_confirmation=1) and Discover More Valuable Content!