# Part 2

From the `Java Bootcamp Resources`, launch **`Part 2`**.

![2.png](https://img-c.udemycdn.com/redactor/raw/article_lecture/2025-01-03_18-48-01-8a70ce01c0857bab6a0ce8494abd74cd.png)

# Background

In this workbook, the focus is on **polymorphism**, which is one of the core principles of object-oriented programming. Polymorphism allows objects of different classes to be treated as objects of a common superclass. This makes it easier to create more flexible and reusable code.  In our example, the `Lab` class will manage both `Microscope` and `Centrifuge` objects by treating them as instances of their common superclass, `LabEquipment`.

## Task 1
Inside the `Lab` class, define an `ArrayList` field of `LabEquipment` objects:

```java
import java.util.ArrayList;

public class Lab {
                      // Polymorphism
    private ArrayList<LabEquipment> labEquipments; 
}
```
## Task 2
Create a constructor for the `Lab` class that initializes the `labEquipments` field to an empty ArrayList.

## Task 3

Create a copy constructor inside the `LabEquipment` class.

## Task 4

Create a copy constructor inside the `Centrifuge` class and inside the `Microscope` class.

## Task 5
Test your copy constructors. Use breakpoints to visualize the runtime.
```java
public static void main(String[] args) {
    Microscope microscope1 = new Microscope("Nikon", "E200", 2021, 1000);
    Centrifuge centrifuge1 = new Centrifuge("Eppendorf", "5424R", 2020, 15000);

    // Test the copy constructors
    Microscope microscopeCopy = new Microscope(microscope1);
    Centrifuge centrifugeCopy = new Centrifuge(centrifuge1);

    System.out.println("Original Microscope: " + microscope1.getManufacturer() + " " + microscope1.getModel());
    System.out.println("Copied Microscope: " + microscopeCopy.getManufacturer() + " " + microscopeCopy.getModel());
    
    System.out.println("Original Centrifuge: " + centrifuge1.getManufacturer() + " " + centrifuge1.getModel());
    System.out.println("Copied Centrifuge: " + centrifugeCopy.getManufacturer() + " " + centrifugeCopy.getModel());
```

## Task 6 (**Tricky!)**
Create a `getLabEquipment` method that takes an index as a parameter and returns a deep copy of the `LabEquipment` object at that index.

**Hints**: 
   1. Create an `abstract` method called `clone()` inside the parent class that returns a `LabEquipment` object. 
   2. Override the `clone()` method in each child class to return a copy of the **current object**.
   3. The abstract method exposes functionality that each child object is forced to override.


## Task 7
Create a `setLabEquipment` method that takes a `LabEquipment` object and an index as parameters and sets the `LabEquipment` object at the specified index to a deep copy of the given object.

## Task 8
Create an `addLabEquipment` method that takes a `LabEquipment` object as a parameter and adds a deep copy of the object to the `labEquipments` `ArrayList`.

## Task 9
Test the `Lab` class by creating a few Microscope and Centrifuge objects, initializing a `Lab` object with those lab equipments, and then using the `getLabEquipment`, `setLabEquipment`, and `addLabEquipment` methods to manipulate the lab equipments.

```java
public static void main(String[] args) {
    Microscope microscope1 = new Microscope("Nikon", "E200", 2021, 1000);
    Centrifuge centrifuge1 = new Centrifuge("Eppendorf", "5424R", 2020, 15000);

    // Test the copy constructors
    Microscope microscopeCopy = new Microscope(microscope1);
    Centrifuge centrifugeCopy = new Centrifuge(centrifuge1);

    System.out.println("Original Microscope: " + microscope1.getManufacturer() + " " + microscope1.getModel());
    System.out.println("Copied Microscope: " + microscopeCopy.getManufacturer() + " " + microscopeCopy.getModel());
    
    System.out.println("Original Centrifuge: " + centrifuge1.getManufacturer() + " " + centrifuge1.getModel());
    System.out.println("Copied Centrifuge: " + centrifugeCopy.getManufacturer() + " " + centrifugeCopy.getModel());

    Lab lab = new Lab();

    // Test the addLabEquipment method
    lab.addLabEquipment(microscope1);
    lab.addLabEquipment(centrifuge1);

    // Test the getLabEquipment method
    LabEquipment retrievedLabEquipment = lab.getLabEquipment(0);
    System.out.println("Retrieved Lab Equipment: " + retrievedLabEquipment.getManufacturer() + " " + retrievedLabEquipment.getModel());

    // Test the setLabEquipment method
    Microscope microscope2 = new Microscope("Olympus", "CX23", 2021, 400);
    lab.setLabEquipment(microscope2, 0);

    // Verify that the lab equipment was updated
    retrievedLabEquipment = lab.getLabEquipment(0);
    System.out.println("Updated Lab Equipment: " + retrievedLabEquipment.getManufacturer() + " " + retrievedLabEquipment.getModel());
}
}
```
## Task 10
Use breakpoints to inspect how the `Lab` class manages the ArrayList of `LabEquipment` objects.

----------

##### Your Path to Cloud-Native Engineering (After Learning Java)
###### 1. Develop Java Web Applications With Spring Boot → [Spring Boot Bootcamp](https://www.udemy.com/course/the-complete-spring-boot-development-bootcamp/?couponCode=SPRING_BOOTCAMP)
###### 2. Containerize and Deploy Web Applications with Docker → [Docker Bootcamp](https://www.udemy.com/course/docker-bootcamp-conquer-docker-with-real-world-projects/?couponCode=DOCKER_BOOTCAMP)
###### 3. Orchestrate Cloud Native Applications with Kubernetes → [Kubernetes Bootcamp](https://kubernetestraining.io/)