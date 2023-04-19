# Part 1

From the `Java Bootcamp Resources`, launch **`Part 1`**.

![1.png](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F85391d27-5dd8-4a8b-9a15-271f727a3ca6?alt=media&token=4f1b90ab-38ed-4272-abff-b4bcb4c59f87)


## Task 1
Create a new file named `City.java`. Inside the file, create the City class.

```java
public class City {

}
```
The City class will define the following fields:

```java
    private String name;
    private String country;
    private long population;
```

## Task 2
Create getter and setter methods for each field of the `City` class. Ensure that the setter methods perform the following argument validations and throw an `IllegalArgumentException` with an appropriate error message if the input is invalid:

- `setName` method:

   - Check if the input `name` is `null` or `blank`.
   - If the validation fails, throw an `IllegalArgumentException` with the message `"Name cannot be null or blank."`

- `setCountry` method:

   - Check if the input `country` is `null` or `blank`.
   - If the validation fails, throw an `IllegalArgumentException` with the message `"Country cannot be null or blank."`

 - `setPopulation` method:

    - Check if the input `population` is less than or equal to 0.
    - If the validation fails, throw an `IllegalArgumentException` with the message `"Population must be greater than 0."`

After implementing the setter methods with the appropriate validations, create the corresponding getter methods for each field.

## Task 3
Create a constructor that initializes the fields of a newly created object by calling the setter methods.

``` java
public City(String name, String country, long population) {
    setName(name);
    setCountry(country);
    setPopulation(population);
}
```

Using the setter methods in the constructor ensures that the argument validation is performed in a single place, keeping the code DRY (Don't Repeat Yourself).

## Task 4
Test your constructor and getter/setter methods by creating instances (objects) of the City class. Uncomment each test one by one to ensure that the methods throw an `IllegalArgumentException` when the input is invalid. Remember to re-comment the test before moving on to the next one.

```java
public static void main(String[] args) {
    City city1 = new City("New York", "USA", 8500000);
    System.out.println(city1.getName());

    // Uncomment the following line to test invalid input for setName method
    // city1.setName("");

    // Uncomment the following line to test invalid input for setCountry method
    // city1.setCountry("");

    // Uncomment the following line to test invalid input for setPopulation method
    // city1.setPopulation(-1);

    // Uncomment the following line to test invalid input for the constructor
    // City city2 = new City("", "USA", 8500000);
}
```
When testing each method, the program will throw an `IllegalArgumentException` if the input is invalid. This helps us to identify mistakes in our application and fix the issues, preventing the creation of objects with an invalid state that could lead to unexpected behavior or errors during program execution.

-----
##### Subscribe to our [YouTube Channel](https://www.youtube.com/@RayanSlim087?sub_confirmation=1) and Discover More Valuable Content!


