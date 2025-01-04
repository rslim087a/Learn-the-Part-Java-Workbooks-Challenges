# Workbook 13.3

From the `Java Bootcamp Resources`, launch **starter**.

![starter.png](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F87bced44-2cd9-4db0-9a76-22125c478254?alt=media&token=7dc717de-b9d3-40c6-9ec2-32908aa28976)

## Task 1

Use `forEach` to iterate the `HashMap` and print the following message.
```java
System.out.println(sku + "\t" + item.getPrice() + "\t" + item.getName())
```
 Consider that it will rely on a `BiConsumer` to perform its task.

| Functional Interface | Example |
| ----- | -------------------- |
| Consumer | `x -> { code } `|
| Predicate | `x  ->  { return boolean }`|
| Function | `x  ->  { return value }`|
| BiConsumer | `(x, y) -> { code }`|
| Comparator | `(x, y) -> { return int }`|
| BinaryOperator | `(x, y) -> { return value (same type) }`|

### Expected Output
```
SKU             Price   Item
DOFO-008        10.0    Super Doo-dad
THNG-003        2.99    Thingamajig
WIDG-005        6.99    Super Widget
GADG-006        8.99    Super Gadget
THNG-007        15.0    Super Thingamajig
WIDG-001        3.99    Widget
GADG-002        5.99    Gadget
DBOO-004        4.99    Doo-dad
```

----------

##### Your Path to Cloud-Native Engineering (After Learning Java)
###### 1. Create Enterprise Java Apps With Spring Boot → [Spring Boot Bootcamp](https://www.udemy.com/course/the-complete-spring-boot-development-bootcamp/?couponCode=SPRING_BOOTCAMP)
###### 2. Ship Code Like A Tech Giant With Docker → [Docker Bootcamp](https://www.udemy.com/course/docker-bootcamp-conquer-docker-with-real-world-projects/?couponCode=DOCKER_BOOTCAMP)
###### 3. Build Production-Grade Cloud Systems → [Kubernetes Bootcamp](https://kubernetestraining.io/)