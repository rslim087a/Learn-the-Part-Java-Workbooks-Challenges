# Global Superstore 3

**Prerequisite:** You wrote the solution for Part 2.


## Task 1
-----
Remove this line of code:

     System.out.println("Access Denied. We apologize for the inconvenience. Have a good day " + name + ".");

After the user enters their information, the `main` thread must wait for the worker threads to die. Then, you can present the user with sales data:
```java
    System.out.println("\nThank you " + <name> + ". The average sales for Global Superstore are:\n");
    System.out.println("Average Furniture Sales: " + <furniture sales>);
    System.out.println("Average Technology Sales: " + <tech sales>);
    System.out.println("Average Office Supplies Sales: " + <office sales>);
    System.out.println("Total Average: " + <total>);
```

Your output should appear as follows:


```
>>: Please enter your name to access the Global Superstore dataset: Rayan

>>: Thank you Rayan. The average sales for Global Superstore are:

>>: Average Furniture Sales: 9799.21280813723
>>: Average Technology Sales: 9854.096986549781
>>: Average Office Supplies Sales: 9540.319577001303
>>: Total Average: 9651.778039610392
```
## Good Luck!
--------
##### Subscribe to our [YouTube Channel](https://www.youtube.com/@RayanSlim087?sub_confirmation=1) and Discover More Valuable Content!