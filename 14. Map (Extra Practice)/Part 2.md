# Part 2

From the `Java Bootcamp Resources`, launch **`Part 2`**.

![2.png](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F4d714b6a-ae3f-4d16-8b31-70134b6710f6?alt=media&token=dd553cd9-af91-4185-b764-d504c82f628d)


## Task 1
Create a new file named `CityPopulationTracker.java`. Inside the file, create the `CityPopulationTracker` class.

```java
public class CityPopulationTracker {

}
```

The `CityPopulationTracker` class will define the following field:

```java
    private HashMap<String, City> cityPopulations;
```

## Task 2
Create a constructor for the `CityPopulationTracker` class that initializes the `cityPopulations` field to an empty `HashMap`.

## Task 3
Create a `getCity` method that takes a `city` name as a parameter and returns a deep copy of the `City` object associated with that city.

## Task 4
Create a `setCity` method that takes a `City` object as a parameter, and sets a deep copy of the `City` object in the `HashMap` with the corresponding city name as the key.

## Task 5
Create an `addCity` method that takes a `City` object as a parameter, and adds a deep copy of the `City` object to the `HashMap` with the corresponding city name as the key.

## Task 6
Test the `CityPopulationTracker` class by adding a few `City` objects, and then use the `getCity`, `setCity`, and `addCity` methods to manipulate the city data.

```java
public static void main(String[] args) {
    CityPopulationTracker tracker = new CityPopulationTracker();
    
    // Test the addCity method
    tracker.addCity(new City("New York", "USA", 8550405));
    tracker.addCity(new City("Los Angeles", "USA", 3971883));

    // Test the getCity method
    City nyCity = tracker.getCity("New York");
    System.out.println("Population of New York: " + nyCity.getPopulation());

    // Test the setCity method
    City updatedNyCity = new City("New York", "USA", 8600000);
    tracker.setCity(updatedNyCity);

    // Verify that the city data was updated
    nyCity = tracker.getCity("New York");
    System.out.println("Updated population of New York: " + nyCity.getPopulation());
}
```

## Task 7
Use breakpoints to inspect how the `CityPopulationTracker` class manages the `HashMap` of city names and `City` objects with deep copying when using the `getCity`, `setCity`, and `addCity` methods.


-----
##### Subscribe to our [YouTube Channel](https://www.youtube.com/@RayanSlim087?sub_confirmation=1) and Discover More Valuable Content!

