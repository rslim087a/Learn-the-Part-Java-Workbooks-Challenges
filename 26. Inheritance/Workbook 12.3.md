# Workbook 12.3

From the `Java Bootcamp Resources`, launch **starter**.

![starter.png](https://img-c.udemycdn.com/redactor/raw/article_lecture/2025-01-03_18-51-08-03692470427bec5370be2f17c37199e7.png)


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

##### **Go From Zero to DevOps Master**: *[Java → Spring Boot → Docker → Kubernetes](https://rslim087a.github.io/zero-devops-roadmap/)*