# Bank Management - Part 7
----
**Goal**: Finalize the `Bank` class.
 
## Task 1
------
Create an `addTransaction` method.


```java
    /**
     * Name: addTransaction
     * @param transaction
     * 
     * Inside the function:
     *   1. adds a new transaction object to the array list.
     */
```

## Task 2
------
Define the following:

```java
  /**
   * Name: getTransactions
   * @param accoundId (String)
   * @return (Transaction[])
   * 
   * 1. returns an array of transactions whose id matches the accountId 
   */
```
As you define the method, use a stream and run through a pipeline of operations:

**Intermediate Operation**
1. `filter`: Filters elements based on a predicate.

**Terminal Operation**

2. `collect`: Collects the stream elements. Use the familiar `toList` collector to collect elements into a `List`.

Finally, convert the resulting `List` to an array by using `toArray`. By default, `toArray` returns `Object[]`. You can force `toArray` to return a specific type using this syntax:

```
list.toArray(new CustomClass[list.size()]);
```

## Task 3
------
Add the code snippet below inside `main()`. The code:
 1. Loops through an array of accounts and adds them to a `Bank` object. 
 2. Loops through an array of transactions and adds to them to the same `Bank` object.
 3. Gets every the transaction that matches the account: `"f84c43f4-a634-4c57-a644-7602f8840870"`

```java
        Account[] accounts = new Account[] {
            new Chequing("f84c43f4-a634-4c57-a644-7602f8840870", "Michael Scott", 1524.51),
            new Savings("ce07d7b3-9038-43db-83ae-77fd9c0450c9", "Saul Goodman", 2241.60)
        };

        for (Account account : accounts) {
            bank.addAccount(account);
        }

        Transaction[] transactions = new Transaction[] {
            new Transaction(Transaction.Type.WITHDRAW, 1546905600, "f84c43f4-a634-4c57-a644-7602f8840870", 624.99),
            new Transaction(Transaction.Type.DEPOSIT, 1578700800, "f84c43f4-a634-4c57-a644-7602f8840870", 441.93),
            new Transaction(Transaction.Type.WITHDRAW, 1547078400, "f84c43f4-a634-4c57-a644-7602f8840870", 546.72),
            new Transaction(Transaction.Type.WITHDRAW, 1546732800, "f84c43f4-a634-4c57-a644-7602f8840870", 546.72),
            new Transaction(Transaction.Type.DEPOSIT, 1578355200, "f84c43f4-a634-4c57-a644-7602f8840870", 635.95),
            new Transaction(Transaction.Type.WITHDRAW, 1547078400, "ce07d7b3-9038-43db-83ae-77fd9c0450c9", 875.64),
            new Transaction(Transaction.Type.WITHDRAW, 1578614400, "ce07d7b3-9038-43db-83ae-77fd9c0450c9", 912.45),
            new Transaction(Transaction.Type.WITHDRAW, 1577836800, "ce07d7b3-9038-43db-83ae-77fd9c0450c9", 695.09),
            new Transaction(Transaction.Type.WITHDRAW, 1609459200, "ce07d7b3-9038-43db-83ae-77fd9c0450c9", 917.21),
            new Transaction(Transaction.Type.WITHDRAW, 1578096000, "ce07d7b3-9038-43db-83ae-77fd9c0450c9", 127.94),
            new Transaction(Transaction.Type.WITHDRAW, 1546819200, "ce07d7b3-9038-43db-83ae-77fd9c0450c9", 612.52)
        };

        for (Transaction transaction : transactions) {
            bank.addTransaction(transaction);
        }
        
        Transaction[] filteredTransactions = bank.getTransactions("f84c43f4-a634-4c57-a644-7602f8840870");

```
Place a breakpoint next to the `filteredTransactions` line and make sure it contains 5 elements:

![Screen Shot 2021-08-31 at 11.11.57 PM.png](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2Fb5ebc946-a629-4ae3-b41a-48269b18dd7c?alt=media&token=09a89493-f296-4462-9eca-811eeaa46ae7)

## Task 4
------

Inside `Bank`, define the following:

```java
  /**
   * Name: getAccount()
   * @param transactionId (String)
   * @return (Account)
   * 
   * 1. returns an account whose id matches a transaction. 
   */
```
As you define the method, run a stream through a pipeline of operations:

1. `filter`: Filters elements based on a predicate.
2. `findFirst()`: returns the first element of the stream.
3. `orElse(null)`: return null otherwise.

Then, test your `get` method inside `main()` by adding this line:

```
Account account = bank.getAccount("ce07d7b3-9038-43db-83ae-77fd9c0450c9");

```
Place a breakpoint next to the `account` line and make sure it defines the following object:

![Screen Shot 2021-08-31 at 11.28.40 PM.png](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F760ffd0e-be43-4f97-9129-03c49a550468?alt=media&token=15567978-9990-421d-a272-679cf0f29ee3)

## Task 5
------
Make `addTransaction` `private` and remove the code inside `main()`. 

The caller is forbidden from adding transactions. It's the bank that decides to add successful transactions and ignore the ones that fail.

