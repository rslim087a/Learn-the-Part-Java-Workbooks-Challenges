# Workbook 13.6

From the `Java Bootcamp Resources`, launch **starter**.

![starter.png](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F87bced44-2cd9-4db0-9a76-22125c478254?alt=media&token=7dc717de-b9d3-40c6-9ec2-32908aa28976)

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
###### 1. Create Enterprise Java Apps With Spring Boot → [Spring Boot Bootcamp](https://www.udemy.com/course/the-complete-spring-boot-development-bootcamp/?couponCode=SPRING_BOOTCAMP)
###### 2. Ship Code Like A Tech Giant With Docker → [Docker Bootcamp](https://www.udemy.com/course/docker-bootcamp-conquer-docker-with-real-world-projects/?couponCode=DOCKER_BOOTCAMP)
###### 3. Build Production-Grade Cloud Systems → [Kubernetes Bootcamp](https://kubernetestraining.io/)