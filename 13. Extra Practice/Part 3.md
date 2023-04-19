# Part 3

From the `Java Bootcamp Resources`, launch **`Part 3`**.

![3.png](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2Fb482a4c6-07ab-4d4b-94a6-f3f2f662d3ea?alt=media&token=fdb5d33b-1e9f-412f-9353-e2a54e897162)

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
##### Subscribe to our [YouTube Channel](https://www.youtube.com/@RayanSlim087?sub_confirmation=1) and Discover More Valuable Content!