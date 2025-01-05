#  List Collections - Extra Practice

From the `Java Bootcamp Resources`, launch **`Part 1`**.

![1.png](https://img-c.udemycdn.com/redactor/raw/article_lecture/2025-01-03_22-37-30-eb761bb9128ea9c6561d841cc7089007.png)

## Task 1

Create a new file named `Book.java`. Inside the file, create the Book class.

```java
public class Book {

}
```
The `Book` class will define the following fields:

```java
    private String title;
    private String author;
    private double rating;
    private double price;
```
The Book class serves as a blueprint for creating Book objects.

## Task 2

Create a constructor that initializes the fields of a newly created object.


## Task 3

Create a constructor that initializes a new object using an existing object's fields.

## Task 4
Create getter and setter methods for each field of the Book class.

## Task 5
Test your constructor and getter/setter methods by creating instances (objects) of the Book class.

```java
public static void main(String[] args) {
    Book book1 = new Book("To Kill a Mockingbird", "Harper Lee", 4.27, 15.99);
    Book book2 = new Book("1984", "George Orwell", 4.17, 12.99);
    Book book3 = new Book("Moby-Dick", "Herman Melville", 3.5, 14.99);
    Book book4 = new Book("Pride and Prejudice", "Jane Austen", 4.25, 10.99);
}
```

## Task 6
Test the copy constructor by creating two objects with fields copied from two existing objects.

```java
public static void main(String[] args) {
    // Assuming the Book objects from Task 5 are available
    Book copyBook1 = new Book(book1);
    Book copyBook2 = new Book(book3);
}
```
## Task 7

Use breakpoints to inspect field initialization in the new objects created using the copy constructor and verify the getter/setter methods are working correctly.

-----
##### Your Path to Cloud-Native Engineering (After Learning Java)
###### 1. Develop Java Web Applications With Spring Boot → [Spring Boot Bootcamp](https://www.udemy.com/course/the-complete-spring-boot-development-bootcamp/?couponCode=SPRING_BOOTCAMP)
###### 2. Containerize and Deploy Web Applications with Docker → [Docker Bootcamp](https://www.udemy.com/course/docker-bootcamp-conquer-docker-with-real-world-projects/?couponCode=DOCKER_BOOTCAMP)
###### 3. Orchestrate Cloud Native Applications with Kubernetes → [Kubernetes Bootcamp](https://kubernetestraining.io/)