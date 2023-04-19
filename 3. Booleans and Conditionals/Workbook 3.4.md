# Workbook 3.4

From the `Java-Bootcamp-Resources`, launch the **`Workbook 3.4`** folder.

![Screen Shot 2022-10-16 at 6.04.12 PM.png](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F03335aa5-a392-430b-9399-f030b8646e8b?alt=media&token=cbc9bc6e-bab5-4cdd-b6c0-7761dc8764c1)

## The Weather Network
-------------------

The workbook starts with a temperature (Celsius). There's also a `String` variable `forecast` that doesn't start with a value.

```java
public class WeatherNetwork {

     public static void main﻿(﻿String[] args﻿) {
        int temp = 25﻿;
        String forecast;

        System.out.println(forecast);
    }
}
```

## Task 1 - Update the forecast.
-----------------------------

Update the `forecast` variable based on the temperature.

-   Less than or equal to **-1**

> The forecast is FREEZING! Stay home!

-   Less than or equal to **10** 

> The forecast is Chilly. Wear a coat!

-   Otherwise

> It's warm. Go outside!

## Run your code.

### Test Case 1:
```java
    int temp = 25﻿;
```
`>>: It's warm. Go outside!`

### Test Case 2:
```java
    int temp = -1;
```
`>>: The forecast is FREEZING! Stay home!`

### Test Case 3:
```java
    int temp = 0;
```
`>>: The forecast is Chilly. Wear a coat!`

### Test Case 4:
```java
    int temp = 10;
```
`>>: The forecast is Chilly. Wear a coat!`


### Test Case 5:
```java
    int temp = 11;
```
`>>: It's warm. Go outside!`


### Test Case 6:
```java
    int temp = -12;
```
`>>: The forecast is FREEZING! Stay home!`

## Visualizing the Runtime

After you solve this workbook, I still recommend watching the video solution on Udemy.

![Screen Shot 2022-10-17 at 2.59.42 PM.png](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2Ff102b494-aa2f-4c62-a8d6-12899bb64768?alt=media&token=da6b1365-05c5-453d-922f-769722922160)

It will show you how to visualize the runtime using Visual Studio Code.

----------
##### Subscribe to our [YouTube Channel](https://www.youtube.com/@RayanSlim087?sub_confirmation=1) and Discover More Valuable Content!