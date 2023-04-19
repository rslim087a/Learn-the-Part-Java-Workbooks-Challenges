# Workbook 3.5

From the `Java Bootcamp Resources`, launch the **`Workbook 3.5`** folder.

![Screen Shot 2022-10-16 at 6.44.39 PM.png](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2Fdd27cafe-ec54-44bd-93b6-111b96de713e?alt=media&token=ae82e428-1c88-4cc5-b7b1-0251b65bbfd6)



## Your Work Schedule
------------------

Assume that `day` can be any value between 1 (Monday) and 7 (Sunday). There's also a `boolean` variable: `holiday`.

```java
public class WorkSchedule {

     public static void main﻿(﻿String[] args﻿) {
           int day = 3;
           boolean holiday = true;                ﻿ ﻿
     }
}

```

## Task 1 - Do I have work that day?
---------------------------------

In the event of a holiday, `print`:

> Woohoo, no work

During the weekend (Saturday or Sunday), `print`:

> It's the weekend, no work!

Otherwise, `print`:

> Wake up at 7:00 :(

## Run your code.
--------------

### Test Case 1:
```java
    int day = 3;
    boolean holiday = true;                ﻿ ﻿
```

`>>woohoo, no work!`

### Test Case 2:

```java
    int day = 3;
    boolean holiday = false;                ﻿ ﻿
```

`>>Wake up at 7:00 :(`

### Test Case 3:

```java
    int day = 6;
    boolean holiday = false;                ﻿ ﻿
```
`>>It's the weekend, no work!`

## Visualizing the Runtime

After you solve this workbook, I still recommend watching the video solution on Udemy.

![Screen Shot 2022-10-17 at 2.59.56 PM.png](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2Fc712b067-a1f0-4262-a588-11a0e619048d?alt=media&token=a79884ca-69f0-42ad-b821-cfcfe5391d26)

It will show you how to visualize the runtime using Visual Studio Code.

----------
##### Subscribe to our [YouTube Channel](https://www.youtube.com/@RayanSlim087?sub_confirmation=1) and Discover More Valuable Content!