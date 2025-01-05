# Workbook 10.1

From the `Java Bootcamp Resources`, launch **`starter`**.

![starter.png](https://img-c.udemycdn.com/redactor/raw/article_lecture/2025-01-03_19-04-44-1f96398f7b9b87fb54ee97e1bce870e8.png)

## Task 1

The `details()` method contains many loose integers.
```java
"\nCourt length (feet): " + 94 + 
"\nRim height (feet): " + 10 + 
"\nDistance from three-point arc: " + 23 + 
"\nPoints awarded beyond the three-point arc: " + 3 +
"\nPoints awarded inside the three-point arc: " + 2 +
"\nPoints awarded from a free throw: " + 1 + 
"\nLength of each quarter (minutes): " + 12 +
"\nSeconds to attempt shot after gaining possession: " + 24;
```
Create eight constants inside `Regulation` and use them inside the `Game` class.
```java
public class Regulation {

    COURT_LENGTH
    RIM_HEIGHT
    THREE_POINT_DISTANCE
    BEYOND_THREE_POINT_ARC
    INSIDE_THREE_POINT_ARC 
    FREE_THROW
    QUARTER_LENGTH
    POSSESSION_TIME 

}
```

----------
##### Your Path to Cloud-Native Engineering (After Learning Java)
###### 1. Develop Java Web Applications With Spring Boot → [Spring Boot Bootcamp](https://www.udemy.com/course/the-complete-spring-boot-development-bootcamp/?couponCode=SPRING_BOOTCAMP)
###### 2. Containerize and Deploy Web Applications with Docker → [Docker Bootcamp](https://www.udemy.com/course/docker-bootcamp-conquer-docker-with-real-world-projects/?couponCode=DOCKER_BOOTCAMP)
###### 3. Orchestrate Cloud Native Applications with Kubernetes → [Kubernetes Bootcamp](https://kubernetestraining.io/)