# Part 3

From the `Java Bootcamp Resources`, launch **`Part 3`**.

![3.png](https://img-c.udemycdn.com/redactor/raw/article_lecture/2025-01-03_22-27-09-669aa067281080e0190d14baa5a97fa4.png)

## Task 1
Inside the Main class, create a method called `isNullOrBlank` that takes a `String` input and returns `true` if the input is `null` or `blank`.


```java
public static boolean isNullOrBlank(String input) {
    // TODO
}
```

## Task 2

Create a method called `incorrectIssueNumber` that takes an `int` input and returns `true` if the input is less than or equal to 0.

```java
public static boolean incorrectIssueNumber(int issueNumber) {
    // TODO
}
```

## Task 3
Create a method called `incorrectPublicationYear` that takes an `int` input and returns `true` if the input is less than or equal to `0`.

```java
public static boolean incorrectPublicationYear(int publicationYear) {
    // TODO
}
```

## Task 4
Create a method called `promptForTitle` that takes a `Scanner` input and returns a valid `title` entered by the user.

```java
public static String promptForTitle(Scanner scanner) {
    while (true) {
        System.out.print("\nPlease enter a valid title: ");
        String title = scanner.nextLine();
        // TODO
    }
}
```
## Task 5
Create a method called `promptForPublisher` that takes a `Scanner` input and returns a valid publisher entered by the user.

```java
public static String promptForPublisher(Scanner scanner) {
    while (true) {
        System.out.print("\nPlease enter a valid publisher: ");
        String publisher = scanner.nextLine();
        // TODO
    }
}
```

## Task 6

Create a method called `promptForIssueNumber` that takes a `Scanner` input and returns a valid issue number entered by the user.

```java
public static int promptForIssueNumber(Scanner scanner) {
    while (true) {
        System.out.print("\nPlease enter a valid issue number (greater than 0): ");
        // First check if the next input is not an integer
              // scanner.next();
              // continue;
 
        int issueNumber = scanner.nextInt();
        // TODO
    }
}
```
## Task 7
Create a method called `promptForPublicationYear` that takes a Scanner input and returns a valid publication year entered by the user.

```java
public static int promptForPublicationYear(Scanner scanner) {
    while (true) {
        System.out.print("\nPlease enter a valid publication year (greater than 0): ");
        // First check if the next input is not an integer
              // scanner.next();
              // continue;
        int publicationYear = scanner.nextInt();
        // TODO
    }
}
```
## Task 8
Test the interactive methods in the main method.

```java
public static void main(String[] args) {
    Scanner scanner = new Scanner(System.in);

    String title = promptForTitle(scanner);
    String publisher = promptForPublisher(scanner);
    int issueNumber = promptForIssueNumber(scanner);
    int publicationYear = promptForPublicationYear(scanner);

    Magazine newMagazine = new Magazine(title, publisher, issueNumber, publicationYear);

    MagazineLibrary library = new MagazineLibrary();
    library.addMagazine(newMagazine);

    System.out.println("Magazine added to the library: " + newMagazine.getTitle());
}
```
-----
##### Your Path to Cloud-Native Engineering (After Learning Java)
###### 1. Develop Java Web Applications With Spring Boot → [Spring Boot Bootcamp](https://www.udemy.com/course/the-complete-spring-boot-development-bootcamp/?couponCode=SPRING_BOOTCAMP)
###### 2. Containerize and Deploy Web Applications with Docker → [Docker Bootcamp](https://www.udemy.com/course/docker-bootcamp-conquer-docker-with-real-world-projects/?couponCode=DOCKER_BOOTCAMP)
###### 3. Orchestrate Cloud Native Applications with Kubernetes → [Kubernetes Bootcamp](https://kubernetestraining.io/)