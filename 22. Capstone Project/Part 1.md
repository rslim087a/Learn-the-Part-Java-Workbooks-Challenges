# Capstone Project

Congratulations on reaching the Capstone Project. This project will test the skills that you learned in Module 2.  As such, a video solution will not be provided, but you will still have access to a final solution inside your Bootcamp Resources.

## Download the starter project
-----------------------------------

Launch the `starter-code` folder inside `Java Bootcamp Resources` -> `Module 2` -> `Casptone Project`.


## Task 1

Inside `TradeAccount.java`, create an abstract `TradeAccount` class. The `abstract` class will define the following field:

```java
    private String id;
```

## Task 2

Create getter and setter methods for the `id` field in the `TradeAccount` class. Do not worry about argument validation.

## Task 3

Create a constructor that initializes the `id` field of a newly created `TradeAccount` object.

## Task 4

Add an abstract method called `clone` to the `TradeAccount` class. The `clone` method will have no parameters and return a `TradeAccount` object.

## Task 5

Make sure that `CashAccount` extends the `TradeAccount` class. The `CashAccount` class will define the following field:

```java
    private BigDecimal cashBalance;
```

## Task 6

Create getter and setter methods for the `cashBalance` field in the `CashAccount` class. Do not worry about argument validation.
 
## Task 7

Create a constructor that initializes the fields of a newly created `CashAccount` object by calling the superclass constructor and updating the `cashBalance` field.

## Task 8

Override the clone method in the `CashAccount` class. The method should return a new `CashAccount` object with the same `id` and `cashBalance`.

## Task 9

Make sure that `MarginAccount` extends the `TradeAccount` class. The `MarginAccount` class will define the following field:

```java
    private BigDecimal margin;
```

## Task 10

Create getter and setter methods for the `margin` field in the `MarginAccount` class. Do not worry about argument validation.

## Task 11

Create a constructor that initializes the fields of a newly created `MarginAccount` object by calling the superclass constructor and updating the `margin` field.

## Task 12
Override the clone method in the `MarginAccount` class. The method should return a new `MarginAccount` object with the same `id` and `margin`.

## Task 13
Test your implementation by creating instances of the `CashAccount` and `MarginAccount` classes and calling their clone methods.

```java
    public static void main(String[] args) {
        CashAccount cashAccount = new CashAccount("C123", new BigDecimal("1000.00"));
        System.out.println("Cash Account Details:");
        System.out.println("ID: " + cashAccount.getId());
        System.out.println("Cash Balance: " + cashAccount.getCashBalance());

        CashAccount clonedCashAccount = (CashAccount) cashAccount.clone();
        System.out.println("Cloned Cash Account Details:");
        System.out.println("ID: " + clonedCashAccount.getId());
        System.out.println("Cash Balance: " + clonedCashAccount.getCashBalance());

        System.out.println();

        MarginAccount marginAccount = new MarginAccount("M456", new BigDecimal("5000.00"));
        System.out.println("Margin Account Details:");
        System.out.println("ID: " + marginAccount.getId());
        System.out.println("Margin: " + marginAccount.getMargin());

        MarginAccount clonedMarginAccount = (MarginAccount) marginAccount.clone();
        System.out.println("Cloned Margin Account Details:");
        System.out.println("ID: " + clonedMarginAccount.getId());
        System.out.println("Margin: " + clonedMarginAccount.getMargin());
    }
```

Compile and run the `Main` class to test your implementation. The output should display the details of the cash account and margin account instances, as well as the cloned instances.

----------

##### Subscribe to our [YouTube Channel](https://www.youtube.com/@RayanSlim087?sub_confirmation=1) and Discover More Valuable Content!