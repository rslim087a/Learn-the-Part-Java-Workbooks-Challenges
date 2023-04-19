# Quidditch – Part 3

**Prerequisite**: You finished the lesson: `HashMap`.

**Goal**: set up the `Game class`.

## **Task 1**
-----------------------------
`scoreboard` implies parity between `Team` and `Integer`. Define a `HashMap` that can store `Team` : `Integer` entries.

## **Task 2**
----------------------

1.  Constructor.

    -  Two parameters: `Team home`, `Team away`.

    -  Sets `scoreboard` equal to a new object of the `HashMap class`.
  
    -   Adds `home`:`0` and `away`:`0` to the scoreboard.    

2.  Getter: `getScore`

    -   Receives one parameter: `Team team`.

    -   Returns the score for the requested `team`.

3.  Setter: `setScore`

    -   Receives two parameters: `Team team`, `Integer Score`.

    -   Updates a `team`'s score to 50.

4.  Getter: `getTeam`. 
    -   Receives one parameter: `String name`.
    -   `return null` for now.
5.  Setter: `setTeam`

    -   **Impossible**
    - You cannot update a key.

## Task 4
--------------------------------

### 1. Test the constructor 

Inside `main()`, create a new object of the `Game` class. Pass the following objects into the constructor.

```java
  home = new Team("GRYFFINDOR", "Oliver", "Harry", 
    new String[] {"Angelina", "Ginny", "Katie"});
  
  away = new Team("SLYTHERIN", "Vincent",  "Draco", 
    new String[] {"Bridget", "Harper", "Malcolm"});
```
### **Compare your output with one of the following scenarios:**
---
1. **Reference Trap:** each key shares the same reference as the outside variable.
    - **Pitfall**: updating the outside variable updates the key in the `HashMap`


![Screen Shot 2021-07-11 at 2.06.58 PM.png](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F99f9b7e8-c5e8-4e0b-ac78-7cf4adbbe131?alt=media&token=981f3924-4f89-4711-ba20-7aed3822d4e6)


2. **Correct Result**: each key should store a unique reference that points to a copy.

![Screen Shot 2021-07-11 at 2.09.27 PM.png](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F7b9dc85d-6fdb-4996-892b-1545b4b4cbb9?alt=media&token=e9d2384f-4fe2-4365-bbfd-65f7a8371389)

### 2. `getScore`

From `main()`, fetch the score for `gryffindor` and print it. If you did everything correctly, it **should not** work and return `null`.

### 3. `setScore`

From `main()`, update the score for `gryffindor` to `50`. If you did everything correctly, it **should not** work. It should add a new key to the `HashMap` instead. Use breakpoints to confirm your result. 

## **Task 5: `equals`**
--------------------------------

Your code is using the default `equals` method to compare `Team` objects.

- **Problem**: The default `equals` method compares references. But, each key has a different reference from the one being passed in.

   - `getScore`: It can't find a reference that matches the parameter, so it returns `null`.

   - `setScore`: It can't find a reference that matches the parameter. So, it adds a new key instead of updating the existing one.

- **Solution**: The code needs *your* `equals` method to compare `Team` objects. **Hint:** arrays are equal if they share the same `toString`.

After creating your `equals()` method, re-launch the 
debugger.
**The code should still not work!**
## What's wrong?
--------------------------------
Adding an `equals()` method is not enough. You also need to add a **`hashCode()`** method.

--------
##### Subscribe to our [YouTube Channel](https://www.youtube.com/@RayanSlim087?sub_confirmation=1) and Discover More Valuable Content!