# Workbook 8.1

From the `Java Bootcamp Resources`, launch **`starter`**.

![1.png](https://img-c.udemycdn.com/redactor/raw/article_lecture/2025-01-03_22-41-33-68fce9306d0a534a7e49be3377f32a44.png)

## Task 1

Initialize the `List` field inside the `Store` constructor,
```java
    private List<Movie> movies;

    public Store() {
        
    }
```
**`LinkedList`** or **`ArrayList`?**

This application prioritizes retrieving/updating data and does not add/remove elements from the middle.

## Task 2

Finish writing the code for these methods. 

```java
    public Movie getMovie(int index) {
        return null;
    }

    public void setMovie(int index, Movie movie) {
        // TODO
    }

    public void addMovie(Movie movie) {
        // TODO
    }
```

## Task 3

Inside the `main()` method, populate the store using a **`foreach`** loop. 
```java
    public static void main(String[] args) {
        Movie[] movies = new Movie[] {
            new Movie("The Shawshank Redemption", "BlueRay", 9.2),
            new Movie("The Godfather", "BlueRay", 9.1),
            new Movie("The Godfather: Part II", "DVD", 9.0),
            new Movie("12 Angry Men", "DVD", 8.9),
            new Movie("The Dark Knight", "BlueRay", 9.0),
            new Movie("Schindler's List", "DVD", 8.9),
            new Movie("The Lord of the Rings: The Return of the King", "BlueRay", 8.9),
            new Movie("Pulp Fiction", "DVD", 8.8),
            new Movie("The Good, the Bad and the Ugly", "DVD", 8.8),
            new Movie("The Lord of the Rings: The Fellowship of the Ring", "DVD", 8.8)
        };

        // TODO: Populate store using a foreach loop. 

        printStore();
        userInput();

    }
```

Don't use a regular loop because we don't need the index.


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