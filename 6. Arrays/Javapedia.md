# Javapedia

In this section's final project, you're the editor for Javapedia.

&nbsp;

![](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F4b1de0c5-7d04-4b16-ac48-3222cfff5350?alt=media&token=63863247-ae4a-4fe8-9112-97cd2d63b143)


Javapedia is a free encyclopedia that anyone can edit. As a world-renowned editor, your task is to submit information about famous historical figures.

![](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F1fc9d377-883c-4e5c-a99d-e853ab76b8e2?alt=media&token=128929e6-6ac2-4061-a6ad-90fb37f9e3cb)

Then, Javapedia will print the content from its "database" (in our case, a 2D array)

![](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F0e97e0bd-0f30-4d83-aff8-cd423bdbba69?alt=media&token=226e096b-2cbc-4453-9c04-abaa453f3d9d)

Javapedia also lets the user search popular figures by name:

```
**﻿**﻿**﻿**﻿**Javapedia**﻿**﻿**﻿**﻿**
How many historical figures will you register?
2

        Figure: 1
         - Name: Marco Polo
         - Date of birth: 08﻿/﻿01﻿/﻿1324
         - Occupation: Merchant

        Figure: 2
         - Name: Shakespeare
         - Date of birth: 26﻿/﻿03﻿/﻿1564
         - Occupation: Playwright

These are the values you stored:
        Marco Polo 08﻿/﻿01﻿/﻿1324 Merchant
        Shakespeare 26﻿/﻿03﻿/﻿1564 Playwright

Wh﻿o ﻿do﻿ y﻿ou want infor﻿ma﻿ti﻿on﻿ on? Marco Polo

        Name: Marco Polo
        Date of birth: 08/01/1324
        Occupation: Merchant
```

Launch the workbook
-------------------

First, launch the workbook from Visual Studio Code.

![](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2Fdb7a838d-1115-4e12-be18-c544b1a123f7?alt=media&token=2b117380-707e-43b2-a57c-bfc3bc7f83fb)

From `Java Bootcamp Resources` -> `Module 2` -> `6. Array`, open Javapedia.

Task 1
------

Ask the user: `How many historical figures will you register?`. Store the value in an `int` variable.

![](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F3525fda0-27af-4aa1-a85f-2520815448bf?alt=media&token=ff70843d-511b-4f3a-bcb8-1323cc9049e9)

Task 2
------

Make a 2D array named: `database`. The data we're going to submit will take the form of a table.

![](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F5bf7e43b-7769-4db4-9daa-5b31ce5fd4ab?alt=media&token=23d33bde-b8ad-4ec2-b7f3-c6fed9a8a422)

So, our array must have as many rows as there are historical figures. Each row also needs 3 values.

**Don't populate the array yet. Leave that for task 3.**

Task 3
------

Create a `for` loop that runs through every row in the database. The user needs to submit three values per row.

![](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F1aae31d9-3ad6-43f3-a580-a868ea12103d?alt=media&token=5adadfec-6e52-4282-adc7-4dabc248d5ec)

As the user submits each value, you need to store it in the appropriate row. While doing this task, be careful of the `nextLine` pitfall (see cheat sheet).

Task 4
------

Print the contents of `database`. Create a function called `print2DArray`.

```java
/**
 * Function name: print2DArray
 * @param array (String[][])
 *
 * Inside the function
 *  1. print the database
 *   - a tab of space precedes each row.
 *   - each value in database has one space from the other value.
 */
```

**Inside the function:**

-   add a tab of space before each row.

-   add a space after printing each value.

![](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F4c7ed36a-613b-4fc0-a5c0-8c694c6c0b7f?alt=media&token=52a03554-df98-48d4-812a-207a59fe5284)

Once you finish writing the function, use it to print `database`:

![](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F6a1efdc4-29d8-4c3b-ba5b-aeff5104766a?alt=media&token=9974b5c1-5011-40b1-964e-41b3aa7a5c90)

Task 5
------

The final task is to let the user search the database by name. If the search matches a name in `database`, print that row's information.

**Final Output:**

```
**﻿**﻿**﻿**﻿**Javapedia**﻿**﻿**﻿**﻿**
How many historical figures will you register?﻿2

        Figure: 1
         - Name: Marco Polo
         - Date of birth: 08﻿/﻿01﻿/﻿1324
         - Occupation: Merchant

        Figure: 2
         - Name: Shakespeare
         - Date of birth: 26﻿/﻿03﻿/﻿1564
         - Occupation: Playwright

These are the values you stored:
        Marco Polo 08﻿/﻿01﻿/﻿1324 Merchant
        Shakespeare 26﻿/﻿03﻿/﻿1564 Playwright

Wh﻿o ﻿do﻿ y﻿ou want infor﻿ma﻿ti﻿on﻿ on? Marco Polo

        Name: Marco Polo
       ﻿ Date of birth: 08/01/1324
        Occupation: Merchant
```

When printing the information, add a tab of space before each line.

Good luck!
----------
##### Subscribe to our [YouTube Channel](https://www.youtube.com/@RayanSlim087?sub_confirmation=1) and Discover More Valuable Content!