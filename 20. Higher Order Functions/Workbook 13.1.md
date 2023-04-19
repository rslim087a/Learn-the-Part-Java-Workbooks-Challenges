# Workbook 13.1

From the `Java Bootcamp Resources`, launch **starter**.

![starter.png](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F87bced44-2cd9-4db0-9a76-22125c478254?alt=media&token=7dc717de-b9d3-40c6-9ec2-32908aa28976)

## Task 1

Use `forEach` to iterate the `ArrayList` and print the following messages.
```java
        System.out.println("Date: " + p.getDate().format(DateTimeFormatter.ofPattern("dd/MM/yyyy")));
        System.out.println("Amount: " + p.getAmount());
        System.out.println("---");
```
 Consider that `forEach` relies on a `Consumer` to perform its task.


| Functional Interface | Example |
| ----- | -------------------- |
| Consumer | `x -> { code } `|
| Predicate | `x  ->  { return boolean }`|
| Function | `x  ->  { return value }`|
| BiConsumer | `(x, y) -> { code }`|
| Comparator | `(x, y) -> { return int }`|
| BinaryOperator | `(x, y) -> { return value (same type) }`|


### **Expected Output**
```
Date: 01/01/2020
Amount: 100.0
---
Date: 15/02/2020
Amount: 200.0
---
Date: 30/03/2020
Amount: 300.0
---
Date: 01/04/2020
Amount: 50.0
---
Date: 15/05/2020
Amount: 75.0
---
Date: 30/06/2020
Amount: 100.0
---
```

----------

##### Subscribe to our [YouTube Channel](https://www.youtube.com/@RayanSlim087?sub_confirmation=1) and Discover More Valuable Content!