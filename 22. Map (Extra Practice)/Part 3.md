# Part 3

From the `Java Bootcamp Resources`, launch **`Part 3`**.

![3.png](https://img-c.udemycdn.com/redactor/raw/article_lecture/2025-01-03_22-17-46-0a6f5c23863c8bfc358a210a31caa3e1.png)


## Task 1

Inside the `Main` class, create a method called `isNullOrBlank` that takes a `String` input and returns `true` if the input is `null` or `blank`.

```java
public static boolean isNullOrBlank(String input) {
    // TODO
}
```
## Task 2

Create a method called `incorrectPopulation` that takes an `int` input and `returns` `true` if the input is less than or equal to 0.

```java
public static boolean incorrectPopulation(int population) {
    // TODO
}
```
## Task 3
Create a method called `promptForCityName` that takes a `Scanner` input and returns a valid city name entered by the user.

```java
public static String promptForCityName(Scanner scanner) {
    while (true) {
        System.out.print("\nPlease enter a valid city name: ");
        String cityName = scanner.nextLine();
        // TODO
    }
}
```

## Task 4
Create a method called `promptForCountry` that takes a `Scanner` input and returns a valid country entered by the user.

```java
public static String promptForCountry(Scanner scanner) {
    while (true) {
        System.out.print("\nPlease enter a valid country: ");
        String country = scanner.nextLine();
        // TODO
    }
}
```
## Task 5
Create a method called `promptForPopulation` that takes a `Scanner` input and returns a valid population entered by the user.

```java
public static int promptForPopulation(Scanner scanner) {
    while (true) {
        System.out.print("\nPlease enter a valid population (greater than 0): ");
        // First check if the next input is not an integer
              // scanner.next();
              // continue;

        int population = scanner.nextInt();
        // TODO
    }
}
```

## Task 6
Test the interactive methods in the main method.

```java
public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        String cityName = promptForCityName(scanner);

        String country = promptForCountry(scanner);

        int population = promptForPopulation(scanner);

        City newCity = new City(cityName, country, population);

        CityPopulationTracker tracker = new CityPopulationTracker();
        tracker.addCity(newCity);

        System.out.println("City added to the tracker: " + newCity.getName());
}
```
-----
##### **Go From Zero to DevOps Master**: *[Java → Spring Boot → Docker → Kubernetes](https://rslim087a.github.io/zero-devops-roadmap/)*