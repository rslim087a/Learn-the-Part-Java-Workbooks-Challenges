# Workbook 13.6

From the `Java Bootcamp Resources`, launch **starter**.

![starter.png](https://img-c.udemycdn.com/redactor/raw/article_lecture/2025-01-03_18-25-35-803e9dc16d1839b670faeb221c2b78c0.png)

## Task 1
```java
List<String> names = Arrays.asList("Alice", "Bob", "Charlie", "Dave");
```

**1.  `map`**: transform each name into this greeting `"Hello, " + name + "!"`.

**2. `forEach`**: print every greeting in the stream.

```
>>: Hello, Alice!
>>: Hello, Bob!
>>: Hello, Charlie!
>>: Hello, Dave!
```

## Task 2
```java
 List<String> usernames = Arrays.asList("sparklingunicorn", "galactic_goddess", "neon_ninja", "purplepixiedust");
```

**1. `filter`**: keep the username that matches `neon_ninja`.

**2. `findFirst().orElse(null)`**: return the first element in the stream.


```
>>: Found you: neon_ninja
```

## Task 3

```java
List<Integer> numbers = Arrays.asList(1, 2, 3, 4, 5, 6);
```

**1. `filter`**: keep the numbers that are even.

**2. `count()`**: count the number of elements in the stream.


```
>>: There are 3 even numbers in this list
```

--------
##### Your Path to Cloud-Native Engineering (After Learning Java)
###### 1. Develop Java Web Applications With Spring Boot → [Spring Boot Bootcamp](https://www.udemy.com/course/the-complete-spring-boot-development-bootcamp/?couponCode=SPRING_BOOTCAMP)
###### 2. Containerize and Deploy Web Applications with Docker → [Docker Bootcamp](https://www.udemy.com/course/docker-bootcamp-conquer-docker-with-real-world-projects/?couponCode=DOCKER_BOOTCAMP)
###### 3. Orchestrate Cloud Native Applications with Kubernetes → [Kubernetes Bootcamp](https://kubernetestraining.io/)