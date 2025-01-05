# Part 2

From the `Java Bootcamp Resources`, launch **`Part 2`**.

![2.png](https://img-c.udemycdn.com/redactor/raw/article_lecture/2025-01-03_22-48-26-034dd97d10e3824d3feabf695ddd5a4b.png)

## **Task 1**

Modify the `Contact` class by removing the `age` parameter from the constructor.

```java
    public Contact(String name, String phoneNumber, String birthDate) {
        this.name = name;
        this.phoneNumber = phoneNumber;
        this.birthDate = birthDate;
        // Remove the age update
    }
```
Age will be derived from the `birthDate` that is passed in.


## Task 2 

This task provides an excellent opportunity to practice navigating the web to search documentation and find resources.

### Part 1

Create a `toAge` method that converts the `birthDate` string to an age.


```java
public int toAge(String birthDate) {
    // Your implementation here
}
```

### Part 2
`LocalDate` makes it really easy to work with dates. 

Convert the `String` into a LocalDate using the [**`LocalDate.parse` method**](https://docs.oracle.com/javase/8/docs/api/java/time/LocalDate.html#parse-java.lang.CharSequence-java.time.format.DateTimeFormatter-). Ensure that the `LocalDate` follows the pattern `yyyy-MM-dd`.

```java
public int toAge(String birthDate) {
    // 1. Convert birthDate String to LocalDate
}
```

### Part 3

Define a `LocalDate` object representing the current date using the [**`LocalDate.now` method**](https://docs.oracle.com/javase/8/docs/api/java/time/LocalDate.html#now--).

```java
public int toAge(String birthDate) {
    // 1. Convert birthDate String to LocalDate
    // 2. Get the current date
}
```

### Part 4

Define a `Period` object representing the period between two dates using the [**`Period.between` method**](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/time/Period.html#between(java.time.LocalDate,java.time.LocalDate))

```java
public int toAge(String birthDate) {
    // 1. Convert birthDate String to LocalDate
    // 2. Get the current date
    // 3. Calculate the period between both dates
}
```

### Part 5
Extract the number of years from the `Period` object and return it using the [**`Period.getYears` method**](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/time/Period.html#getYears())

```java
public int toAge(String birthDate) {
    // 1. Convert birthDate String to LocalDate
    // 2. Get the current date
    // 3. Calculate the period between both dates
    // 4. Return the number of years
}
```

## Task 3

Modify the constructor to update the `age` field by calling `toAge` and passing in the `birthDate`.


## Task 4

Use breakpoints to visualize the runtime of the `age` field being updated automatically from the `birthDate`.


## Task 5

Update the `birthDate` of one of the previously created objects:

```java
public static void main(String[] args) {
    // contacts from before
    contact1.setBirthDate("1989-01-01");
}

```
## Task 6

The `age` should be automatically updated once the `birthDate` is updated, so make `setAge` `private`, as it should not be accessible outside of this class. 

We only need to call `setAge` from `setBirthDate` so that `age` is automatically updated when the `birthDate` is updated.


## Task 7

Use breakpoints to visualize the runtime of the person's 	`birthDate` and `age` updating simultaneously.

----------
##### Your Path to Cloud-Native Engineering (After Learning Java)
###### 1. Develop Java Web Applications With Spring Boot → [Spring Boot Bootcamp](https://www.udemy.com/course/the-complete-spring-boot-development-bootcamp/?couponCode=SPRING_BOOTCAMP)
###### 2. Containerize and Deploy Web Applications with Docker → [Docker Bootcamp](https://www.udemy.com/course/docker-bootcamp-conquer-docker-with-real-world-projects/?couponCode=DOCKER_BOOTCAMP)
###### 3. Orchestrate Cloud Native Applications with Kubernetes → [Kubernetes Bootcamp](https://kubernetestraining.io/)
