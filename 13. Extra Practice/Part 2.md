# Part 2

From the `Java Bootcamp Resources`, launch **`Part 2`**.

![2.png](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F4d714b6a-ae3f-4d16-8b31-70134b6710f6?alt=media&token=dd553cd9-af91-4185-b764-d504c82f628d)

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
##### Subscribe to our [YouTube Channel](https://www.youtube.com/@RayanSlim087?sub_confirmation=1) and Discover More Valuable Content!