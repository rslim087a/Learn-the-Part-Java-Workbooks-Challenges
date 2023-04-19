#  List Collections - Extra Practice

From the `Java Bootcamp Resources`, launch **`Part 1`**.

![1.png](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F995797a5-9b4c-4d77-a8f9-9c2b364e7f85?alt=media&token=ebf6ecea-753a-47e1-a694-0964cf811716)

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
##### Subscribe to our [YouTube Channel](https://www.youtube.com/@RayanSlim087?sub_confirmation=1) and Discover More Valuable Content!