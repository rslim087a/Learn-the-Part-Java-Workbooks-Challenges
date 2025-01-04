# Workbook 13.2

From the `Java Bootcamp Resources`, launch **starter**.

![starter.png](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F87bced44-2cd9-4db0-9a76-22125c478254?alt=media&token=7dc717de-b9d3-40c6-9ec2-32908aa28976)

## Task 1

Considering that `sort` relies on a `Comparator`, sort the `prices` in **descending** order.

| Functional Interface | Example |
| ----- | -------------------- |
| Consumer | `x -> { code } `|
| Predicate | `x  ->  { return boolean }`|
| Function | `x  ->  { return value }`|
| BiConsumer | `(x, y) -> { code }`|
| Comparator | `(x, y) -> { return int }`|
| BinaryOperator | `(x, y) -> { return value (same type) }`|


## Task 2
Use `forEach` to print each price in the sorted `List`.

### **Expected Output**

```
Prices
------
111.99
88.99
77.99
55.99
55.99
33.99
11.49
```

## Task 3

Sort the `books` `List` in **ascending** (alphabetical) order.


## Task 4

Use `forEach` to print each book in the sorted `List`.

```
Library
--------
Moby-Dick
One Hundred Years of Solitude
Pride and Prejudice
The Alchemist
The Brothers Karamazov
The Catcher in the Rye
The Great Gatsby
The Lord of the Rings
The Picture of Dorian Gray
To Kill a Mockingbird
```
----------

##### Your Path to Cloud-Native Engineering (After Learning Java)
###### 1. Create Enterprise Java Apps With Spring Boot → [Spring Boot Bootcamp](https://www.udemy.com/course/the-complete-spring-boot-development-bootcamp/?couponCode=SPRING_BOOTCAMP)
###### 2. Ship Code Like A Tech Giant With Docker → [Docker Bootcamp](https://www.udemy.com/course/docker-bootcamp-conquer-docker-with-real-world-projects/?couponCode=DOCKER_BOOTCAMP)
###### 3. Build Production-Grade Cloud Systems → [Kubernetes Bootcamp](https://kubernetestraining.io/)