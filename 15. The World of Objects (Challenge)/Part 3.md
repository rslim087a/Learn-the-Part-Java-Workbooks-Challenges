# Part 3

From the `Java Bootcamp Resources`, launch **`Part 3`**.

![3.png](https://img-c.udemycdn.com/redactor/raw/article_lecture/2025-01-03_22-53-46-3286cc5e9a874db1d05209f122edb366.png)

## Initial Output

A while loop keeps running while the user enters the `String` `continue`.

```java
********************************MOVIE STORE*******************************
9.2     BlueRay         The Shawshank Redemption
9.1     BlueRay         The Godfather
9.0     DVD             The Godfather: Part II
8.9     DVD             12 Angry Men
9.0     BlueRay         The Dark Knight
8.9     DVD             Schindlers List
8.9     BlueRay         The Lord of the Rings: The Return of the King
8.8     DVD             Pulp Fiction
8.8     DVD             The Good, the Bad and the Ugly
8.8     DVD             The Lord of the Rings: The Fellowship of the Ring

To edit another rating, type: 'continue': continue
To edit another rating, type: 'continue': continue
To edit another rating, type: 'continue': stop
```
The code uses `next()` instead of `nextLine()` to pick up the next `String`.

## Task 1

Add code that prompts the user to enter an integer.
```java
    System.out.print("\nPlease choose an integer between 0 - 9: ");
    // grab nextInt()
```

```java
********************************MOVIE STORE*******************************
9.2     BlueRay         The Shawshank Redemption
9.1     BlueRay         The Godfather
9.0     DVD             The Godfather: Part II
8.9     DVD             12 Angry Men
9.0     BlueRay         The Dark Knight
8.9     DVD             Schindlers List
8.9     BlueRay         The Lord of the Rings: The Return of the King
8.8     DVD             Pulp Fiction
8.8     DVD             The Good, the Bad and the Ugly
8.8     DVD             The Lord of the Rings: The Fellowship of the Ring


Please choose an integer between 0 - 9: 4
```
## Task 2

Grab a movie from the store based on the user input.

## Task 3

Add code that prompts the user to enter a rating for the movie.

```java
    System.out.print("Set a new rating for " + movie.getName() + ": ");
    // grab nextDouble()
```

```
********************************MOVIE STORE*******************************
9.2     BlueRay         The Shawshank Redemption
9.1     BlueRay         The Godfather
9.0     DVD             The Godfather: Part II
8.9     DVD             12 Angry Men
9.0     BlueRay         The Dark Knight
8.9     DVD             Schindlers List
8.9     BlueRay         The Lord of the Rings: The Return of the King
8.8     DVD             Pulp Fiction
8.8     DVD             The Good, the Bad and the Ugly
8.8     DVD             The Lord of the Rings: The Fellowship of the Ring


Please choose an integer between 0 - 9: 4

Set a new rating for The Dark Knight: 5.8
```

## Task 4

Update the store, and print the updated store.

```java
    store.setMovie(choice, movie);
    printStore();
```

## Final Output

```
********************************MOVIE STORE*******************************
9.2     BlueRay         The Shawshank Redemption
9.1     BlueRay         The Godfather
9.0     DVD             The Godfather: Part II
8.9     DVD             12 Angry Men
9.0     BlueRay         The Dark Knight
8.9     DVD             Schindler's List
8.9     BlueRay         The Lord of the Rings: The Return of the King
8.8     DVD             Pulp Fiction
8.8     DVD             The Good, the Bad and the Ugly
8.8     DVD             The Lord of the Rings: The Fellowship of the Ring


Please choose an integer between 0 - 9: 5
Set a new rating for Schindler's List: 9.8

********************************MOVIE STORE*******************************
9.2     BlueRay         The Shawshank Redemption
9.1     BlueRay         The Godfather
9.0     DVD             The Godfather: Part II
8.9     DVD             12 Angry Men
9.0     BlueRay         The Dark Knight
9.8     DVD             Schindler's List
8.9     BlueRay         The Lord of the Rings: The Return of the King
8.8     DVD             Pulp Fiction
8.8     DVD             The Good, the Bad and the Ugly
8.8     DVD             The Lord of the Rings: The Fellowship of the Ring

To edit another rating, type: 'continue': stop
```
----------

##### **Go From Zero to DevOps Master**: *[Java → Spring Boot → Docker → Kubernetes](https://rslim087a.github.io/zero-devops-roadmap/)*
