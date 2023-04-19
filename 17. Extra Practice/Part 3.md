# Part 3

From the `Java Bootcamp Resources`, launch **`Part 3`**.

![3.png](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2Fb482a4c6-07ab-4d4b-94a6-f3f2f662d3ea?alt=media&token=fdb5d33b-1e9f-412f-9353-e2a54e897162)
# 

## Task 1
Inside the Main class, create a method called `isNullOrBlank` that takes a `String` input and returns `true` if the input is `null` or `blank`.

```java
public static boolean isNullOrBlank(String input) {
    // TODO
}
```

## Task 2
Create a method called `invalidYear` that takes an `int` input and returns `true` if the input is less than your minimum production year (see your Car class).

```java
public static boolean invalidYear(int year) {
    // TODO
}
```

## Task 3
Create a method called `invalidPrice` that takes a double input and returns true if the input is less than the minimum price or greater than the maximum price (see your Car class).

```java
public static boolean invalidPrice(double price) {
    // TODO
}
```

## Task 4

Create a method called `invalidBodyType` that:

1. Takes a `String` input and capitalizes it.
2. Returns `true` if the input does not match one of the body types in the enum.

The second part is tricky but here's a hint: you can call `valueOf` from your enum. It returns an enum constant if it recognizes the string, otherwise, it will throw an `IllegalArgumentException`. In which case, catch the exception and return a boolean.

```java
public static boolean invalidBodyType(String bodyType) {
    // TODO
}
```

## Task 5
Create a method called `promptForBodyType` that takes a `Scanner` input and returns a valid body type entered by the user.

```java
public static BodyType promptForBodyType(Scanner scanner) {
    while (true) {
        System.out.print("\nPlease enter a valid car body type: ");
        String bodyType = scanner.nextLine();
        // TODO
    }
}
```


## Task 6

Create a method called `promptForMake` that takes a `Scanner` input and returns a valid `make` entered by the user.

```java
public static String promptForMake(Scanner scanner) {
    while (true) {
        System.out.print("\nPlease enter a valid car make: ");
        String make = scanner.nextLine();
        // TODO
    }
}
```

## Task 7
Create a method called `promptForModel` that takes a `Scanner` input and returns a valid `model` entered by the user.

```java
public static String promptForModel(Scanner scanner) {
    while (true) {
        System.out.print("\nPlease enter a valid car model: ");
        String model = scanner.nextLine();
        // TODO
    }
}
```

## Task 8
Create a method called `promptForYear` that takes a `Scanner` input and returns a valid production year entered by the user.

```java
public static int promptForYear(Scanner scanner) {
    while (true) {
        System.out.print("\nPlease enter a valid production year: ");
        // TODO
    }
}
```

## Task 9
Create a method called `promptForPrice` that takes a `Scanner` input and returns a valid price entered by the user.

```java
public static double promptForPrice(Scanner scanner) {
    while (true) {
        System.out.print("\nPlease enter a valid car price: ");
        // TODO
    }
}
```

## Task 10
Test the interactive methods in the main method.

```java
public static void main(String[] args) {
    Scanner scanner = new Scanner(System.in);

    String make = promptForMake(scanner);
    String model = promptForModel(scanner);
    BodyType bodyType = promptForBodyType(scanner);
    int year = promptForYear(scanner);
    double price = promptForPrice(scanner);

    Car newCar = new Car(make, model, bodyType, year, price);

    CarDealership dealership = new CarDealership();
    dealership.addCar(newCar);

    System.out.println("Car added to the dealership: " + newCar.getMake() + " " + newCar.getModel());
}

```

----------

##### Subscribe to our [YouTube Channel](https://www.youtube.com/@RayanSlim087?sub_confirmation=1) and Discover More Valuable Content!

