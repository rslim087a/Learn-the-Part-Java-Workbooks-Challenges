# Part 2

From the `Java Bootcamp Resources`, launch **`Part 2`**.

![2.png](https://img-c.udemycdn.com/redactor/raw/article_lecture/2025-01-03_22-26-24-e01edb91ebfa86f2335f6ed4398b259d.png)

## Task 1
Create a new file named `MagazineLibrary`.java. Inside the file, create the MagazineLibrary class.

```java
public class MagazineLibrary {

}
```

The MagazineLibrary class will define the following field:

```java
    private ArrayList<Magazine> magazines;
```

## Task 2
Create a constructor for the `MagazineLibrary` class that initializes the `magazines` field to an empty ArrayList.

## Task 3
Create a `getMagazine` method that takes an index as a parameter and returns a deep copy of the Magazine object at that index.


**Hint**: You must return to the `Magazine` class and give it a copy constructor. 

## Task 4
Create a `setMagazine` method that takes a Magazine object and an index as parameters and sets the Magazine object at the specified index to a deep copy of the given object.

## Task 5
Create an `addMagazine` method that takes a Magazine object as a parameter and adds a deep copy of the object to the magazines `ArrayList`.

## Task 6
Test the `MagazineLibrary` class by creating a few `Magazine` objects, initializing a `MagazineLibrary` object with those magazines, and then using the `getMagazine`, `setMagazine`, and `addMagazine` methods to manipulate the magazines.

```java
public static void main(String[] args) {
    Magazine magazine1 = new Magazine("Magazine 1", "Publisher 1", 1, 2020);
    Magazine magazine2 = new Magazine("Magazine 2", "Publisher 2", 2, 2021);

    MagazineLibrary library = new MagazineLibrary();
    
    // Test the addMagazine method
    library.addMagazine(magazine1);
    library.addMagazine(magazine2);

    // Test the getMagazine method
    Magazine retrievedMagazine = library.getMagazine(0);
    System.out.println(retrievedMagazine.getTitle());

    // Test the setMagazine method
    Magazine newMagazine = new Magazine("Magazine 3", "Publisher 3", 3, 2022);
    library.setMagazine(newMagazine, 0);

    // Verify that the magazine was updated
    retrievedMagazine = library.getMagazine(0);
    System.out.println(retrievedMagazine.getTitle());
}
```

## Task 7
Use breakpoints to inspect how the `MagazineLibrary` class manages the `ArrayList` of `Magazine` objects with deep copying when using the `getMagazine`, `setMagazine`, and `addMagazine` methods.

-----
##### **Go From Zero to DevOps Master**: *[Java → Spring Boot → Docker → Kubernetes](https://rslim087a.github.io/zero-devops-roadmap/)*