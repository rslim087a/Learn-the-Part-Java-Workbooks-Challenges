# Part 2

From the `Java Bootcamp Resources`, launch **`Part 2`**.

![2.png](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F4d714b6a-ae3f-4d16-8b31-70134b6710f6?alt=media&token=dd553cd9-af91-4185-b764-d504c82f628d)

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
##### Subscribe to our [YouTube Channel](https://www.youtube.com/@RayanSlim087?sub_confirmation=1) and Discover More Valuable Content!
