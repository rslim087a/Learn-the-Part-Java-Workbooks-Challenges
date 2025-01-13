# Part 2

From the `Java Bootcamp Resources`, launch **`Part 2`**.

![2.png](https://img-c.udemycdn.com/redactor/raw/article_lecture/2025-01-03_22-30-00-e670f6ff3d72c0a18b468f1ae9baa972.png)


## Task 0

The `loadMovies` method is already implemented. 
```java
     public static void loadMovies(String fileName) throws FileNotFoundException {
         // reads input from file...
     }
```

If you want to visualize its runtime, feel free to watch the video solution.

## Task 1

This method should return `true` if the choice is less than 0 or greater than 9.
```java
    public static boolean incorrectChoice(int choice) {
        // TODO
    }
```

## Task 2

This method should return `true` if the rating is less than 0 or greater than 10.
```java
    public static boolean incorrectRating(double rating) {
        // TODO
    }
```

## Task 3

The method `promptForChoice` will return the integer they choose.
```java
    public static int promptForChoice(Scanner scanner) {
        while (true) {
            System.out.print("\nPlease choose an integer between 0 - 9: ");

            int choice = scanner.nextInt();
            return choice; <--------------
        }
    }
```

**Scenario One**: `continue` the while loop if the user doesn't enter an integer.

```java
    public static int promptForChoice(Scanner scanner) {
        while (true) {
            System.out.print("\nPlease choose an integer between 0 - 9: ");

            // 1. Anticipate the user not entering an integer. <--------------

            int choice = scanner.nextInt();

            return choice; 
        }
    }
```

**Scenario Two**: `continue` the while loop if the user enters an incorrect choice.

```java
    public static int promptForChoice(Scanner scanner) {
        while (true) {
            System.out.print("\nPlease choose an integer between 0 - 9: ");

            // 1. Anticipate the user not entering an integer.

            int choice = scanner.nextInt();

            // 2. Anticipate the choice being incorrect. <--------------
            return choice; 
        }
    }
```

## Task 4

The method `promptForRating` will return the rating they choose.
```java
    public static double promptForRating(Scanner scanner, String name) {
        while (true) {
            System.out.print("\nSet a new rating for " + name + ": ");
            

            double rating = scanner.nextDouble();            
            return rating; <---------
         }
    }
```

**Scenario One**: `continue` the while loop if the user doesn't enter a `double`.

```java
    public static double promptForRating(Scanner scanner, String name) {
        while (true) {
            System.out.print("\nSet a new rating for " + name + ": ");
            
            // 1. Anticipate the user not entering a double. <-------------

            double rating = scanner.nextDouble();            
            
            return rating;
         }
    }
```

**Scenario Two**: `continue` the while loop if the user enters an incorrect rating.

```java
    public static double promptForRating(Scanner scanner, String name) {
        while (true) {
            System.out.print("\nSet a new rating for " + name + ": ");
            
            // 1. Anticipate the user not entering a double.

            double rating = scanner.nextDouble();
            
            // 2. Anticipate the rating being incorrect. <----------
            
            return rating;
         }
    }
```

----------

##### **Go From Zero to DevOps Master**: *[Java → Spring Boot → Docker → Kubernetes](https://rslim087a.github.io/zero-devops-roadmap/)*