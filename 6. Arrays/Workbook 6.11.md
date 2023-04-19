# Workbook 6.11

From the `Java Bootcamp Resources`, launch **`Workbook 6.11`**.

![6.11.png](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2Ff5d37803-f252-46bd-8853-29baa2c374c1?alt=media&token=4f31635e-fc0f-43b1-8e86-8aff053688f6)

## Task 1

Create a function called `celciusToFahrenheit`.  
```java
/**
 * Function name: celciusToFahrenheit.
 * 
 * 
 *
 * 
 *   
 */
```
The function will **receive** an array of values in `Celcius`.
```java
/**
 * Function name: celciusToFahrenheit.
 * @param celsius ( double[] )
 * 
 *
 * 
 *   
 */
```
The function will **return** an array of values in `Fahrenheit`.
```java
/**
 * Function name: celciusToFahrenheit.
 * @param celsius ( double[] )
 * @return fahrenheit ( double[] )
 * 
 * 
 *   
 */
```

1. The function creates a `double[]` array called `fahrenheit`.
```java
/**
 * Function name: celciusToFahrenheit.
 * @param celsius ( double[] )
 * @return fahrenheit ( double[] )
 *
 * Inside the function:
 *    1. Creates a double[] array called 'fahrenheit'.
 *    
 *    
 *     
 */
```
2. The function copies every value from the `celcius` parameter to the `fahrenheit` array.

```java
/**
 * Function name: celciusToFahrenheit.
 * @param celsius ( double[] )
 * @return fahrenheit ( double[] )
 *
 * Inside the function:
 *    1. Creates a double[] array called 'fahrenheit'.
 *    2. Copies all the values from celsius to fahrenheit.
 *    
 *     
 */
```
3. The function uses the formula below to convert every value in the fahrenheit array to Fahrenheit.

```java
/**
 * Function name: celciusToFahrenheit.
 * @param celsius ( double[] )
 * @return fahrenheit ( double[] )
 *
 * Inside the function:
 *    1. Creates a double[] array called 'fahrenheit'.
 *    2. Copies all the values from celsius to fahrenheit.
 *    3. Updates the fahrenheit values (F = (C/5 * 9) + 32).
 * 
 */
```
4. Finally, the function returns the result.
```java
/**
 * Function name: celciusToFahrenheit.
 * @param celsius ( double[] )
 * @return fahrenheit ( double[] )
 *
 * Inside the function:
 *     1. Creates a double[] array called 'fahrenheit'.
 *     2. Copies all the values from celsius to fahrenheit.
 *     3. Updates the fahrenheit values (F = (C/5 * 9) + 32).
 *     4. return fahrenheit.
 */
```


## Task 2

The starter code contains an array of Celsius values.

```java
double[﻿] celsius = {﻿12.5﻿, 14.5﻿, 17.0﻿, 21.0﻿, 23.0﻿, 18.5﻿, 20.0﻿}﻿;
```
Use your function to return an array of Fahrenheit values from the `celsius` array.

```java
double[﻿] fahrenheit = celciusToFahrenheit(celsius);
```

Print the contents of `fahrenheit` using `Arrays.toString`.

### Result

```
>>: [54.5, 58.099999999999994, 62.5999999999994, 69.800000000001, 73.4, 65.300000000001, 68.0]
```

## Task 3

Remove your print statement. Instead, create a function that receives a `double[]` array and a `String`.  

```java
/**
 * Function name - printTemperatures
 * @param temp ( double[] )
 * @param tempType ( String ) can be: Celsius or Fahrenheit
 *
 * 
 *
 *  
 *      
 *      
 *
 */
```
1. The function prints the temperature type using `print`, not `println`.

```java
/**
 * Function name - printTemperatures
 * @param temp ( double[] )
 * @param tempType ( String ) can be: Celsius or Fahrenheit
 *
 * Inside the function:
 *  1. System.out.print(tempType + ": ");
 *  
 *    
 *      
 * 
 */
```
2. The function uses a **`for`** loop to print the temperatures on the same line.

```java
/**
 * Function name - printTemperatures
 * @param temp ( double[] )
 * @param tempType ( String ) can be: Celsius or Fahrenheit
 *
 * Inside the function:
 *  1. System.out.print(type + ": ");
 *  2. A loop prints the temperatures in ONE line System.out.print(temp[i] + " ");
 *    
 *  
 */
```
3. The function prints a new line after the loop.

```java
/**
 * Function name - printTemperatures
 * @param temp ( double[] )
 * @param tempType ( String ) can be: Celsius or Fahrenheit
 *
 * Inside the function:
 *  1. System.out.print(type + ": ");
 *  2. A loop prints the temperatures in ONE line System.out.print(temp[i] + " ");
 *  3. Prints a new line after the loop System.out.print("\n");
 */
```
## Task 4

Call `printTemperatures` for each array.

```java
        double[] celsius = {12.5, 14.5, 17.0, 21.0, 23.0, 18.5, 20.0};
        double[] fahrenheit = celsiusToFahrenheit(celsius);

        printTemperatures(celsius, "Celsius");
        printTemperatures(fahrenheit, "Fahrenheit");
```

## Result

```java
>>: Celsius: 12.5 14.5 17.0 21.0 23.0 18.5 20.0
>>: Fahrenheit: 54.5 58.099999999999994 62.599999999999994 69.80000000000001 73.4 65.30000000000001 68.0
```
Don't mind the decimal points. You will learn rounding in **Module 2**.


## Visualizing the Runtime

After you solve this workbook, I still recommend watching the video solution on Udemy.

![11.png](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F7fbac23f-ab9b-4db0-acf1-fe902fc215fe?alt=media&token=40606162-ac20-4ae5-bec9-abff9ed1c676)

It will show you how to visualize the runtime using Visual Studio Code.

----------
##### Subscribe to our [YouTube Channel](https://www.youtube.com/@RayanSlim087?sub_confirmation=1) and Discover More Valuable Content!