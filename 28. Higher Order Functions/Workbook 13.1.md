# Workbook 13.1

From the `Java Bootcamp Resources`, launch **starter**.

![starter.png](https://img-c.udemycdn.com/redactor/raw/article_lecture/2025-01-03_18-42-48-e972bb666fc3b9aa8e54201ab9e23930.png)

## Task 1

Use `forEach` to iterate the `ArrayList` and print the following messages.
```java
        System.out.println("Date: " + p.getDate().format(DateTimeFormatter.ofPattern("dd/MM/yyyy")));
        System.out.println("Amount: " + p.getAmount());
        System.out.println("---");
```
 Consider that `forEach` relies on a `Consumer` to perform its task.


| Functional Interface | Example |
| ----- | -------------------- |
| Consumer | `x -> { code } `|
| Predicate | `x  ->  { return boolean }`|
| Function | `x  ->  { return value }`|
| BiConsumer | `(x, y) -> { code }`|
| Comparator | `(x, y) -> { return int }`|
| BinaryOperator | `(x, y) -> { return value (same type) }`|


### **Expected Output**
```
Date: 01/01/2020
Amount: 100.0
---
Date: 15/02/2020
Amount: 200.0
---
Date: 30/03/2020
Amount: 300.0
---
Date: 01/04/2020
Amount: 50.0
---
Date: 15/05/2020
Amount: 75.0
---
Date: 30/06/2020
Amount: 100.0
---
```

----------

##### Your Path to Cloud-Native Engineering (After Learning Java)
###### 1. Develop Java Web Applications With Spring Boot → [Spring Boot Bootcamp](https://www.udemy.com/course/the-complete-spring-boot-development-bootcamp/?couponCode=SPRING_BOOTCAMP)
###### 2. Containerize and Deploy Web Applications with Docker → [Docker Bootcamp](https://www.udemy.com/course/docker-bootcamp-conquer-docker-with-real-world-projects/?couponCode=DOCKER_BOOTCAMP)
###### 3. Orchestrate Cloud Native Applications with Kubernetes → [Kubernetes Bootcamp](https://kubernetestraining.io/)