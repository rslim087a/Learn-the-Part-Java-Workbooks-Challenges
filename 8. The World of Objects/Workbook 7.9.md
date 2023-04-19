# Workbook 7.9

From the `Java Bootcamp Resources`, launch **`Workbook 7.9`**.

![9.png](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F5e9a77a4-1107-45e1-a281-ec9198402fd0?alt=media&token=04ffc3d2-0879-490f-9d69-ae37b7870baa)

## Task 1

Inside the `Airline` class, there is a method called `createReservation`. 

```java
    public void createReservation(Person person) {


    }
```
The method indexes an element (based on the seat number) and sets it equal to an object.

```java
    public void createReservation(Person person) {
        int index = person.getSeatNumber() - 1;  // seat number used as index.
        people[index] = new Person(person);      // indexed element is set equal to the object.
        System.out.println("Thank you " + person.getName() + " for flying with Java airlines. Your seat number is " + person.getSeatNumber() + ".\n");
    }
```
Inside the function, create a loop that keeps running **while** the spot in the array is *reserved* (indexed element is not `null`).

```java
    public void createReservation(Person person) {
        int index = person.getSeatNumber() - 1; 
        /*
            1. Loop that keeps running "while" the indexed element is not `null`.
	*/
        people[index] = new Person(person); 
        System.out.println("Thank you " + person.getName() + " for flying with Java airlines. Your seat number is " + person.getSeatNumber() + ".\n");
    }
```
**While** the loop is running, tell them that the spot is already taken:

```java
     System.out.println("\n" + person.getName() + ", seat: " + person.getSeatNumber() + " is already taken. Please choose another seat.\n");
```
**While** the loop is running, call `person.chooseSeat()` so that they "choose another seat".

```java
    person.chooseSeat(); 
```

Run your code.

```
>>: Thank you Cleopatra for flying with Java airlines. Your seat number is 1.
>>: Thank you Alexander the Great for flying with Java airlines. Your seat number is 2.
>>: Thank you Julius Caesar for flying with Java airlines. Your seat number is 3.
>>: Thank you Hannibal for flying with Java airlines. Your seat number is 4.
>>: Thank you Confucius for flying with Java airlines. Your seat number is 5.
>>: Thank you Pericles for flying with Java airlines. Your seat number is 6.
>>: Thank you Spartacus for flying with Java airlines. Your seat number is 7.
>>: Thank you Marcus Aurelius for flying with Java airlines. Your seat number is 8.
>>: Thank you Leonidas for flying with Java airlines. Your seat number is 9.
>>: Thank you Sun Tzu for flying with Java airlines. Your seat number is 10.
>>: Thank you Hammurabi for flying with Java airlines. Your seat number is 11.
```

## Task 2

Change Hammurabi's seat number to 10.

