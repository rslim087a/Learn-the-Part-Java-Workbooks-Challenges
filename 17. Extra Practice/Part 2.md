# Part 2

From the `Java Bootcamp Resources`, launch **`Part 2`**.

![2.png](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F4d714b6a-ae3f-4d16-8b31-70134b6710f6?alt=media&token=dd553cd9-af91-4185-b764-d504c82f628d)

## Task 1

The `CarDealership` `class` will define an `ArrayList` of `Car` objects.

## Task 2
Create a constructor for the `CarDealership` class that initializes the `cars` field to an empty `ArrayList`.

## Task 3
Create a `getCar` method that takes an index as a parameter and returns a deep copy of the `Car` object at that index.

**Hint**: You must return to the Car class and give it a copy constructor.

## Task 4
Create a `setCar` method that takes a `Car` object and an index as parameters and sets the `Car `object at the specified index to a deep copy of the given object.

## Task 5
Create an `addCar` method that takes a `Car` object as a parameter and adds a deep copy of the object to the `cars` `ArrayList`.

## Task 6
Test the `CarDealership` class by creating a few Car objects, initializing a `CarDealership` object with those cars, and then using the `getCar`, `setCar`, and `addCar` methods to manipulate the cars.

```java
public static void main(String[] args) {
    Car car1 = new Car("Toyota", "Camry", BodyType.SEDAN, 2020, 30000);
    Car car2 = new Car("Honda", "Civic", BodyType.SEDAN, 2021, 25000);

    CarDealership dealership = new CarDealership();
    
    // Test the addCar method
    dealership.addCar(car1);
    dealership.addCar(car2);

    // Test the getCar method
    Car retrievedCar = dealership.getCar(0);
    System.out.println(retrievedCar.getMake() + " " + retrievedCar.getModel());

    // Test the setCar method
    Car newCar = new Car("Ford", "Mustang", BodyType.COUPE, 2022, 45000);
    dealership.setCar(newCar, 0);

    // Verify that the car was updated
    retrievedCar = dealership.getCar(0);
    System.out.println(retrievedCar.getMake() + " " + retrievedCar.getModel());
}
```

## Task 7
Use breakpoints to inspect how the CarDealership class manages the `ArrayList` of `Car` objects with deep copying when using the `getCar`, `setCar`, and `addCar` methods.

----------

##### Subscribe to our [YouTube Channel](https://www.youtube.com/@RayanSlim087?sub_confirmation=1) and Discover More Valuable Content!

