# Part 1

From the `Java Bootcamp Resources`, launch **`Part 1`**.

![1.png](https://img-c.udemycdn.com/redactor/raw/article_lecture/2025-01-03_22-52-09-961726c7868b629db69c576a50858720.png)

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

##### Your Path to Cloud-Native Engineering (After Learning Java)
###### 1. Develop Java Web Applications With Spring Boot → [Spring Boot Bootcamp](https://www.udemy.com/course/the-complete-spring-boot-development-bootcamp/?couponCode=SPRING_BOOTCAMP)
###### 2. Containerize and Deploy Web Applications with Docker → [Docker Bootcamp](https://www.udemy.com/course/docker-bootcamp-conquer-docker-with-real-world-projects/?couponCode=DOCKER_BOOTCAMP)
###### 3. Orchestrate Cloud Native Applications with Kubernetes → [Kubernetes Bootcamp](https://kubernetestraining.io/)