# Bank Management - Part 4
----

> **Interface**: a contract of behavior.

A class that implements an interface must override all of its methods.
## Task 1
------
Based on the requirements, `Chequing` implements a `Taxable` interface. Add a `void tax(double income)` method inside `Taxable` and override it inside `Chequing`.

## Task 2
------
Create a unit test named `incomeTax()`.
- deposit `$4,000` into the chequing account.
- call `tax()` for an income of `$4,000`.
- assert the resulting balance is `5374.51`.

You can find the taxable income and tax rate inside `requirements.txt`. 

## Good Luck!
--------
##### Subscribe to our [YouTube Channel](https://www.youtube.com/@RayanSlim087?sub_confirmation=1) and Discover More Valuable Content!