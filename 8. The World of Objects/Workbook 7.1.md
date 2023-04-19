# Workbook 7.1

Inside the `Java Bootcamp Resources`, launch **`Workbook 7.1`**.

![1.png](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2Ff32f7672-ee23-4a8d-ac9d-6b728ce93576?alt=media&token=cca21ed2-40c2-403f-a26a-69581239cc5e)

## **Task 1**

Create a new file named `Person.java`. Inside the file, create the `Person`  `class`.

```java
public class Person {


}
```

The `Person` `class` will define the following fields:

```
    String name;
    String nationality;
    String dateOfBirth;
    String[] passport;
    int seatNumber;
```

The `Person` class is a **blueprint** from which you can create `Person` objects.

## **Task 2**

Create one object of the `Person` class. Then print every field in the object.

```java
>>﻿: null
>>﻿: null
>>﻿: null
>>﻿: null
>>﻿: 0
```

## **Task 3**

Update each field in the object before printing them.

```java
        person.name = // a String
        person.nationality // a String
        person.dateOfBirth = // a String
        person.passport = // Array that stores: {person.name, person.nationality, person.dateOfBirth}
        person.seatNumber = // an Integer
```
### Hint for `passport`

You can only use shorthand initialization in the same line as the variable declaration.

![0.png](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F63a767b8-6b63-4c3e-905a-5ce626243c3f?alt=media&token=8801430f-bcbf-48a3-ad4a-db8683c4da39)

That's because the compiler is able to infer the array type.

![12.png](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F9237d2f9-bf6e-4d8c-bb09-1e3090ad3fca?alt=media&token=0a52f1c7-d445-497e-bf8e-9fa6d06dea69)

You cannot use shorthand initialization on another line because the compiler can't infer the type.

![13.png](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F846051bd-4687-4a87-ac55-391074a2ba36?alt=media&token=515d62b3-cee8-466f-b9ac-ef42c1c8f834)

You need to explicitly define a `new` array that can store `String` elements.

![14.png](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F4886a529-732d-4327-8f2b-6d6319508d09?alt=media&token=a7c6e50a-fe75-43a2-b063-1ca4732d8736)

## Task 4

Print the fields of your updated object.

```java
        System.out.println(person.name);
        System.out.println(person.nationality);
        System.out.println(person.dateOfBirth);
        System.out.println(Arrays.toString(person.passport));
        System.out.println(person.seatNumber);
```
### Result
```
>>﻿: Rayan Slim
>>﻿: Canadian
>>﻿: 01﻿/﻿01﻿/﻿1111
>>﻿: [Rayan Slim, Canadian, 01﻿/﻿01﻿/﻿1111﻿]
>>﻿: 5
```

## Visualizing the Runtime

After you solve this workbook, I still recommend watching the video solution on Udemy.

![1.png](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2Fa6868065-1769-496c-916e-ed2499d23530?alt=media&token=a7869820-17c2-46ff-b66f-a42fad1e5b12)

It will show you how to visualize the runtime using Visual Studio Code.

----------

##### Subscribe to our [YouTube Channel](https://www.youtube.com/@RayanSlim087?sub_confirmation=1) and Discover More Valuable Content!