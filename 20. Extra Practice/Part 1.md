# Part 1

From the `Java Bootcamp Resources`, launch **`Part 1`**.

![1.png](https://img-c.udemycdn.com/redactor/raw/article_lecture/2025-01-03_22-25-30-8bd3a3b04c6af2166e20a2cd9f058a0f.png)


## Task 1

Create a new file named `Magazine.java`. Inside the file, create the Magazine class.

```java
public class Magazine {

}

```

The Magazine class will define the following fields:

```java
    private String title;
    private String publisher;
    private int issueNumber;
    private int publicationYear;
```

## Task 2
Create getter and setter methods for each field of the `Magazine` class. Ensure that the setter methods perform the following argument validations and throw an `IllegalArgumentException` with an appropriate error message if the input is invalid:

- `setTitle` method:

     - Check if the input `title` is `null` or `blank`.
     - If the validation fails, throw an `IllegalArgumentException` with the message `"Title cannot be null or blank."`

- `setPublisher` method:
    - Check if the input `publisher` is null or `blank`.
    - If the validation fails, throw an `IllegalArgumentException` with the message `"Publisher cannot be null or blank."`

- `setIssueNumber` method:

  - Check if the input `issueNumber` is less than or equal to `0`.
  - If the validation fails, throw an `IllegalArgumentException` with the message `"Issue number must be greater than 0."`

- `setPublicationYear` method:

  - Check if the input `publicationYear` is less than or equal to 0.
  - If the validation fails, throw an `IllegalArgumentException` with the message `"Publication year must be greater than 0."`


After implementing the setter methods with the appropriate validations, create the corresponding getter methods for each field.



## Task 3
Create a constructor that initializes the fields of a newly created object by calling the setter methods.

```java
public Magazine(String title, String publisher, int issueNumber, int publicationYear) {
    setTitle(title);
    setPublisher(publisher);
    setIssueNumber(issueNumber);
    setPublicationYear(publicationYear);
}
```
Using the setter methods in the constructor ensures that the argument validation is performed in a single place, keeping the code DRY (Don't Repeat Yourself).

## Task 4
Test your constructor and getter/setter methods by creating instances (objects) of the Magazine class. Uncomment each test one by one to ensure that the methods throw an `IllegalArgumentException` when the input is invalid. Remember to re-comment the test before moving on to the next one.



```java
public static void main(String[] args) {
    Magazine magazine1 = new Magazine("Magazine 1", "Publisher 1", 1, 2020);
    System.out.println(magazine1.getTitle());

    // Uncomment the following line to test invalid input for setTitle method
    // magazine1.setTitle("");

    // Uncomment the following line to test invalid input for setPublisher method
    // magazine1.setPublisher("");

    // Uncomment the following line to test invalid input for setIssueNumber method
    // magazine1.setIssueNumber(-1);

    // Uncomment the following line to test invalid input for setPublicationYear method
    // magazine1.setPublicationYear(0);

    // Uncomment the following line to test invalid input for the constructor
    // Magazine magazine2 = new Magazine("", "Publisher 2", 2, 2020);
}
```

When testing each method, the program will throw an `IllegalArgumentException` if the input is invalid. This helps us to identify mistakes in our application and fix the issues, preventing the creation of objects with an invalid state that could lead to unexpected behavior or errors during program execution.

-----
##### **Go From Zero to DevOps Master**: *[Java → Spring Boot → Docker → Kubernetes](https://rslim087a.github.io/zero-devops-roadmap/)*