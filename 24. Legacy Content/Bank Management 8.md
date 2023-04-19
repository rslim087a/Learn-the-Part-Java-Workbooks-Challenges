# Bank Management - Part 8
----
**Goal**: Set up `Main`.
 

## Task 1
---
Inside `Main`, create a new `Bank` object. 
```
static Bank bank = new Bank();
```

## Task 2
Define a method based on the Doc comment.

```java
    /**
     * Name: createObject
     * @param values (String[] values)
     * @return Account
     * 
     * Inside the function:
     *   1. Dynamically creates a Chequing, Loan, or Savings object based on the values array. 
     */
```
A `values` parameter would have four elements. For example:

    {"Chequing","f84c43f4-a634-4c57-a644-7602f8840870","Michael Scott","1524.51"};

You can approach this task in one of two ways:

1. Use a `switch` statement that creates an object based on the first element in `values`.
2. Use the following syntax to dynamically create an object based on the first element in `values`.
```
    Class.forName("src.main.model.account." + first_element)
          .getConstructor(String.class, String.class, double.class)
          .newInstance(second_element, third_element, fourth_element);
```
You can choose either option. Option 2 is better than option 1 because it's dynamic whereas option 1 involves code duplication. If you choose option 2, it throws a lot of checked exceptions. Instead of catching each one separately, consider that `Exception` is the base class for all exceptions (think of polymorphism).

```java
catch (Exception e) {
    System.out.println(e.getMessage());
}
```
Whether you choose option 1 or 2, call `createObject()` from `main()` using the `values` array and confirm that an object gets created.

```java
    String[] values = new String[] {"Chequing","f84c43f4-a634-4c57-a644-7602f8840870","Michael Scott","1524.51"};
```

![Screen Shot 2021-09-02 at 7.19.21 PM.png](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F499ed087-8d2e-41b2-9f9d-de0f23d339cc?alt=media&token=445943e7-f3bf-46e7-9fb6-f7b772f0d0c0)

After you confirm the method works, clear `main()`.

## Task 3
----
Define a method based on the Doc Comment.
```java
    /**
     * Name: returnAccounts()
     * @return ArrayList<Account>
     * @throws FileNotFoundException
     * 
     * Inside the function:
     *    1. Creates a Scanner object and reads the data from accounts.txt.
     *    2. Creates an Account object for every line in accounts.txt.
     *    3. Returns an ArrayList of Account objects.
     */
 ```

Call the method from `main()` and confirm the resulting `ArrayList` has 16 elements.

![Screen Shot 2021-09-02 at 6.46.05 PM.png](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F2dbf2c86-d1c0-41cd-a03e-dcd6bc75490e?alt=media&token=c79a7e0a-f158-419b-bade-48cfe59cabe0)

## Task 4
-----
Define a method based on the Doc Comment.

```java
    /**
     * Name: loadAccounts
     * @param accounts (ArrayList<Account>)
     * 
     * Inside the function:
     *   1. Loads every account into the Bank object.
     *  
     */
```

## Task 5
-----
Define a method based on the Doc Comment.

```java
    /**
     * Name: returnTransactions()
     * @return ArrayList<Transaction>
     * @throws FileNotFoundException
     * 
     * Inside the function:
     *    1. Creates a Scanner object and reads the data from transactions.txt.
     *    2. Populates an ArrayList with transaction objects.
     *    3. Sorts the ArrayList.
     */
```

Call the method from `main()` and confirm the resulting `ArrayList` has 352 **sorted** transactions.

![Screen Shot 2021-09-02 at 7.26.24 PM.png](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F148fc5c7-9be5-49d8-ba95-0a1f32f1ed2f?alt=media&token=31c77341-05bd-463f-b007-d856468f3920)

## Task 6
-----
Define a method based on the following Doc Comment. 
```java
    /**
     * Name: runTransactions
     * @param transactions ArrayList<Transaction>
     * 
     * Inside the function:
     *  1. Executes every transaction using bank.execute.
     */
```


## Task 7
-----
Define a method that prints the transaction history of an account.

```java
    /**
     * Name: transactionHistory
     * @param id (String)
     * 
     * Inside the function
     *   1. Print: \t\t\t\t   TRANSACTION HISTORY\n\t
     *   2. Print every transaction that corresponds to the id. (Waits 300 milliseconds before printing the next one)
     *             - Use this format "\t"+transaction+"\n"
     *   3. Print: \n\t\t\t\t\tAFTER TAX\n
     *   4. Print: "\t" + account that corresponds to id +"\n\n\n\n"
     */
```

## Task 8
-----
Replace your `main()` method with the following and run your code.


```java
    public static void main(String[] args) {

        try {
            ArrayList<Account> accounts = returnAccounts();
            loadAccounts(accounts);

            ArrayList<Transaction> transactions = returnTransactions();
            runTransactions(transactions);
            bank.deductTaxes();
            for (Account account : accounts) {
                System.out.println("\n\t\t\t\t\t ACCOUNT\n\n\t"+account+"\n\n");
                transactionHistory(account.getId());
            }
            
         } catch (FileNotFoundException e) {
            System.out.println(e.getMessage());
        }
    }
```

**Final Output:**

![Untitled.gif](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2Fa2e02fce-f496-4232-a831-dc83e1b51713?alt=media&token=3206a9d3-5b0d-46c7-9d70-7d7753f67a4f)

## Good Luck!
--------
##### Subscribe to our [YouTube Channel](https://www.youtube.com/@RayanSlim087?sub_confirmation=1) and Discover More Valuable Content!