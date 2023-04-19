# Stock Trading

The stock trading application will test your ability to apply concepts from module two. It will also challenge you to get creative and research.

![Untitled 3.gif](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2Fa498a8da-62db-4a63-b74f-9fe0e8c341a9?alt=media&token=cef5c26c-c99e-4dba-a3a2-c4c86a2c5a7f)

## Attention: Windows Users

Use the **Git Bash** console to run this project. You can download Git Bash here: https://git-scm.com/downloads.

![Screen Shot 2022-06-24 at 3.18.34 PM.png](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F0a36c0f8-247b-4a55-9ace-e4619043777d?alt=media&token=abbba2ef-6448-4cb5-b1f5-b00ae1bc63a4)

Git Bash will successfully interpret the color codes used in this project.

**Instructions**
================

The instructions are not detailed because there are many ways to solve this challenge. It's up to you to come up with a plan of action.

## **a) Open the starter project**
-----------------------------------

![Screen Shot 2021-10-03 at 11.03.13 PM.png](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F4cd1caf9-6721-42c5-9bcb-f272f8604b27?alt=media&token=d88e7493-825a-4316-84dd-ae9d241bfbb4)
## **b) Inheritance**
-----------------------------------

From the requirements, identify the parent and children classes. 


## c) Test-Driven Development
----- 

> **Test-Driven Development:** Writing tests before writing code. 

Read the requirements before writing any of the following unit tests.

**Buy Tests:**

- Shares of a stock for a `Personal` account increase after purchase.
- Shares of a stock for a `TFSA` increase after purchase.
- No shares are added in the event of insufficient funds.
- Funds available in a `Personal` account decrease after purchase.
- Funds available in a `TFSA` decrease after purchase (must account for `TRADE_FEE`).

**Sell Tests:**

- Shares of a stock for a `Personal` account decrease after purchase.
- Shares of a stock for a `TFSA` decrease after purchase.
- No funds are added if shares being sold exceeds shares owned.
- Funds available in a `Personal` account increase after sale (must account for `SALE_FEE`).
- Funds available in a `TFSA` increase after sale (must account for `TRADE_FEE`).

## d) Aesthetics
----- 

Your children classes must inherit this `toString`.


```java
    public String toString() {
        return "\n  Stock\t\t"  + Color.RESET + "Shares" +
        "\n\n" + displayPortofolio() + Color.RESET +
        "\n  Funds Left\t" + Color.GREEN + "$" + round(this.getFunds()) + Color.RESET;
    }
```

## **e) Main**
-----------------------
Your `Main` class contains pre-defined methods. 

### **Part 1** 
First, call the method that explains the application to the user.

### **Part 2** 
After the user chooses an account, call the method that displays their initial balance.

### **Part 3** 
There are 2160 records in each CSV file. Create a loop that runs from 1 to 2160.


```java
        for (int day = 1; day <= 2160; day++) {
         
        }
```

During each run, display the prices (see **`part 4`** first). 

### **Part 4** 
You must learn to stream the elements of a CSV file. Inside `getPath()`, use the following code to return the **`Path`** of the CSV file.

`Path path = Paths.get(Thread.currentThread().getContextClassLoader().getResource("src/main/data/"+stock+".csv").toURI());`

Catch the checked exception as needed.

### **Part 5** 
Complete the `getPrice()` method.

**Hints:**
- You can run through all lines as a stream of elements using: `Files.lines(path)`.

- You must skip the first element in each file (the column headers). You can skip an element in a stream using `.skip(element number)`.
- **Intermediate Operations**:
``` java
    .filter(filter value that matches day)
    .map(map to price value)
```
- **Terminal Operations**:
``` java
    .findFirst()
    .orElse(null)
```
### **Part 6** 
After displaying the prices, ask the user to
 - `buyOrSell()`
 - `chooseStock()`
 - `numShares()`

Then execute the `buy/sell` trade with your `Account` object.

### **Part 7** 
Call `tradeStatus()` to notify the user of a `"successful"` or `"unsuccessful"` trade.

## **f) Research**
----------------------- 
Don't be afraid to research! As a developer, it's important that you practice finding resources online. 

## **g) Run the finished application**
----------------------- 
Before you start coding, I encourage you to run the finished application and get familiar with the output. 

![Untitled 3.gif](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2Fa498a8da-62db-4a63-b74f-9fe0e8c341a9?alt=media&token=cef5c26c-c99e-4dba-a3a2-c4c86a2c5a7f)

## Good luck!
--------
##### Subscribe to our [YouTube Channel](https://www.youtube.com/@RayanSlim087?sub_confirmation=1) and Discover More Valuable Content!