# Bank Management - Part 6
----
**Goal**: create the `Bank` class.

## Task 1
------
Create a `Bank` class inside `Bank.java`.

## Task 2
------
The `Bank` class defines two fields: 
- `ArrayList<Account> accounts;`
- `ArrayList<Transaction> transactions`;

## Task 3
------
Add a constructor that receives no parameters. Your constructor will initialize each `ArrayList`.

## Task 4
------
Define the following method:
```java
    /**
     * Name: addAccount
     * @param account (Account)
     * 
     * Inside the function:
     *   1. adds an account to the accounts ArrayList
     */
```
Because `Account` is `abstract`, you will not be able to create a `new Account` copy. So, what's the solution?

## Task 5
-----
Inside the `Account` class, create an `abstract` method called `clone()`.
 
```java
    public abstract Account clone();
```
This will force every child to override a `clone()` method.

## Task 6
-----
Override the `clone()` method inside every child class. The purpose of `clone()` is to return a **`new`** copy of the current object: **`this`**.

## Task 7
-----
Add the following snippet inside `main()`.

```java
  Chequing chequing = new Chequing("f84c43f4-a634-4c57-a644-7602f8840870", "Michael Scott", 1524.51);
  Account chequingCopy = chequing.clone();

  Savings savings = new Savings("ce07d7b3-9038-43db-83ae-77fd9c0450c9", "Saul Goodman", 2241.60);
  Account savingsCopy = savings.clone();
```
Test your `clone()` method by adding four breakpoints and visualizing the runtime. Confirm that `clone()` returns a copy of the object.

## Task 8
-----
Revisit task 4 and fix `addAccount()`.

## Good Luck!
--------
##### Subscribe to our [YouTube Channel](https://www.youtube.com/@RayanSlim087?sub_confirmation=1) and Discover More Valuable Content!