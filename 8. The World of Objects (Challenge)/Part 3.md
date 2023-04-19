# Part 3

From the `Java Bootcamp Resources`, launch **`Part 3`**.

![3.png](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2Fb482a4c6-07ab-4d4b-94a6-f3f2f662d3ea?alt=media&token=fdb5d33b-1e9f-412f-9353-e2a54e897162)

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

##### Subscribe to our [YouTube Channel](https://www.youtube.com/@RayanSlim087?sub_confirmation=1) and Discover More Valuable Content!
