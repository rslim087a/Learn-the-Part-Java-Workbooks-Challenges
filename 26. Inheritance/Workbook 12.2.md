# Workbook 12.2

From the `Java Bootcamp Resources`, launch **starter**.

![starter.png](https://img-c.udemycdn.com/redactor/raw/article_lecture/2025-01-03_18-51-08-03692470427bec5370be2f17c37199e7.png)

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

##### **Go From Zero to DevOps Master**: *[Java → Spring Boot → Docker → Kubernetes](https://rslim087a.github.io/zero-devops-roadmap/)*