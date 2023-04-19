# Bank Management - Part 2
---
**Goal**: create the parent class.

## Task 1
------
Create an `Account` class inside the `account` folder. The `Account class` will serve as the parent for `Chequing`, `Savings`, and `Loan`.

## Task 2
------
Every child class will inherit three fields: `id`, `name`, and `balance`.

## Task 3
------
Add a constructor to the parent class.

## Task 4
------
Add a copy constructor to the parent class.

## Task 5
------
Add getters/setters to the parent class.

## Task 6
------
Add a constructor and copy constructor to every child class.

## Task 7
------

Test your code by creating three `Account` objects:


```java
Chequing chequing = new Chequing("f84c43f4-a634-4c57-a644-7602f8840870", "Michael Scott", 1524.51);
Savings savings = new Savings("ce07d7b3-9038-43db-83ae-77fd9c0450c9", "Saul Goodman", 2241.60);
Loan loan = new Loan("4991bf71-ae8f-4df9-81c1-9c79cff280a5", "Phoebe Buffay", 2537.31);
```
Add three breakpoints and visualize the runtime. Confirm that each object is using its parent's constructor to update its fields.

Task 8
------
`Override` `toString` for the `Account` class. Use the following format:
```java
    @Override
    public String toString() {
        return (className of current object) + "    " +
            "\t" + id + "" +
            "\t" + name + "" +
            "\t$" + balance + "";
    }
```
Task 9
------
Print each object:


```
>>: Chequing        f84c43f4-a634-4c57-a644-7602f8840870    Michael Scott   $1524.51
>>: Savings         ce07d7b3-9038-43db-83ae-77fd9c0450c9    Saul Goodman    $2241.6
>>: Loan            4991bf71-ae8f-4df9-81c1-9c79cff280a5    Phoebe Buffay   $2537.31

```
Task 10
------
Data isn't always perfect. Apply "quality control" inside the constructor and setters.

## Good Luck!
--------
##### Subscribe to our [YouTube Channel](https://www.youtube.com/@RayanSlim087?sub_confirmation=1) and Discover More Valuable Content!