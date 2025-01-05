# Part 2

From the `Java Bootcamp Resources`, launch **`Part 2`**.

![2.png](https://img-c.udemycdn.com/redactor/raw/article_lecture/2025-01-03_19-00-46-88db7a5f544b37750e972d6ac4784359.png)

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

##### Your Path to Cloud-Native Engineering (After Learning Java)
###### 1. Develop Java Web Applications With Spring Boot → [Spring Boot Bootcamp](https://www.udemy.com/course/the-complete-spring-boot-development-bootcamp/?couponCode=SPRING_BOOTCAMP)
###### 2. Containerize and Deploy Web Applications with Docker → [Docker Bootcamp](https://www.udemy.com/course/docker-bootcamp-conquer-docker-with-real-world-projects/?couponCode=DOCKER_BOOTCAMP)
###### 3. Orchestrate Cloud Native Applications with Kubernetes → [Kubernetes Bootcamp](https://kubernetestraining.io/)

