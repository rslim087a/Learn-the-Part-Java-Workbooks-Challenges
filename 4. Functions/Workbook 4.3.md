# Workbook 4.3

From the `Java Bootcamp Resources`, launch the **`Workbook 4.3`** folder.

![4.3.png](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F45585afb-2d3c-4372-a1ba-174db6fcfc01?alt=media&token=c91a5eda-829d-4bbf-950a-92bcf75db7f4)

## Weather
-------
These are the temperatures for noon, evening, and midnight in Fahrenheit. We need to convert them to Celsius.

```java
public static void main﻿(﻿String[] args﻿) {

   double noon = 77﻿;          //temperature in fahrenheit.
   double evening = 61﻿;       //temperature in fahrenheit
   double midnight = 55﻿;      //temperature in fahrenheit

}
```

## Task 1 - Write a function

You will write a function that converts Fahrenheit to Celcius.

- Function name.

```java
/**
 * Function name: fahrenheitToCelsius. <-----
 * @param fahrenheit (double)
 * @return celsius (double)
 *
 * Inside the function:
 *  1. return the celsius temperature.    C = (F - 32) * 5/9
 */
```

- Parameter.

```java
/**
 * Function name: fahrenheitToCelsius.
 * @param   fahrenheit (double)  <------
 * @return  celsius   (double)
 *
 * Inside the function:
 *  1. return the celsius temperature.   C = (F - 32) * 5/9
 */
```

- Return value.

```java
/**
 * Function name: fahrenheitToCelsius.
 * @param   fahrenheit (double)
 * @return  celsius   (double) <------
 *
 * Inside the function:
 *  1. return the celsius temperature.   C = (F - 32) * 5/9
 */
```

Inside the function, use the equation to go from Fahrenheit to Celsius. Then, return the result.

```java
/**
 * Function name: fahrenheitToCelsius.
 * @param   fahrenheit (double)
 * @return  celsius   (double)
 *
 * Inside the function:
 *  1. return the celsius temperature.   C = (F - 32) * 5/9  <----
 */
```

## Task 2 - Write another function

-  Function name.

```java
/**
 * Name: printTemperatures  <-----
 * @param fahrenheit (double) 
 *
 * Inside the function:
 *  1. prints the fahrenheit value: "F: <temp in fahrenheit>".
 *  2. calls fahrenheitToCelsius, and
 *     prints the celcius value: "C: <temp in celsius> \n".
 */
```

- Parameter.

```java
/**
 * Name: printTemperatures
 * @param fahrenheit (double) <-----
 *
 * Inside the function:
 *  1. prints the fahrenheit value: "F: <temp in fahrenheit>".
 *  2. calls fahrenheitToCelsius, and
 *     prints the celcius value: "C: <temp in celsius> \n"..
 */
```

- Return value: The function is `void`.

- Code the logic inside the function

```java
/**
 * Name: printTemperatures
 * @param fahrenheit (double)
 *
 * Inside the function:  <-----
 *  1. prints the fahrenheit value: "F: <temp in fahrenheit>".
 *  2. calls fahrenheitToCelsius, and prints the celcius value: "C: <temp in celsius> \n"..
 */
```

## Task 3 - Call the function

From `main()`, call the `printTemperatures` function for each value.

## Run your code

![](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F668e8d4e-bcac-40ee-a9ae-7eb3ccb11992?alt=media&token=962bad7b-7a68-4710-95d4-a2391181c922)

## Visualizing the Runtime

After you solve this workbook, I still recommend watching the video solution on Udemy.

![4.3.png](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F253e59f7-93fb-4c41-a1fd-d1ccdd8ef104?alt=media&token=ca70e078-f2de-45fc-92a0-fcfff7da990b)

It will show you how to visualize the runtime using Visual Studio Code.

----------
##### Subscribe to our [YouTube Channel](https://www.youtube.com/@RayanSlim087?sub_confirmation=1) and Discover More Valuable Content!