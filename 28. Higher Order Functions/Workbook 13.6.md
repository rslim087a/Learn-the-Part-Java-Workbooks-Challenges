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
##### **Go From Zero to DevOps Master**: *[Java → Spring Boot → Docker → Kubernetes](https://rslim087a.github.io/zero-devops-roadmap/)*