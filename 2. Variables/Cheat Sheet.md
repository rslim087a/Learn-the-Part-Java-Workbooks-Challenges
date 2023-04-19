# Cheat Sheet

This cheat sheet contains important takeaways that lead up to section two.

## **1\. Getting Started**

-   `class`: contains all of your code.

-   `main()`: entry point of your app.

-   `javac <file-name>.java`: compiles your code.

-   `java <file-name>`: runs the compiled code.

## **2\. Variables**

**Data types**

There are 6 main data types (we didn't cover `boolean` yet).

![](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F3d09e5e0-aeb9-43f0-83c2-fc2ba5ed2240?alt=media&token=44e844e4-103f-4450-a9d5-fc4cc8a53115)

`long` can store very big numbers. But, `int` is faster and takes less memory.

![](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F1b8ba9d5-fe44-43a0-9cab-8a22ead4b1c3?alt=media&token=56913d7b-7da1-44d5-b556-6f1608b50caa)

**Operators**

![](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F458bd2ef-637d-41e2-939f-cdb337a639ba?alt=media&token=e69232c6-f840-4a58-83c6-96acd6436aab)

**Scanner**

`nextLine()`: scans for a `String` value.

`nextDouble()`: scans for a `double` value.

`nextLong()`: scans for a `long` value.

`nextInt()`: scans for an `int` value.

## Coding Pitfalls

### Pitfall
---
Put math operations in brackets if you wish to embed them inside a `String`.

-   Example: `"5 + 2 is " + (5 + 2);`

### Pitfall
----
|`nextLine()` Trap | |
| --- | --- |
| Pitfall  | `nextLine()` gets skipped when placed after `nextInt()` , `nextDouble()`, or `nextLong()`. 
| Solution  |Add a throwaway `nextLine()` before the "real" `nextLine()`.



## Good coding habits

-   class: `CamelCase`.

-   variable: `lowerCamelCase`.

## Tips and tricks

**Terminal**

-   Use the **up** key to run previous terminal commands.

-   Write `clear` to clear the terminal output.

-   Press the `tab` key for auto-complete.

**Escape characters**

-   `\n` adds a new line of space.

-   `\t` adds a new tab of space.

**Shortcut keys**

-   Use `CMD/Ctrl`+`/` to comment a highlighted piece of code.

------
##### Subscribe to our [YouTube Channel](https://www.youtube.com/@RayanSlim087?sub_confirmation=1) and Discover More Valuable Content!