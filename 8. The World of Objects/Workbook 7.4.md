# Workbook 7.4

From the `Java Bootcamp Resources`, launch **`Workbook 7.4`**.

![4.png](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2Ff2c3be38-46f6-485b-9f8e-03057a8bf3b5?alt=media&token=00c3f19a-a819-44b2-b582-f47a580030b3)

## **Task 1**

Inside the `Person` class, add a copy constructor.

## **Task 2**
Your code contains a `Person` object.

```java
    Person person = new Person("Rayan Slim", "Canadian", "01/01/1111", 5);
```
That person's twin is also flying with Java airlines. Use this code to test your copy constructor.

```java
    Person twin = new Person(person); // creates a copy of the first object.
    twin.setName("Jad Slim"); // updates name field of the second object.
    twin.setSeatNumber(3); // updates the seat number of the second object.
```
Print the other person's fields as well.

```java
    System.out.println("Name: " + twin.getName() + "\n" + "Nationality: " + twin.getNationality() + "\n" + "Date of Birth: " + twin.getDateOfBirth() + "\n" + "Seat Number: " + twin.getSeatNumber() + "\n");
```

```java
Name: Rayan Slim
Nationality: Canadian
Date of Birth: 01/01/1111
Seat Number: 10

Name: Jad Slim
Nationality: Canadian
Date of Birth: 01/0﻿1﻿/1﻿1﻿11
Seat Number: 3
```

## Visualizing the Runtime

After you solve this workbook, I still recommend watching the video solution on Udemy.

![4.png](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2Ff6e8aee8-43a4-43b8-b0f6-c53f12572d68?alt=media&token=b13a38b7-4f44-496e-8a22-f5d706426f28)

It will show you how to visualize the runtime using Visual Studio Code.

----------
##### Subscribe to our [YouTube Channel](https://www.youtube.com/@RayanSlim087?sub_confirmation=1) and Discover More Valuable Content!