# Workbook 7.5

From the `Java Bootcamp Resources`, launch **`Workbook 7.5`**.

![5.png](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F05e991af-ee0f-4320-a794-d637854b1833?alt=media&token=8d629d2f-9a9a-45c4-897d-87e2c0d91a4f)

## Task 1

Inside the `Person` class, define a function called `applyPassport`.

```java
/**
 *  Function name: applyPassport
 * 
 *
 *  
 *     
 */
```
The function returns a `boolean` and does not expect parameters.

```java
/**
 *  Function name: applyPassport
 *  @return (boolean)    <----
 *
 * 
 *     
 */
```

This code randomly returns 0 or 1.

```java
int number = (int) (Math.random() * 2);  //random int that can be 0 or 1.
```

Use this code to return `true` if the number equals `1`, and `false` otherwise. 

```java
/**
 *  Function name: applyPassport
 *  @return (boolean)
 *
 *  Inside the function:
 *     1. Returns a random boolean of true or false.
 */
```

Do not use `if` - `else` to accomplish this task.

![24.png](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F3a1b962b-f6b5-47de-82d1-33499ccec9f0?alt=media&token=4a56e3a8-e23c-4e73-bbc7-8b974d38a17d)

## **Task 2**

Inside the `Person` class, define a function called `chooseSeat`.

```java
/**
 *  Function name: chooseSeat
 *
 * 
 *   
 */
```
This code returns a random number between 1 and 11.
```java
(int) (Math.random() * 11 + 1); 
```
`chooseSeat` must use this code to update `this.seat` with a random seat.

```java
/**
 *  Function name: chooseSeat
 *
 *  Inside the function:
 *    1. Sets this.seat to a random number between 1 -- 11.
 */
```

## Task 3

Your starter project should contain one object.

```java
    Person person = new Person("Rayan Slim", "Canadian", "01/01/1111", 5);
```

Call `applyPassport` from your object. If the function returns `true`:

```java
    System.out.println("Congratulations " + person.getName() + ". Your passport was approved!");
```

Otherwise:

```java
    System.out.println("We are sorry " + person.getName() + ". We cannot process your application.");
```

**Example Output 1:**

```java
>>﻿: Name: Rayan Slim
>>﻿: Nationality: Canadian
>>﻿: Date of Birth: 01﻿/﻿01﻿/﻿1111
>>﻿: Seat Number: 10

﻿>>﻿: Congratulations Ray﻿an Slim. Your passport was﻿ approved!
```

**Example Output 2:**

```
>>: Name: Rayan Slim
>>: Nationality: Canadian
>>: Date of Birth: 01﻿/﻿01﻿/﻿1111
>>: Seat Number: 10

>>: We are sorry Rayan S﻿lim. We cannot process you﻿r application.
```

Run your code multiple times. Each run should output a random result.

## Task 4.

Unfortunately the person's seat is already taken. Your object must call `chooseSeat` to "choose another seat".


**Example Output 1**

```java
>>﻿: Name: Rayan Slim
>>﻿: Nationality: Canadian
>>﻿: Date of Birth: 01﻿/﻿01﻿/﻿1111
﻿>>﻿: Seat Number: 10

﻿>>﻿: Congratulations Ray﻿an Slim. Your passport was﻿ approved!
```

**Example Output 2**

```java
>>﻿: Name: Rayan Slim
>>﻿: Nationality: Canadian
>>﻿: Date of Birth: 01﻿/﻿01﻿/﻿1111
>>﻿: Se﻿at Number: 10

>﻿>: We are sorry Rayan ﻿Slim. We cannot process yo﻿ur application.﻿
```

**Example Output 3**

```java
>>﻿: Name: Rayan Slim
>>﻿: Nationality: Canadian
>>﻿: Date of Birth: 01﻿/﻿01﻿/﻿1111
﻿>>﻿: Seat Number: 4

>>﻿: Congratulations Ray﻿an Slim. Your passport was﻿ approved!
```

Keep testing the function. It should keep updating the person's `seatNumber` in the range `1 - 11`.

## Visualizing the Runtime

After you solve this workbook, I still recommend watching the video solution on Udemy.

![5.png](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F2eac1be6-ae3a-47be-a396-303eab8b8200?alt=media&token=3c1a552e-a448-489e-8bb6-8f947d64ae45)

It will show you how to visualize the runtime using Visual Studio Code.

----------

##### Subscribe to our [YouTube Channel](https://www.youtube.com/@RayanSlim087?sub_confirmation=1) and Discover More Valuable Content!