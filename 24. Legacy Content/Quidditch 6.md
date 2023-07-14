# Quidditch – Part 6

**Goal**: Quality control the `Game` class.

Unchecked exceptions
--------------------

An **unchecked** exception crashes the app as a result of badly written code.

You should throw an:

-   `IllegalArgumentException` when the caller passes faulty arguments into a method/constructor.

-   `IllegalStateException` when an object calls its method at a "bad time" (object not in a legal state).

Throwing an unchecked exception forces the caller to improve their code.

## **Task 1 – Inspecting the** `Game` **class**
------------------------------------------------
- `setScore` is vulnerable to receiving `null` objects and adding them as keys. Throw an `IllegalArgumentException` to prevent that.

- All other methods/constructors will respond appropriately when presented with illegal arguments.


--------
##### Become a Java Web Developer with our [Spring Boot Course](https://udemy-redirect-app.herokuapp.com/spring) (86% Sale).