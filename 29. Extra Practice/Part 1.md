# Part 1

From the `Java Bootcamp Resources`, launch **`Part 1`**.

![1.png](https://img-c.udemycdn.com/redactor/raw/article_lecture/2025-01-03_18-23-35-8a2f41145a36160948d612b01d9db3d4.png)


## Task 1
Inside the `MovieStore` class, create the following field:

```java
private List<Movie> movies;
```

## Task 2
Create a constructor class that initializes the `movies` field to an empty `ArrayList`.

```java
public MovieStore() {
    this.movies = new ArrayList<>();
}
```

## Task 3
Create a method named `addMovie` that takes a Movie object as a parameter and adds it to the `movies` list.

## Task 4
Create a method named `filterByGenre` that takes a `String` representing a genre as a parameter and returns a `List<Movie>` containing only movies of the specified genre.

 - `stream()` - Converts the movies list into a Stream<Movie>.
 - `filter()` - Filters the stream of movies, keeping only movies with the specified genre. Outputs a filtered `Stream<Movie>`.
 - `toList()` - Collects the filtered stream of movies into a List<Movie>.

## Task 5
Create a method named `sortByReleaseYear` that returns a `List<Movie>` containing all movies sorted by their release year in ascending order.

 - `stream()` - Converts the movies list into a Stream<Movie>.
 - `sorted()` - Sorts the stream of movies by their release year in ascending order. Outputs a sorted `Stream<Movie>`.
 - `toList()` - Collects the sorted stream of movies into a List<Movie>.


## Task 6
Create a method named `getTopRatedMovies` that takes an `int` value n as a parameter and returns a `List<Movie>` containing the top n rated movies in descending order.

 - `stream()` - Converts the movies list into a Stream<Movie>.
 - `sorted()` - Sorts the stream of movies by their rating in descending order. Outputs a sorted `Stream<Movie>`.
 - `limit()` - Trims the sorted stream to the top n rated movies. Outputs a limited Stream<Movie>.
 - `toList()` - Collects the limited stream of movies into a List<Movie>.

## Task 7
Test the `MovieStore` class by creating a few `Movie` objects, initializing a `MovieStore` object, and then using the methods from Tasks 4 to 6 to perform various operations on the movies.

```java
public static void main(String[] args) {
    Movie movie1 = new Movie("Inception", "Christopher Nolan", "Sci-Fi", 2010, 8.8);
    Movie movie2 = new Movie("The Dark Knight", "Christopher Nolan", "Action", 2008, 9.0);
    Movie movie3 = new Movie("The Matrix", "Lana Wachowski, Lilly Wachowski", "Sci-Fi", 1999, 8.7);
    Movie movie4 = new Movie("Pulp Fiction", "Quentin Tarantino", "Crime", 1994, 8.9);

    MovieStore movieStore = new MovieStore();
    movieStore.addMovie(movie1);
    movieStore.addMovie(movie2);
    movieStore.addMovie(movie3);
    movieStore.addMovie(movie4);

    List<Movie> sciFiMovies = movieStore.filterByGenre("Sci-Fi");
    List<Movie> sortedMovies = movieStore.sortByReleaseYear();
    List<Movie> topRatedMovies = movieStore.getTopRatedMovies(3);

    System.out.println("Sci-Fi Movies:");
    sciFiMovies.forEach(movie -> System.out.println(movie));

    System.out.println("\nSorted by Release Year:");
    sortedMovies.forEach(movie -> System.out.println(movie));

    System.out.println("\nTop Rated Movies:");
    topRatedMovies.forEach(movie -> System.out.println(movie));
}
```

-----
##### Your Path to Cloud-Native Engineering (After Learning Java)
###### 1. Develop Java Web Applications With Spring Boot → [Spring Boot Bootcamp](https://www.udemy.com/course/the-complete-spring-boot-development-bootcamp/?couponCode=SPRING_BOOTCAMP)
###### 2. Containerize and Deploy Web Applications with Docker → [Docker Bootcamp](https://www.udemy.com/course/docker-bootcamp-conquer-docker-with-real-world-projects/?couponCode=DOCKER_BOOTCAMP)
###### 3. Orchestrate Cloud Native Applications with Kubernetes → [Kubernetes Bootcamp](https://kubernetestraining.io/)