## Unit Tests
------
You need to unit test the behavior inside `requirements.txt`.

```
    The bank keeps a record of every account created and transaction made.
    The bank can execute transactions for any account. 
    Depending on the account, some transactions may be denied. <----
    The bank can deduct taxes from taxable accounts. <-----

```
 - The third line requires two unit tests. 
    - Test if the bank keeps a record of successful transactions.
    - Test if the bank ignores failed transactions.
 - The fourth line requires one unit test.

## Task 5
------

Inside `test`, create a new file named `BankTests.java`. Then, add the following `@Before` method:

```java
  Bank bank;

  @Before
  public void setup() {
      bank = new Bank();
      bank.addAccount(new Chequing("f84c43f4-a634-4c57-a644-7602f8840870", "Michael Scott", 1524.51));
    }

```

## Task 6
------
Create a unit test named `successfulTransactions`. `successfulTransactions` must assert `getTransactions("f84c43f4-a634-4c57-a644-7602f8840870").length` returns 2 after a successful withdrawal and deposit.
```java
    @Test
    public void successfulTransaction() {
        this.bank.withdrawTransaction(new Transaction(Transaction.Type.WITHDRAW, 1546905600, "f84c43f4-a634-4c57-a644-7602f8840870", 624.99));
        this.bank.depositTransaction(new Transaction(Transaction.Type.DEPOSIT, 1578700800, "f84c43f4-a634-4c57-a644-7602f8840870", 441.93));
        assertEquals(2, bank.getTransactions("f84c43f4-a634-4c57-a644-7602f8840870").length);
    }
```
`withdrawTransaction` and `depositTransaction` get the account that a transaction belongs to and executes the transaction.


## Task 7
------
Create a unit test named `failedTransaction`. `failedTransaction` must assert `getTransactions("f84c43f4-a634-4c57-a644-7602f8840870").length` returns 0 after a failed withdrawal.

        this.bank.withdrawTransaction(new Transaction(Transaction.Type.WITHDRAW, 1546905600, "f84c43f4-a634-4c57-a644-7602f8840870", 10000000));
        assertEquals(0, bank.getTransactions("f84c43f4-a634-4c57-a644-7602f8840870").length);

## Task 8
------
Make `withdrawTransaction` and `depositTransaction` `private`. Inside Bank.java, create a method named `executeTransaction`.


```java
    /**
     * Name: executeTransaction
     * @param transaction
     * 
     * Inside the function:
     *  1. calls withdrawTransaction if transaction type is WITHDRAW
     *  2. calls depositTransaction if transaction type is DEPOSIT
     * 
     */
```
Call executeTransaction for your unit tests.

## Task 9
------
Create a `private` method called `getIncome`. 

```java
    /**
     * Name: getIncome
     * @param account (Taxable)
     * @return double
     * 
     * Inside the function:
     *   1. Gets every transaction that matches the account's id.
     *   2. Maps every transaction to a double.
     *       - Transactions of type WITHDRAW are mapped to negative numbers.
     *       - Transactions of type DEPOSIT are mapped to positive numbers.
     *   3. Takes the sum of every number and returns the income.
     * 
     */
```
## Task 10
------
Create a unit test named `taxDeduction()`. `taxDeduction` must assert calling `deductTaxes()` deducts taxes for `Taxable` objects whose income exceeds 3000.

    @Test
    public void taxDeduction() {
        this.bank.executeTransaction(new Transaction(Transaction.Type.DEPOSIT, 1578700800, "f84c43f4-a634-4c57-a644-7602f8840870", 4000));
        this.bank.deductTaxes();
        assertEquals(5374.51, bank.getAccount("f84c43f4-a634-4c57-a644-7602f8840870").getBalance());
    }

Inside `Bank.java`, you can check if an object is `Taxable` using this syntax: `Taxable.class.isAssignableFrom(account.getClass())`.

## Task 11
------
If your test passes, give it another transaction. The resulting balance for account `"f84c43f4-a634-4c57-a644-7602f8840870"` after tax deduction should be `4949.51`.

    @Test
    public void taxDeduction() {
        this.bank.executeTransaction(new Transaction(Transaction.Type.DEPOSIT, 1578700800, "f84c43f4-a634-4c57-a644-7602f8840870", 4000));
        this.bank.executeTransaction(new Transaction(Transaction.Type.WITHDRAW, 1578700800, "f84c43f4-a634-4c57-a644-7602f8840870", 500));

        this.bank.deductTaxes();
        assertEquals(4949.51, bank.getAccount("f84c43f4-a634-4c57-a644-7602f8840870").getBalance());
    }



## Task 12
------
Confirm that all of your tests pass.

![Screen Shot 2021-09-01 at 2.28.59 AM.png](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F4b700741-6744-4ae7-a68d-f1c4a623840d?alt=media&token=e4531faf-f246-4ed7-871c-95a3f863dc80)

## Good Luck!
--------
##### Subscribe to our [YouTube Channel](https://www.youtube.com/@RayanSlim087?sub_confirmation=1) and Discover More Valuable Content!