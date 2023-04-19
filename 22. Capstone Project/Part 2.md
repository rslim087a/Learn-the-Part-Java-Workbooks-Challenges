# Capstone Project

This workbook assumes that you successfully completed Part 1.

## Task 1
Inside `TradeAccountRepository.java`, create a `TradeAccountRepository` class. The class will define a `private datastore` field:

```java
    private Map<String, TradeAccount> datastore = new HashMap<>();
```

The `datastore` field will be used to store `TradeAccount` objects using their `id` as the key.

## Task 2

- Create a method called `createTradeAccount` in the `TradeAccountRepository` class. 
- The method should have one parameter, a `TradeAccount` object, and return no value. 
- The `createTradeAccount` method should store a clone of the `TradeAccount` object in the datastore using the id field as the key.

## Task 3
- Create a method called `retrieveTradeAccount` in the `TradeAccountRepository` class. 
- The method should have one parameter, a `String id`, and return a `TradeAccount` object.
- The retrieveTradeAccount method should return a clone of the `TradeAccount` object stored in the datastore with the specified `id`.

## Task 4
- Create a method called `updateTradeAccount` in the `TradeAccountRepository` class. 
- The method should have one parameter, a `TradeAccount` object, and return no value.
- The updateTradeAccount method should update the `TradeAccount` object in the datastore using the `id` field as the key. It should store a clone of the `TradeAccount` object to ensure that the original object is not modified.

## Task 5
- Create a method called `deleteTradeAccount` in the `TradeAccountRepository` class. 
- The method should have one parameter, a `String id`, and return no value.
- The `deleteTradeAccount` method should remove the `TradeAccount` object with the specified `id` from the datastore.

## Task 6
 Test your implementation by creating a `TradeAccountRepository` object and performing the create, retrieve, update, and delete operations.

```java
    public static void main(String[] args) {
        TradeAccountRepository repository = new TradeAccountRepository();

        CashAccount cashAccount = new CashAccount("C123", new BigDecimal("1000.00"));
        repository.createTradeAccount(cashAccount);

        MarginAccount marginAccount = new MarginAccount("M456", new BigDecimal("5000.00"));
        repository.createTradeAccount(marginAccount);

        TradeAccount retrievedCashAccount = repository.retrieveTradeAccount("C123");
        System.out.println("Retrieved Cash Account ID: " + retrievedCashAccount.getId());
        System.out.println("Cash Balance: " + ((CashAccount) retrievedCashAccount).getCashBalance());

        TradeAccount retrievedMarginAccount = repository.retrieveTradeAccount("M456");
        System.out.println("Retrieved Margin Account ID: " + retrievedMarginAccount.getId());
        System.out.println("Margin: " + ((MarginAccount) retrievedMargin
```

----------

##### Subscribe to our [YouTube Channel](https://www.youtube.com/@RayanSlim087?sub_confirmation=1) and Discover More Valuable Content!