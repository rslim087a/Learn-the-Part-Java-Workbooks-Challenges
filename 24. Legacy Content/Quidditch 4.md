# Quidditch – Part 4 
**Prerequisite**: You finished the lesson: `hashCode()`.

## Background
---
> `equal` objects **must** share the same `hashCode`.

When you add an `equals()` method, you **must** also add a `hashCode()` method that assigns equal objects the same hashCode.

1. `HashMap` uses the `hashCode` to find which bucket the key is in.
2. **After it finds the bucket**, `equals()` can compare your object against the key.

![Untitled.gif](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F547e6d87-a2c7-47c4-bf81-973f771e095a?alt=media&token=4d8a9afc-f604-4795-8ef2-af161a341037)

## **Task 1**
---
Inside `Team.java`, add a `hashCode` method that assigns equal objects the same `hashCode`. 

**NOTE:** `Objects.hash()` doesn't work with arrays. Pass the `chasers` field in as a **`String`**: `Arrays.toString(chasers)`.

## **Task 2: Test your code**
---
**Expected Output:**
1. `getScore` should return the score 0.
2. `setScore` should update gryffindor's score.

## Task 3: `getTeam`
----
You will retrieve the `Team` key that matches the `String` parameter.

**Background information:**
1. You can run through **`key-value`** pairs as an `entrySet`.
2. `forEach` runs through every entry.
3. Each entry contains a key and value.

![Screen Shot 2021-07-11 at 3.07.01 PM.png](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F7e3a94ea-45a1-48de-95f5-b8516540922a?alt=media&token=a281c2b0-2f59-4e10-a9f0-97ec68b1ea0e)
- You can also run through each **`key`** as a `keySet`.

![Screen Shot 2021-07-11 at 6.09.22 PM.png](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F0814c4c8-94e9-45e1-8be0-366ea572b1ca?alt=media&token=920512af-b963-41d0-a309-a07a3af78028)


**Task:** Choose to run an `entrySet` or `keySet` through a stream pipeline. Then, choose one of the following pipelines to return the matching key:

**Pipeline 1**

![Screen Shot 2021-07-13 at 7.48.07 PM.png](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2Fa3d96e13-3b59-4317-8fd1-f068aa9444bc?alt=media&token=a98df557-1ea1-4bce-bde7-50cf8f8dc5f5)

**Pipeline 2**

![Screen Shot 2021-07-13 at 7.47.23 PM.png](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F022e5df3-b640-4326-9b5c-811381f82d4c?alt=media&token=5c9a3660-361c-4724-bcfd-5902be2a8f63)

There are four possible ways to approach this problem. **Only do one.** The solution video will cover all four implementations.

### **Hints:** 

- For `entrySet`, the stream is a sequence of **entries.**
- For `keySet`, the stream is a sequence of **keys**.
- For pipeline 2, collect should return a list with only **one element.**
- Indexing a `List` is the same as `ArrayList`.


### 4. `Test`

From `main()`, fetch the object named `"GRYFFINDOR"`. Then, print the object that it returns.


## Task 4: `gameCount`

Create a `static` variable called `gameCount` that counts up every time there's a `new Game`.

## Good Luck!
--------
##### Subscribe to our [YouTube Channel](https://www.youtube.com/@RayanSlim087?sub_confirmation=1) and Discover More Valuable Content!
