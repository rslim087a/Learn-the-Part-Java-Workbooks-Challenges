# Quidditch – Part 2

**Goal**: Quality control the `Team` class.

Unchecked exceptions
--------------------

An **unchecked** exception crashes the app as a result of badly written code.

You should throw an:

-   `IllegalArgumentException` when the caller passes faulty arguments into a method/constructor.

-   `IllegalStateException` when an object calls its method at a "bad time" (object not in a legal state).

Throwing an unchecked exception forces the caller to improve their code.

## **Task 1 –** `Team` **Constructor**
---------------------------------------

In the `Team` constructor, throw an `IllegalArgumentException` if:

-   any of the fields are `null`.

-   any of the `String` values are blank.

-   `chasers` `length` not equal to 3. 

## **Task 2**

### 1. Create a test that fails
---
Write a unit test named `hasNullTest`. The test defines the following array. Then, use `assertTrue` to check if the array `hasNull`.

```java
String[] chasers = new String[] {null, "Ginny", "Katie"});
```
Inside `Team.java`, write code to make the test fail. 
Make the method `static` because it doesn't interact with any fields. By making it `static`, it belongs to the `class`, so you can call it directly from the `class`.

```java
    /**
     * Function name: hasNull
     * @param array
     * @return (boolean)
     * 
     * Inside the function:
     *    1. return false;
     */
 ```
### 2. Make the test pass 

Inside the function, use a `for` loop that runs through the length of the parameter. `return true` if any element is `null`.

### 3. Refactor
--- 
![Screen Shot 2021-07-13 at 2.25.19 PM.png](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F20cbf07a-15a6-4919-b884-927ac8de1d13?alt=media&token=59b5c4a4-e26f-41e6-b42b-7dca8ad1d73d)

1. You can pass regular arrays into an `Arrays.stream()` pipeline.

2. `anyMatch` is a terminal operation that returns `true` if **ANY** element matches the predicate, and `false` otherwise.

### 4. Refactor
--- 
Refactor if necessary.





## **Task 3**

### 1. Create a test that fails
---

Write a unit test named `hasBlankTest`. Inside, use `assertTrue` and call `hasBlank` to assert the array below has a blank field:
```java
String[] chasers = {"    ", "Ginny", "Katie"};                  
```
Then, write code to make the test fail.
```java
    /**
     * Function name: hasBlank
     * @param array
     * @return (boolean)
     * 
     * Inside the function:
     *    1. return false;
     */
 ```

### 2. Make the test pass
See Task 2.

### 3. Refactor 
Refactor if necessary.

## **Task 4**

Inside the constructor, throw an `IllegalArgumentException` if an array `hasNull` or `hasBlank`.

## **Task 5**

Apply the same quality control inside every setter. Use the following function for `setHouse`, `setKeeper`, and `setSeeker`:

    public void checkParam(String param) {
        if (param == null || param.isBlank()) {
            throw new IllegalArgumentException(param + " cannot be null or blank");
        }
    }


**Final Remarks**
---------------
- You added checkpoints to the `Team` `class`. Each checkpoint forbids the caller from misusing the methods/constructor.

- You unit tested two methods. Each method is modular and free of bugs.

![Screen Shot 2021-07-13 at 3.58.46 PM.png](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F79a6be41-8f1a-4509-99e9-57308ffa201d?alt=media&token=4b32bf70-1c36-492c-b628-1f436a0e0b0e)

--------
##### Subscribe to our [YouTube Channel](https://www.youtube.com/@RayanSlim087?sub_confirmation=1) and Discover More Valuable Content!