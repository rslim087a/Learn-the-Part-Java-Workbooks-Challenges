# Workbook 12.3

From the `Java Bootcamp Resources`, launch **starter**.

![starter.png](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F87bced44-2cd9-4db0-9a76-22125c478254?alt=media&token=7dc717de-b9d3-40c6-9ec2-32908aa28976)


## Task 1

The `Main` class contains two errors.
```
Line 18: The method getArea() is undefined for the type Shape
Line 19: The method getVolume() is undefined for the type Shape
```   
Define two `abstract` methods inside `Shape` to expose these behaviors.

## Task 2

It follows that children of `Shape` must define concrete implementations.
```
Cylinder must implement the inherited abstract method Shape.getArea()
Cylinder must implement the inherited abstract method Shape.getVolume()

Sphere must implement the inherited abstract method Shape.getArea()
Sphere must implement the inherited abstract method Shape.getVolume()
```
Use the following table to write equations for area and volume.

| Shape | Volume Formula | Surface Area Formula |
| ----- | -------------- | -------------------- |
| Cylinder | $V = \pi r^2h$ | $A = 2\pi r^2 + 2\pi rh$|
| Sphere | $V = \left(\frac{4}{3}\right) \pi r^3$	 | $A = 4\pi r^2$ |

----------

##### Subscribe to our [YouTube Channel](https://www.youtube.com/@RayanSlim087?sub_confirmation=1) and Discover More Valuable Content!