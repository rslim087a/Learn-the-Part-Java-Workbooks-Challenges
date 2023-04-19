# Capstone Project

This workbook assumes that you successfully completed Part 3.

## Preliminary Task
Remove all the code inside of your `Main` class. At the class level, declare the following variables:
```java
static Path[] paths = new Path[] {Paths.get("data/accounts.txt"), Paths.get("data/transactions.txt")};

static TradeAccountRepository tradeAccountRepository = new TradeAccountRepository();
static CashAccountService cashAccountService = new CashAccountService(tradeAccountRepository);
static MarginAccountService marginAccountService = new MarginAccountService(tradeAccountRepository);
```

- The `paths` array holds the file paths for `data/accounts.txt` and `data/transactions.txt`.
- Instances of `TradeAccountRepository`, `CashAccountService`, and `MarginAccountService` will be used to manage the data.


## Task 1
- Write a method called `loadTradeAccounts` to read the file data/accounts.txt. 
- For each line in the file, split the line into an array of strings and create either a `CashAccount` or a `MarginAccount` object based on the account type. 
- Add the created account to the corresponding account service (`cashAccountService` or `marginAccountService`).


## Task 2

- Write a method called `applyTransactions` to read the file data/transactions.txt. 
- For each line in the file, split the line into an array of strings and determine the account type, transaction type (`DEPOSIT` or `WITHDRAW`), and the amount. 
- Use the appropriate account service (`cashAccountService` or `marginAccountService`) to deposit or withdraw the specified amount.

## Task 3

Copy this method to print the cash balance of the `CashAccount` and `MarginAccount` objects.

```java
public static void finalTest() throws IOException {
    System.out.println("Account A1234B Cash Balance: " + cashAccountService.retrieveTradeAccount("A1234B").getCashBalance());
    System.out.println("Account E3456F Cash Balance: " + cashAccountService.retrieveTradeAccount("E3456F").getCashBalance());
    System.out.println("Account I5678J Cash Balance: " + cashAccountService.retrieveTradeAccount("I5678J").getCashBalance());
    System.out.println("Account C2345D Margin: " + marginAccountService.retrieveTradeAccount("C2345D").getMargin());
    System.out.println("Account G4567H Margin: " + marginAccountService.retrieveTradeAccount("G4567H").getMargin());
}
```

## Task 4

In the `main` method, use a `try-catch` block to call the `loadTradeAccounts`, `applyTransactions`, and `finalTest` methods.

```java
public static void main(String[] args) {
    try {
        loadTradeAccounts();
        applyTransactions();
        finalTest();
    } catch (IOException exception) {
        System.out.println(exception.getMessage());
    }
}
```

### Expected Output
```java
Account A1234B Cash Balance: 512.00
Account E3456F Cash Balance: 325.45
Account I5678J Cash Balance: 125.20
Account C2345D Margin: 15.40
Account G4567H Margin: 224.95
```

# Congratulations on Finishing the Course!

----------

##### Subscribe to our [YouTube Channel](https://www.youtube.com/@RayanSlim087?sub_confirmation=1) and Discover More Valuable Content!