# Part 1

From the `Java Bootcamp Resources`, launch **`Part 1`**.

![1.png](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F995797a5-9b4c-4d77-a8f9-9c2b364e7f85?alt=media&token=ebf6ecea-753a-47e1-a694-0964cf811716)

## Task 1

Add the following fields to the `Movie` class.
```java
    private String name;
    private String format;
    private double rating;
```
Then create a constructor, copy constructor, getters, and setters.

## Task 2

Create a `toString` method that returns the following `String`.
```java
    return this.rating + "\t" + this.format + "\t\t" + this.name + "";
```

## Task 3

Populate the array inside `main()` with the following `Movie` objects.
```java
new Movie("The Shawshank Redemption", "BlueRay", 9.2),
new Movie("The Godfather", "BlueRay", 9.1),
new Movie("The Godfather: Part II", "DVD", 9.0),
new Movie("The Dark Knight", "BlueRay", 9.0),
new Movie("Schindler's List", "DVD", 8.9),
new Movie("The Lord of the Rings: The Return of the King", "BlueRay", 8.9),
new Movie("Pulp Fiction", "DVD", 8.8),
new Movie("The Lord of the Rings: The Fellowship of the Ring", "DVD", 8.8)
```

## Final Output

```java
********************************MOVIE STORE*******************************
9.2     BlueRay         The Shawshank Redemption
9.1     BlueRay         The Godfather
9.0     DVD             The Godfather: Part II
9.0     BlueRay         The Dark Knight
8.9     DVD             Schindlers List
8.9     BlueRay         The Lord of the Rings: The Return of the King
8.8     DVD             Pulp Fiction
8.8     DVD             The Lord of the Rings: The Fellowship of the Ring
```

----------

##### Subscribe to our [YouTube Channel](https://www.youtube.com/@RayanSlim087?sub_confirmation=1) and Discover More Valuable Content!