# Workbook 7.8

From the `Java Bootcamp Resources`, launch **`Workbook 7.8`**.

![8.png](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F0b5a5dca-1749-4a04-95af-97c263d910a8?alt=media&token=dfbcd52d-996f-411e-b309-db90eea4e7ba)

## Task 1
 Inside the `Airline`  `class`, add a constructor that does not receive any parameters.

## Task 2

Inside the constructor, set `people` equal to a `new` array that can store 11 `Person` objects.

## Task 3

Add a getter named `getPerson` that receives an `int index` and returns a `Person` object based on the index.

## Task 4 

Add a setter named `setPerson` that receives **one** parameter `Person person`.

```java
    /** Setter name: setPerson
     *
     * @param person
     *
     *
     *
     *
     * 
     */
```
Consider that the `people` array contains 11 elements, such that the index ranges from **0** to **10**.

```java
                      0       1       2       3       4       5       6       7       8       9      10
Person[] people = {Person, Person, Person, Person, Person, Person, Person, Person, Person, Person, Person};
```

The parameter `Person person` has a `seatNumber` that ranges from **1** to **11**.

![15.png](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F9260b652-db0f-46b8-81ab-4ad1512458f3?alt=media&token=35228c8e-07e9-4e80-a3f4-5632739c3463)

Use the `seatNumber` to index the array **without stepping out of bounds**. Set that element equal to the `Person` object.

```java
    /** Setter name: setPerson
     * @param person (Person)
     * 
     * Inside the setter:
     * 
     *   1. Index the array, and set that element equal to the Person object. 
     */
```

## Task 5

The starter code contains an array of `Person` objects. It also contains an object of the `Airline` class.

```java
    public static void main(String[] args) {
        Person[] people = new Person[] { 
            new Person("Cleopatra", "Egypt", "69 BC", 1),
            new Person("Alexander the Great", "Macedon", "356 BC", 2),
            new Person("Julius Caesar", "Rome", "100 BC", 3),
            new Person("Hannibal", "Carthage", "247 BC", 4),
            new Person("Confucius", "China", "551 BC", 5),
            new Person("Pericles", "Greece", "429 BC", 6),
            new Person("Spartacus", "Thrace", "111 BC", 7),
            new Person("Marcus Aurelius", "Rome", "121 AD", 8),
            new Person("Leonidas", "Greece", "540 BC", 9),
            new Person("Sun Tzu", "China", "544 BC", 10),
            new Person("Hammurabi", "Babylon", "1750 BC", 11),
        };
        Airline airline = new Airline();

    }
```
Use your `for` loop to populate the `airline` with objects from the array in `main()`.

##  Task 6

Print the objects at indices: **1**, **5**, **10**.

```java
    System.out.println(airline.getPerson(1));
    System.out.println(airline.getPerson(5));
    System.out.println(airline.getPerson(10));
```

**Output:**
```java
>>﻿: Name: Alexander the Great
>>﻿: Nationality: Macedon
>>﻿: Date of Birth: 356 BC
>>﻿: Seat Number: 2
>>﻿: Passport: [﻿null﻿, null﻿, null﻿]

>>﻿: Name: Pericles
>>: Nationali﻿ty: Greece
>>: Date of Bi﻿rth: 429 BC
>>: Seat Numbe﻿r: 6
>>: Passport: ﻿[null, null, ﻿null﻿]

>>﻿: Name: Hammurabi
>>: National﻿ity: Babylon
>>: Date of ﻿Birth: 1750 BC
>>: Seat Nu﻿mber: 11
>>: Passpo﻿rt: [null, nu﻿ll, ﻿null]
```

## Visualizing the Runtime

After you solve this workbook, I still recommend watching the video solution on Udemy.

![8.png](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F07ced564-0f95-45f0-8465-212d5973ac01?alt=media&token=5ae04e58-5262-497c-bff4-2037d11f588b)

It will show you how to visualize the runtime using Visual Studio Code.

----------

##### Subscribe to our [YouTube Channel](https://www.youtube.com/@RayanSlim087?sub_confirmation=1) and Discover More Valuable Content!