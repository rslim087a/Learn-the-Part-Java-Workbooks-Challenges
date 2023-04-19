# Workbook 4.5

From the `Java Bootcamp Resources`, launch the **`Workbook 4.5`** folder.

![4.5.png](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F621568d2-4f4c-411d-bc0f-2ba2f4ab8efd?alt=media&token=04511110-9b6f-418b-95b0-a947c764b8bc)

Area Calculator
---------------

In this workbook, you will calculate the area of a square, rectangle, triangle, and circle.

## **Task 1: area of a square**
-----------------------------

- Function name:

```java
/**
 * Name: areaSquare  <------
 * @param side (double)
 * @return the area (double)
 *
 * Inside the function:
 *  1. If side is negative
 *        - prints "Impossible"
 *        - shuts the app down
 *  2. Calculates the area of the square. A = side²
 */
```

- Parameters:

```java
/**
 * Name: areaSquare
 * @param side (double)  <--------
 * @return the area (double)
 *
 * Inside the function:
 *  1. If side is negative
 *        - prints "Impossible"
 *        - shuts the app down
 *  2. Calculates the area of the square. A = side²
 */
```

- Return value:

```java
/**
 * Name: areaSquare
 * @param side (double)
 * @return the area (double) <--------
 *
 * Inside the function:
 *  1. If side is negative
 *        - prints "Impossible"
 *        - shuts the app down
 *  2. Calculates the area of the square. A = side²
 */
```

- Inside the function:
```java
/**
 * Name: areaSquare - returns the area of a square.
 * @param side (double)
 * @return the area (double)
 *
 * Inside the function: <---------
 *  1. If side is negative
 *        - prints "Impossible"
 *        - shuts the app down
 *  2. Calculates the area of the square. A = side²
 */
```

$Area = side²$ 

![68747470733a2f2f666972656261736573746f726167652e676f6f676c65617069732e636f6d2f76302f622f6c6561726e746865706172742d37356165642e61707073706f742e636f6d2f6f2f696d6167657325324662313461363061642d623136302d346637612d396430302d63656637636237656264.png](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2Fd29f2bd4-dcf2-4ec6-863b-bb7db61fa400?alt=media&token=fe1e3d74-164b-4a89-a92d-d99703acc489)

Use a `Math` function to calculate side to the power of 2.

## **Task 2: area of a rectangle**
--------------------------------

Write a function that calculates the area of a rectangle.

$Area = length * width$
![](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F5ad64d99-e194-47f0-9926-c77b0d2c28c8?alt=media&token=f2c25850-02ce-4143-8ca8-26703861c5a4)


1\. Function name.

```java
/**
 * Name: areaRectangle    <------
 * @param length (double).
 * @param width  (double).
 * @return the area (double)
 *
 * Inside the function:
 *  1. If the length OR width is negative
 *       - print "Error: impossible" and
 *       - terminate the program.
 *  2. return the area: length * width
 */
```

2\. Parameters.

```java
/**
 * Name: areaRectangle
 * @param length (double).  <-----
 * @param width  (double).  <-----
 * @return the area (double)
 *
 * Inside the function:
 *  1. If the length OR width is negative
 *       - print "Error: impossible" and
 *       - terminate the program.
 *  2. return the area: length * width
 */
```

**3**. Return value.

```java
/**
 * Name: areaRectangle
 * @param length (double).
 * @param width  (double).
 * @return the area (double)   <------
 *
 * Inside the function:
 *  1. If the length OR width is negative
 *       - print "Error: impossible" and
 *       - terminate the program.
 *  2. return the area: length * width
 */
```

Inside the function:

1.  Check if the length OR width is negative. If so, print "Error: impossible" and terminate the java program.

2.  Then, calculate the area of the rectangle and return it.

```java
/**
 * Name: areaRectangle
 * @param length (double).
 * @param width  (double).
 * @return the area (double)
 *
 * Inside the function:  <-----
 *  1. If the length OR width is negative
 *       - print "Error: impossible" and
 *       - terminate the program.
 *  2. return the area: length * width
 */
```

## **Task 3: area of a triangle**
-------------------------------



![](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F5162690e-6a1d-4105-a7ff-5bc8aa5d7e85?alt=media&token=7e254402-2497-4200-80e6-599c4e9d4459) $Area  = base * height \div 2$

```java
/**
 * Name: areaTriangle
 * @param base: (double).
 * @param height: (double).
 * @return the area (double)
 *
 * Inside the function:
 *  1. If the base OR height is negative
 *      - print "Error: impossible"
 *      - terminate the program.
 *  2. return the area: base * height / 2
 */
```

## **Task 4: area of a circle**
-----------------------------


![](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2Febebafe5-8cb8-4f18-b060-0f5576fe8091?alt=media&token=a29585de-8fa1-4931-aa32-ac09df74ce27) $Area = π * radius²$

How do you get PI? You could set a `double` equal to 3.14159... but, please don't do that. You can get PI from the `Math` class. I encourage you to look it up.

Then, write a function that calculates the area of a circle.

```java
/**
 * Name: areaCircle
 * @param radius (double).
 * @return area (double)
 *
 * Inside the function:
 *  1. If the radius is negative
 *      - print: Impossible
 *      - terminates the program
 *  2. returns the area: π * radius2
 */
```

## **Task 5: Calculate the areas**
--------------------------------

Using the appropriate function, calculate the area for:

-   a square with a side of 2 cm.

-   a rectangle with a length of 1 cm, and a width of 2 cm.

-   a triangle with a base of 1 cm, and a height of 2 cm.

-   a circle with a radius of 2 cm.

```java
// double square = area of square with a side of 2.
// double rectangle = area of rectangle with length: 1, width: 2.
// double triangle = area of triangle with base: 1, height: 2.
// double circle = area of circle with a radius of 2.
```

## **Task 6: Write a function that prints every area**
---------------------------------------------------

Instead of cluttering `main()`with 4 `println` statements, write a function that prints every area.

```java
/**
 * Name: printAreas -- it prints four areas
 * @param square (double)
 * @param rectangle (double)
 * @param triangle (double)
 * @param circle (double)
 *
 * Inside the function:
 *  1. print: ("Square area: <square area>")
 *  2. print: ("Rectangle area: <rectangle area>")
 *  3. print: ("Triangle area: <triangle area>")
 *  4. print: ("Circle area: <circle area>")
 *
 */
```

## **Task 7: Call the** `printAreas` **function.**
---------------------------------------------------

From `main()`, call the printAreas function.

## Run your code
-------------

```
Thank you for using the area calculator
This calculator lets you get the area of﻿:

1 -- Square
2 -- Rectangle
3 -- Triangle
4 -- Circle

Square area: 4.0
Rectangle area: 2.0
Triangle area: 1.0
Circle area: 12.56637061﻿44
```
## Visualizing the Runtime

After you solve this workbook, I still recommend watching the video solution on Udemy.

![4.5.png](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F129f2e19-f52f-4f12-be0f-0042c9dc1f90?alt=media&token=671cd4ab-b9e3-4d4e-be95-91b2e32a85a8)

It will show you how to visualize the runtime using Visual Studio Code.

----------
##### Subscribe to our [YouTube Channel](https://www.youtube.com/@RayanSlim087?sub_confirmation=1) and Discover More Valuable Content!
