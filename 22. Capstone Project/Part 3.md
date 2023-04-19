# Capstone Project

This workbook assumes that you successfully completed Part 2.

## Task 1
Create an interface called `TradeAccountService` with two methods:

```java
public interface TradeAccountService {
    public void deposit(String id, BigDecimal amount);
    public void withdraw(String id, BigDecimal amount);
}
```

## Task 2
Create a class called `CashAccountService` that implements the `TradeAccountService` interface. The class should have a `TradeAccountRepository` object as a private field.

## Task 3
In the `CashAccountService` class, implement the `deposit` and `withdraw` methods:

 - The `deposit` method should add the given amount to the `cashBalance` field of the specified `CashAccount` object.
 - The `withdraw` method should subtract the given amount from the `cashBalance` field of the specified `CashAccount` object.

Also, implement the following methods:

 - `createTradeAccount`
 - `retrieveTradeAccount`
 - `updateTradeAccount`
 - `deleteTradeAccount`

These methods should interact with the `TradeAccountRepository` object to manage `CashAccount` objects.

## Task 4
Create a class called `MarginAccountService` that implements the `TradeAccountService` interface. The class should have a `TradeAccountRepository` object as a `private` field:

## Task 5
In the `MarginAccountService` class, implement the `deposit` and `withdraw` methods:

 - The `deposit` method should add the given amount to the `margin` field of the specified `MarginAccount` object.
 - The `withdraw` method should subtract the given amount from the `margin` field of the specified `MarginAccount` object.

Also, implement the following methods:

 - `createTradeAccount`
 - `retrieveTradeAccount`
 - `updateTradeAccount`
 - `deleteTradeAccount`

These methods should interact with the `TradeAccountRepository` object to manage `MarginAccount` objects.

## Task 6

Below is a code snippet to test your implementation. Make sure that you get a similar output.

### Output
```
>>: Updated CashAccount balance: 1300
>>: Updated MarginAccount margin: 2500
```

### Sample Code
```java

public static void main(String[] args) {
    TradeAccountRepository repository = new TradeAccountRepository();
    CashAccountService cashAccountService = new CashAccountService(repository);
    MarginAccountService marginAccountService = new MarginAccountService(repository);

    // Create CashAccount and MarginAccount objects
    CashAccount cashAccount = new CashAccount("1", BigDecimal.valueOf(1000));
    MarginAccount marginAccount = new MarginAccount("2", BigDecimal.valueOf(2000), BigDecimal.valueOf(10000));

    // Add the accounts to the repository
    cashAccountService.createTradeAccount(cashAccount);
    marginAccountService.createTradeAccount(marginAccount);

    // Deposit and withdraw amounts
    cashAccountService.deposit("1", BigDecimal.valueOf(500));
    cashAccountService.withdraw("1", BigDecimal.valueOf(200));
    marginAccountService.deposit("2", BigDecimal.valueOf(1000));
    marginAccountService.withdraw("2", BigDecimal.valueOf(500));

    // Retrieve and print the updated account balances
    CashAccount updatedCashAccount = cashAccountService.retrieveTradeAccount("1");
    MarginAccount updatedMarginAccount = marginAccountService.retrieveTradeAccount("2");
    System.out.println("Updated CashAccount balance: " + updatedCashAccount.getCashBalance());
    System.out.println("Updated MarginAccount margin: " + updatedMarginAccount.getMargin());

    // Delete the accounts
    cashAccountService.deleteTradeAccount("1");
    marginAccountService.deleteTradeAccount("2");
}
```

----------

##### Subscribe to our [YouTube Channel](https://www.youtube.com/@RayanSlim087?sub_confirmation=1) and Discover More Valuable Content!