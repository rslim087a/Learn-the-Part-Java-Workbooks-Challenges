# Bank Management - Part 3
----

> **Test-Driven Development**: write tests before writing code. 

Unit testing results in modular code. Modular code is:

-   easy to test.
-   immune to bugs.
-   easy to understand.
-   scalable.

## Task 1
------
Based on the requirements, every child shares two common methods: `deposit` and `withdraw`. So, define two `abstract` methods inside the parent class. 

```java
    public abstract void deposit(double amount);
    public abstract boolean withdraw(double amount);
```

## Task 2
------
As you override `deposit` and `withdraw`, define this method inside `Account.java`. You will need it for your unit tests:

```java
 protected double round(double amount) {
     DecimalFormat formatter = new DecimalFormat("#.##");
     return Double.parseDouble(formatter.format(amount));
 }
```

If you live in **Europe** or **Asia**, your `Locale` probably uses `,` for decimals. Set your `DecimalFormat`'s `Locale` to English. 

```java
 protected double round(double amount) {
     DecimalFormat formatter = new DecimalFormat("#.##", new DecimalFormatSymbols(Locale.ENGLISH));
     return Double.parseDouble(formatter.format(amount));
 }
```

Inside `AccountTests`, create a method that runs before every test. Then, add three objects to the `accounts` array:


```java
   accounts = new Account[] {
       new Chequing("f84c43f4-a634-4c57-a644-7602f8840870", "Michael Scott", 1524.51),
       new Savings("ce07d7b3-9038-43db-83ae-77fd9c0450c9", "Saul Goodman", 2241.60),
       new Loan("4991bf71-ae8f-4df9-81c1-9c79cff280a5", "Phoebe Buffay", 2537.31)
   };
```
## Before you continue...
---
Please use the information from `requirements.txt` to guide your unit tests.

## Task 3
------
Create a unit test named `withdrawal`. Inside, withdraw 
`1440` from the chequing account and assert the resulting balance is `84.51`.

## Task 4
------
Create a unit test named `overdraft`. Inside, withdraw 
`1534.43` from the chequing account and assert the resulting balance is `-15.42`.

## Task 5
------
Create a unit test named `overdraftLimit`. Inside, withdraw 
`1726` from the chequing account and assert the resulting balance remains `1524.51`.

## Task 6
------
Create a unit test named `withdrawalFee`. Inside, withdraw 
`100` from the savings account and assert the resulting balance is `2136.60`.

## Task 7
------
Create a unit test named `withdrawalInterest`. Inside, withdraw 
`2434.31` from the loan account and assert the resulting loan balance is `5020.31`.

## Task 8
------
Create a unit test named `withdrawalLimit`. Inside, withdraw 
`7463.69` from the loan account. Your assertion must consider that the account's debt can't exceed `$10,000`.

## Task 9
------
Create a unit test named `deposit`. Make a `$5,000` deposit to  the `Chequing` account and assert the resulting balance is `6524.51`. 

The `deposit` method for `Savings` should be identical to `Chequing`.


## Task 10
------
Create a unit test named `loanDeposit`. Make a `$1,000` deposit to the `Loan` account and assert the resulting loan is `1537.31`.

## Task 11
-----
Confirm that every test passes. 

![Screen Shot 2021-08-26 at 11.34.48 PM.png](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F09caa973-2e40-4f45-9796-556c46030cee?alt=media&token=7327929b-b421-41b1-90aa-ca1dc7381833)

## Good Luck!
--------
##### Subscribe to our [YouTube Channel](https://www.youtube.com/@RayanSlim087?sub_confirmation=1) and Discover More Valuable Content!