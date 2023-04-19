# Part 1

From the `Java Bootcamp Resources`, launch **`Part 1`**.

![1.png](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F85391d27-5dd8-4a8b-9a15-271f727a3ca6?alt=media&token=4f1b90ab-38ed-4272-abff-b4bcb4c59f87)

## Task 1

The Car class defines the following fields:

```java
    private String make;
    private String model;
    private String bodyType;  // Should this really be a String.
    private int productionYear;
    private double price;
```
Instead of using a `String` data type for `bodyType`, consider the following scenario: 
we want to throw an error if the value passed into the constructor or setters is anything other than `SEDAN`, `COUPE`, `HATCHBACK`, `SUV`, `TRUCK`, and `VAN`. Using a `String` might lead to messy exception handling because we would have to check all of these inputs every time we get a value in the constructor and setter, like this:

```java
if (!input.equals("SEDAN") && !input.equals("COUPE") && !input.equals("HATCHBACK") && !input.equals("SUV") && !input.equals("TRUCK") && !input.equals("VAN")) {
    throw new IllegalArgumentException("Invalid body type");
}
```
So, how can we restrict the `bodyType` that gets passed in to be limited only to these values (aside from the possibility of it being `null`) so that we don't have to worry about exception handling?

## Task 2

Create getter and setter methods for each field of the `Car` class. Ensure that the setter methods perform the following argument validations and throw an `IllegalArgumentException` with an appropriate error message if the input is invalid:

- `setMake` method:

   - Check if the input `make` is `null` or `blank`.
   - If the validation fails, throw an `IllegalArgumentException` with the message `"Make cannot be null or blank."`

- `setModel` method:

   - Check if the input `model` is `null` or `blank`.
   - If the validation fails, throw an `IllegalArgumentException` with the message `"Model cannot be null or blank."`

- `setBodyType` method:

   - Check if the input `bodyType` is `null`.
   - If the validation fails, throw an `IllegalArgumentException` with the message `"BodyType cannot be null."`

- `setProductionYear` method:

   - Check if the input `productionYear` is less than the minimum year (e.g., `1900`). Do not use loose integers in your code. Use `static` `final` constants instead.
   - If the validation fails, throw an `IllegalArgumentException` with the message `"Production year must be greater than or equal to the minimum year."`

- `setPrice` method:

   - Check if the input `price` is less than `0` or greater than `200,000`. Do not use loose integers in your code. Use `static` `final` constants instead.
   - If the validation fails, throw an `IllegalArgumentException` with the message `"Price must be within a valid range."`

After implementing the setter methods with the appropriate validations, create the corresponding getter methods for each field.

## Task 3

Create a constructor that initializes the fields of a newly created object by calling the setter methods.

```java
public Car(String make, String model, BodyType bodyType, int productionYear, double price) {
    setMake(make);
    setModel(model);
    setBodyType(bodyType);
    setProductionYear(productionYear);
    setPrice(price);
}
```

Using the setter methods in the constructor ensures that the argument validation is performed in a single place, keeping the code DRY (Don't Repeat Yourself).

## Task 4

Test your constructor and getter/setter methods by creating instances (objects) of the Car class. Uncomment each test one by one to ensure that the methods throw an IllegalArgumentException when the input is invalid. Remember to re-comment the test before moving on to the next one.

```java
public static void main(String[] args) {
    Car car1 = new Car("Toyota", "Camry", BodyType.SEDAN, 2020, 30000);
    System.out.println(car1.getMake());

    // Uncomment the following line to test invalid input for setMake method
    // car1.setMake("");

    // Uncomment the following line to test invalid input for setModel method
    // car1.setModel("");

    // Uncomment the following line to test invalid input for setBodyType method
    // car1.setBodyType(null);

    // Uncomment the following line to test invalid input for setProductionYear method
    // car1.setProductionYear(1899);

    // Uncomment the following line to test invalid input for setPrice method
    // car1.setPrice(-1);

    // Uncomment the following line to test invalid input for setPrice method
    // car1.setPrice(200001);

    // Uncomment the following line to test invalid input for the constructor
    // Car car2 = new Car("", "Camry", BodyType.SEDAN, 2020, 30000);
}
```

-----
##### Subscribe to our [YouTube Channel](https://www.youtube.com/@RayanSlim087?sub_confirmation=1) and Discover More Valuable Content!