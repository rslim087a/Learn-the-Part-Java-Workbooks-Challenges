# **Cheat Sheet**

This cheat sheet contains the most important takeaways that lead up to section seven.

**Definitions**
---------------

-   **Class**: blueprint from which you can create objects.

-   **Object**: an object is a *thing* that you can see or describe.

-   **Field**: class variable that describes an object.

-   **Action**: method (function) that represents what the object can do.

-   **Constructor**: runs when you create a `new` object.

    -   Purpose: update every field of the newly created object.

-   **`this`**: refers to the current object that's calling the constructor or method.

    -   Purpose: useful when fields and parameters have conflicting names.

-   **Copy Constructor**: runs when you create an object.

    -   Purpose: copy every value from a `source` object into a `new` object.

-   **Getter**: method (function) that returns a copy of a `private` field's value.

-   **Setter**: method (function) that updates the value of a `private` field.

-   **`toString`**: method that returns a `String` representation of every field in an object.

    -   Purpose: When you print an object, Java internally calls the `toString` method.

`public` **vs.** `private`
----------------------------------

-   `public`: provides public access to a field or method from anywhere.

    -   Constructors and methods tend to be `public`.

-   `private`: prevents direct access of a field or method outside of its class.

    -   To protect the state of an object, fields tend to be `private`.

**The Big Three**
-----------------

If a `class` has fields, you need to add:

1.  **Constructor** -- to update the fields of a `new` object.

2.  **Getters** -- to get the value of a `private` field.

3.  **Setters** -- to set the value of a `private` field.

**Reference Traps**
-------------------

> The state of a variable should not change because you updated another.

![](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2Ff7f41501-9295-49c1-bba4-6dd81ece1ca7?alt=media&token=9ba5af9b-5caa-4afa-8ff2-f0eff7fd39cf)
-------
##### Subscribe to our [YouTube Channel](https://www.youtube.com/@RayanSlim087?sub_confirmation=1) and Discover More Valuable Content!