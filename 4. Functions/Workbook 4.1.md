# Workbook 4.1

From the `Java Bootcamp Resources`, launch the **`Workbook 4.1`** folder.

![4.1.png](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2Ffd25dd4b-b35e-494b-8047-538810d195f7?alt=media&token=7958b1a6-d720-43a2-8ca8-751f0dfab896)

## Bart's detention.
-----------------

Bart's teacher wants him to write lines on the chalkboard.

![](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F424fd671-c678-4500-8fb7-a433e299ce8b?alt=media&token=a5cef804-8af3-4511-80d7-6185e6885d9c)

He needs to write this paragraph 6 times:

`I will not copy and paste code.`

`I will use Camel Case when writing class names.` 

`I will use lower Camel Case when writing function names.`

`I will use lower Camel Case when writing variables names.`

Bart wrote the paragraph once, but it took him a long time!

```
public class Detention {

     public static void main﻿(﻿String[] args﻿) {
         //what Bart did so far
         System.out.﻿println﻿(﻿"I will not copy and paste code."﻿)﻿;
         System.out.﻿println﻿(﻿"I will use Camel Case when writing class names."﻿)﻿;
         System.out.﻿println﻿(﻿"I will use lower Camel Case when writing function names."﻿)﻿;
         System.out.﻿println﻿(﻿"I will use lower Camel Case when writing variables names."﻿)﻿;
    }

}
```

`>> I will not copy and paste code.`

`>> I will use Camel Case when writing class names. `

`>> I will use lower Camel Case when writing function names. `

`>> I will use lower Camel Case when writing variables names.`

## Task 1 - Write a function
-------------------------

Help Bart write a function that does the task for him. The doc comment will guide you.

```
    /**
      * Function name: printLines
      *
      * Inside the function:
      *   1. prints the four lines
      */
```

A doc comment is embedded inside `/** ... */`. They're best at describing the function name, parameters, and return value.

- The name of the function is `printLines`.

```
    /**
      * Function name: printLines  <--
      *
      * Inside the function:
      *   1. prints the four lines
      */
```

- The comment says nothing about parameters, so you can assume it doesn't take any.

- The comment says nothing about a return value. So, you can assume the function is `void`.

- Inside the function, it prints the four lines.

```
    /**
      * Function name: printLines
      *
      * Inside the function:
      *   1. prints the four lines    <--
      */
```

The doc comment outlines everything you need to make your function.

## Task 2 - Call the function
--------------------------

Once you finish writing it, call the function six times from `main()`.

## Run your code.
--------------


```
   >>I will not copy and paste code.
   >>I will use Camel Case when writing class names.
   >>I will use lower Camel Case when writing function names.
   >>I will use lower Camel Case when writing variables names.

   >>I will not copy and paste code.
   >>I will use Camel Case when writing class names. 
   >>I will use lower Camel Case when writing function names.
   >>I will use lower Camel Case when writing variables names.
   
   >>I will not copy and paste code.
   >>I will use Camel Case when writing class names.
   >>I will use lower Camel Case when writing function names.
   >>I will use lower Camel Case when writing variables names.

   ...
```
## Visualizing the Runtime

After you solve this workbook, I still recommend watching the video solution on Udemy.

![4.1.png](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F90894acf-190f-4e46-bd25-d0fa6b075b5d?alt=media&token=d5b69c48-f1f6-404e-a05f-8f4fbb3f98c7)

It will show you how to visualize the runtime using Visual Studio Code.

----------
##### Subscribe to our [YouTube Channel](https://www.youtube.com/@RayanSlim087?sub_confirmation=1) and Discover More Valuable Content!