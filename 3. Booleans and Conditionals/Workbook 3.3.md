# Workbook 3.3

From the `Java-Bootcamp-Resources`, launch the **`Workbook 3.3`** folder.

![Screen Shot 2022-10-16 at 5.44.01 PM.png](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F689e02cb-9105-4592-8fbe-2e9291b0fc17?alt=media&token=9564167d-a8f2-48ad-ba0b-62ec432ff31c)

## The Quidditch Championship

This is a modified passage from the book: **Harry Potter and the Half-Blood Prince.**

![Screen Shot 2022-10-16 at 8.27.45 PM.png](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F6e92fe9c-93a3-4c3b-9bd8-3eeb3778ed31?alt=media&token=4e98e8b8-508a-4871-bb65-f6b50965b936)

We're going to convert this passage into code. The code starts with the number of points scored by `gryffindor` and `ravenclaw`.

```java
public class Championship {

   public static void main﻿(﻿String[] args﻿) {

        int gryffindor = 400;    //gryffindor points       ﻿ ﻿
        int ﻿ravenclaw = 200;    //ravenclaw p﻿oints﻿
   }

```

## 1\. Calculate the difference in points.
---------------------------------------

Make an `int` variable called `margin`. It will calculate the margin of points `gryffindor` scored over `ravenclaw`.

```java
public class Championship {

   public static void main﻿(﻿String[] args﻿) {

        int gryffindor = 400﻿;    //gryffindor points
        int ravenclaw = 200﻿;    //ravenclaw points

     // margin: amount of points by which gryffindor scored﻿ ﻿over ravencla﻿w ;
   }

}﻿
```

## 2\. if - else if - else.
------------------------------

If `gryffindor` wins by a margin of 300 points or more, `print`:

> Gryffindor takes the house cup!

If `gryffindor` wins by a margin of any points or ties, `print`:

> In second place, Gryffindor!

If `gryffindor` loses within 100 points, `print`:

> In third place, Gryffindor!

`else`, `print`:

> In fourth place, Gryffindor!


## Run your Code
### Test Case 1
```java
        int gryffindor = 400﻿;            
        int ravenclaw = 200﻿;
```
`>>In second place, Gryffindor!`

### Test Case 2:

```java
         int gryffindor = 850﻿;
         int ravenclaw = 500﻿;
```

`>>Gryffindor takes the house cup!`

### Test Case 3:

```java
         int gryffindor = 620﻿;
         int ravenclaw = 500﻿;
```

`>>In second place, Gryffindor!`

### Test Case 4:


```java
         int gryffindor = 450﻿;
         int ravenclaw = 500﻿;
```

`>>In third place, Gryffindor!`

### Test Case 5:

```java
        int gryffindor = 100﻿;
        int ravenclaw = 500﻿;
```

`>>In fourth place, Gryffindor!`

## Visualizing the Runtime

After you solve this workbook, I still recommend watching the video solution on Udemy.

![Screen Shot 2022-10-16 at 5.57.44 PM.png](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2Fad50b3a3-2c63-478b-83fe-d65b003091c4?alt=media&token=a73ffbe6-ad7e-4071-9ec6-4db160826a11)

It will show you how to visualize the runtime using Visual Studio Code.

## Solution Code

The solution code is inside the same folder as the starter project.

![Screen Shot 2022-10-16 at 5.57.24 PM.png](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F81dede16-4518-4cff-878a-49f9e41ae52b?alt=media&token=fff8a58c-532f-4aab-9db7-65003d444f56)

## Good Luck!
-------
##### Subscribe to our [YouTube Channel](https://www.youtube.com/@RayanSlim087?sub_confirmation=1) and Discover More Valuable Content!