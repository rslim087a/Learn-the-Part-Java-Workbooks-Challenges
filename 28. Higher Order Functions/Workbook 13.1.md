# Workbook 13.1

From the `Java Bootcamp Resources`, launch **starter**.

![starter.png](https://img-c.udemycdn.com/redactor/raw/article_lecture/2025-01-03_18-42-48-e972bb666fc3b9aa8e54201ab9e23930.png)

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

##### **Go From Zero to DevOps Master**: *[Java → Spring Boot → Docker → Kubernetes](https://rslim087a.github.io/zero-devops-roadmap/)*