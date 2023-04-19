# Workbook 12.2

From the `Java Bootcamp Resources`, launch **starter**.

![starter.png](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F87bced44-2cd9-4db0-9a76-22125c478254?alt=media&token=7dc717de-b9d3-40c6-9ec2-32908aa28976)

## Task 1

Create a constructor inside `Shape` that updates the `radius` of the **current object**.


## Task 2

Create a constructor inside `Cylinder` that invokes the parent constructor and updates `height`.

## Task 3

Create a constructor inside `Sphere` that invokes the parent constructor.

## Task 4

Add this code to your `main()` method and feel free to visualize the runtime.


```java
        Cylinder cylinder = new Cylinder(1.0, 2.0);
        Sphere sphere = new Sphere(1.0);

        System.out.println("Sphere - radius: " + sphere.getRadius());
        System.out.println("Cylinder - radius: " + cylinder.getRadius() + " height " + cylinder.getHeight());
```
----------

##### Subscribe to our [YouTube Channel](https://www.youtube.com/@RayanSlim087?sub_confirmation=1) and Discover More Valuable Content!