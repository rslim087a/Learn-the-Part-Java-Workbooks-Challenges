# Workbook 7.6

From the `Java Bootcamp Resources`, launch **`Workbook 7.6`**.

![6.png](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2Ffbeacc15-b89a-4783-a96f-280dbe6aca26?alt=media&token=8966c00c-5804-494a-a84a-d88cc3c0fc73)

## **Task 1**

Your constructor will **not** receive a passport parameter. 
```java
    public Person(String name, String nationality, String dateOfBirth, int seatNumber) {
        // ...
    }
```
But it must set `passport` equal to an array that stores 3 elements.

```java
    public Person(String name, String nationality, String dateOfBirth, int seatNumber) {
        // ...
        this.passport = new String[3];
    }
```
We do this because we cannot update their passport until they apply for it.

## **Task 2**

Add the getter `getPassport()`. Make sure it returns a **copy** of the array.

## Task 3
Add this `println()` function at the end of your `main()` method. Replace the placeholders where appropriate.
```java
System.out.println("Name: " + <name field> + "\n" + 
"Nationality: " + <nationality field > + "\n" + 
"Date of Birth: " + <birth date field> + "\n" +
"Seat Number: " + <seat field> + "\n" + "Passport: " +
 <toString of passport field> + "\n");
```


**Your output should appear as follows:**

```java
>>﻿: Name: Rayan Slim
>>﻿: Nationality: Canadian
>>﻿: Date of Birth: 01﻿/﻿01﻿/﻿1111
>>﻿: Seat Number: 5
>>﻿: Passport: [﻿null﻿, null﻿, null﻿]
```

**Task 4**
-------------------
Your code contains a setter `setPassport`. Notice that it doesn't have a parameter.
```java
    public void setPassport() {
        
    }
```
Inside `setPassport`, set `passport` equal to  `{name, nationality, dateOfBirth}`.

**Task 5**
----------------------------

Call the setter if the person gets approved for a passport.

**Test Case:** Passport Approved.

```java
>>﻿: Name: Rayan Slim
>>﻿: Nationality: Canadian
>>﻿: Date of Birth: 01﻿/﻿01﻿/﻿1111
>>﻿: Seat Number: 5
﻿>>﻿: Passport: [Rayan Sl﻿im, Canadian, 01/01/1111]
```

**Test Case:** Passport Denied.

```java
>>﻿: Name: Rayan Slim
>>﻿: Nationality: Canadian
>>﻿: Date of Birth: 01﻿/﻿01﻿/﻿1111
>>﻿: Seat Number: 5
>>﻿: Passport: [﻿null﻿, null﻿, null﻿]
```

Keep running your code and make sure you get alternating outputs.

## Visualizing the Runtime

After you solve this workbook, I still recommend watching the video solution on Udemy.

![6.png](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2Fe1f73bc1-9499-47ab-a381-9690427cf8f2?alt=media&token=cf881588-392b-48a5-ae65-7fb111ab7fbf)

It will show you how to visualize the runtime using Visual Studio Code.

----------

##### Subscribe to our [YouTube Channel](https://www.youtube.com/@RayanSlim087?sub_confirmation=1) and Discover More Valuable Content!