```java
Person[﻿] people = new Person﻿[﻿] {
  new Person﻿﻿﻿(﻿"Cleopatra"﻿, "Egypt"﻿, "69 BC"﻿, 1﻿)﻿,
  new Person﻿﻿﻿(﻿"Alexander the Great"﻿, "Macedon"﻿, "356 BC"﻿, 2﻿)﻿,
  new Person﻿﻿﻿(﻿"Julius Caesar"﻿, "Rome"﻿, "100 BC"﻿, 3﻿)﻿,
  new Person﻿﻿﻿(﻿"Hannibal"﻿, "Carthage"﻿, "247 BC"﻿, 4﻿)﻿,
  new Person﻿﻿﻿(﻿"Confucius"﻿, "China"﻿, "551 BC"﻿, 5﻿)﻿,
  new Person﻿﻿﻿(﻿"Pericles"﻿, "Greece"﻿, "429 BC"﻿, 6﻿)﻿,
  new Person﻿﻿﻿(﻿"Spartacus"﻿, "Thrace"﻿, "111 BC"﻿, 7﻿)﻿,
  new Person﻿﻿﻿(﻿"Marcus Aurelius"﻿, "Rome"﻿, "121 AD"﻿, 8﻿)﻿,
  new Person﻿﻿﻿(﻿"Leonidas"﻿, "Greece"﻿, "540 BC"﻿, 9﻿)﻿,
  new Person﻿(﻿"Sun Tzu"﻿, "China"﻿, "544 BC"﻿, 10﻿﻿﻿)﻿,
  new Person﻿(﻿"Hammurabi"﻿, "Babylon"﻿, "1750 ﻿B﻿C"﻿, 10)﻿, <--------
}﻿;
```
Because of your loop, Hammurabi keeps choosing a seat until they choose one that isn't taken.
```
Thank you Cleopatra for flying with Java airlines. Your seat number is 1. 
Thank you Alexander the Great for flying with Java airlines. Your seat number is 2. 
Thank you Julius Caesar for flying with Java airlines. Your seat number is 3.
Thank you Hannibal for flying with Java airlines. Your seat number is 4. 
Thank you Confucius for flying with Java airlines. Your seat number is 5. 
Thank you Pericles for flying with Java airlines. Your seat number is 6. 
Thank you Spartacus for flying with Java airlines. Your seat number is 7. 
Thank you Marcus Aurelius for flying with Java airlines. Your seat number is 8. 
Thank you Leonidas for flying with Java airlines. Your seat number is 9. 
Thank you Sun Tzu for flying with Java airlines. Your seat number is 10. 

Hammurabi, seat: 10 is already taken. Please choose another seat.
Hammurabi, seat: 6 is already taken. Please choose another seat.
Hammurabi, seat: 6 is already taken. Please choose another seat.
Hammurabi, seat: 2 is already taken. Please choose another seat.
Hammurabi, seat: 2 is already taken. Please choose another seat.
Hammurabi, seat: 2 is already taken. Please choose another seat.
Hammurabi, seat: 4 is already taken. Please choose another seat.
Thank you Hammurabi for flying with Java airlines. Your seat number is 11.
```

## Task 3

Inside the `for` loop, notice that each person is applying for a passport.

```java
boolean passportApproved = people[i].applyPassport();
```

If their passport is approved, update their passport using `setPassport`. **Then** create the reservation.
```java
if (passport is approved)
    - update their passport
    - createReservation
```
Otherwise, print the following message.
```java
    System.out.println("Sorry " + people[i].getName() + ". Your passport: " + Arrays.toString(people[i].getPassport()) + " is not valid.\n");  
```

**Your final output should appear as follows:**


```
>>: Sorry Cleopatra. Your passport: [null, null, null] is not valid.
>>: Thank you Alexander the Great for flying with Java airlines. Your seat number is 2.
>>: Thank you Julius Caesar for flying with Java airlines. Your seat number is 3.
>>: Thank you Hannibal for flying with Java airlines. Your seat number is 4.
>>: Sorry Confucius. Your passport: [null, null, null] is not valid.
>>: Thank you Pericles for flying with Java airlines. Your seat number is 6.
>>: Thank you Spartacus for flying with Java airlines. Your seat number is 7.
>>: Thank you Marcus Aurelius for flying with Java airlines. Your seat number is 8.
>>: Sorry Leonidas. Your passport: [null, null, null] is not valid.
>>: Thank you Sun Tzu for flying with Java airlines. Your seat number is 10.
>>: Hammurabi, seat: 10 is already taken. Please choose another seat.
>>: Hammurabi, seat: 7 is already taken. Please choose another seat.
>>: Thank you Hammurabi for flying with Java airlines. Your seat number is 9.
```



## Task 4
 
Feel free to admire the complexity of this application, yet how clean and expressive the code remains in `main()`. Therein lies the beauty of **Object-Oriented Programming!**

## Visualizing the Runtime

After you solve this workbook, I still recommend watching the video solution on Udemy.

![9.png](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F7e905481-4c24-4f08-bfcf-d8d24d428cab?alt=media&token=5e3bbcdf-6c03-4303-9396-53e8a05673ea)

It will show you how to visualize the runtime using Visual Studio Code.

----------
##### Subscribe to our [YouTube Channel](https://www.youtube.com/@RayanSlim087?sub_confirmation=1) and Discover More Valuable Content!