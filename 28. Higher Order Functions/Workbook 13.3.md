# Workbook 13.3

From the `Java Bootcamp Resources`, launch **starter**.

![starter.png](https://img-c.udemycdn.com/redactor/raw/article_lecture/2025-01-03_18-32-26-a7b9b7c6eaa6a82be27ef1bf4fd98efd.png)

## Task 1

Use `forEach` to iterate the `HashMap` and print the following message.
```java
System.out.println(sku + "\t" + item.getPrice() + "\t" + item.getName())
```
 Consider that it will rely on a `BiConsumer` to perform its task.

| Functional Interface | Example |
| ----- | -------------------- |
| Consumer | `x -> { code } `|
| Predicate | `x  ->  { return boolean }`|
| Function | `x  ->  { return value }`|
| BiConsumer | `(x, y) -> { code }`|
| Comparator | `(x, y) -> { return int }`|
| BinaryOperator | `(x, y) -> { return value (same type) }`|

### Expected Output
```
SKU             Price   Item
DOFO-008        10.0    Super Doo-dad
THNG-003        2.99    Thingamajig
WIDG-005        6.99    Super Widget
GADG-006        8.99    Super Gadget
THNG-007        15.0    Super Thingamajig
WIDG-001        3.99    Widget
GADG-002        5.99    Gadget
DBOO-004        4.99    Doo-dad
```

----------

##### **Go From Zero to DevOps Master**: *[Java → Spring Boot → Docker → Kubernetes](https://rslim087a.github.io/zero-devops-roadmap/)*