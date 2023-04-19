# Bank Management - Part 5
----
**Goal**: create the `Transaction` class.

## Task 1
------
Create a `Transaction` class inside `Transaction.java`.

## Task 2
------
The `Transaction` class defines four fields: 
- `type`
- `long timestamp`
- `String id`
- `double amount`

**Hint:** `type` can only be `WITHDRAW` or `DEPOSIT`.
## Task 3
------
Add a constructor.

## Task 4
------
Add a copy constructor.

## Task 5
------
Add getters/setters.

## Task 6
------
The `long` `timestamp` represents the number of **seconds** since 1970. The constructor for `Date` objects returns a `Date` based on **milliseconds** since 1970.
 
![Screen Shot 2021-09-02 at 11.21.44 PM.png](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2Fce435009-c519-46b8-8ba2-3e3e1c9b3f52?alt=media&token=100d58e8-1da8-4bd0-8e63-8fbda198cfb3)

- Based on that information, think of how you'd create a **correct** `Date` object.

- Research how to format your `Date` object into `dd-MM-yyyy` `String`.

- Don't write any code yet.

## Task 7
------
Inside the `test` folder, create another file named `TransactionTests.java`. Then, add the following `@Before` method:


```
    Transaction transaction;

    @Before
    public void setup() {
        transaction = new Transaction(Transaction.Type.WITHDRAW , 1546905600, "6b8dd258-aba3-4b19-b238-45d15edd4b48", 624.99);
    }

```

## Task 8
------
Create a unit test named `correctDateTest`. `correctDateTest` must assert calling `returnDate()` from the transaction object returns `"07-01-2019"` **OR** `08-01-2019` depending on your time zone.

## Task 9
------
Override `equals()`, `hashCode()`, and make transaction objects "sortable" from lowest to highest timestamp.

## Task 10
------
Override `toString()` and use this format:
```
    @Override
    public String toString() {
        return (type) + "    " +
            "\t" + date dd-mm-yyyy + "" +
            "\t" + id + "" +
            "\t$" + amount + "";
    }
```

## Task 11 – Quality Control
------
- `long timestamp` is **always** valid:
   - Positive timestamp is seconds since 1970.
   - Negative timestamp is seconds that precede 1970. 
- `id` can't be null or blank.
- `amount` can't be negative. The app will determine deposits/withdrawals based on the `type`.

## Good Luck!
--------
##### Subscribe to our [YouTube Channel](https://www.youtube.com/@RayanSlim087?sub_confirmation=1) and Discover More Valuable Content!