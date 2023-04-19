# Quidditch – Part 1
The Quidditch application will cover:

- `Stream Pipelines`
- `HashMap` **(new)**
- `hashCode()` **(new)**
- `static variables`
- `static final constants`
- `static methods`

## Setup

![8c6dce82-e2c7-4814-9652-e3a8bda38e02](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F3e8a4cf2-0581-4074-9fa6-3f107a7dd696?alt=media&token=b73d699e-ca61-4da8-ad58-37876aeb829f)

## `requirements.txt`
-----
**Objects**: `Team` and `Game`.

- **`Team`**:
     - fields: `house`, `keeper`, `seeker`, and `chasers`.
- **`Game`**:
    - fields: `scoreBoard`.
    - actions: see test cases.
    - constants: `QUAFFLE_POINTS` and `SNITCH_POINTS`.
## Task 1
----- 
Add the necessary fields to the `Team` class. Protect each field using the `private` keyword.

## Task 2
----- 
Add a constructor. The constructor parameters are `String house`, `String keeper`, `String seeker`, `String[] chasers`.

## Task 3
-----
Add a copy constructor.

## Task 4
-----
Add getters and setters.

## Task 5
-------
Add a `toString` method that returns the following:


```
   return "House: " + this.house + "\n" +
          "Keeper: " + this.keeper + "\n" +         
          "Seeker: "  + this.seeker + "\n" +         
          "Chasers: " + Arrays.toString(this.chasers) + "\n"; 
```
   
## Task 6
-----
Test your code by creating two objects of the `Team` class:


```
     new Team("GRYFFINDOR", "Oliver", "Harry", 
       new String[] {"Angelina", "Ginny", "Katie"});
 
     new Team("SLYTHERIN", "Vincent",  "Draco", 
       new String[] {"Bridget", "Harper", "Malcolm"});
```

Finally, print each object:


```
>>: House: GRYFFINDOR
>>: Keeper: Oliver
>>: Seeker: Harry
>>: Chasers: [Angelina, Ginny, Katie]

>>: House: SLYTHERIN
>>: Keeper: Vincent
>>: Seeker: Draco
>>: Chasers: [Bridget, Harper, Malcolm]
```

Your terminal should point to the folder `quidditch-game`.
![6f3e8e75-c66a-4bc8-94d1-2ba41902a5b6](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2Ff9214967-45c6-4e52-be35-49519d3c9326?alt=media&token=d9233e0b-5a98-4f71-84d8-195415fc05f2)

But, `Main.java` is inside `src/main`. I recommend just using the **run** button. Keep pressing "Proceed" until the errors go away.

![Screen Shot 2022-02-15 at 6.52.39 PM.png](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2Fa883a886-8cfa-48e9-ae4a-0bf7421eb7a3?alt=media&token=9b104409-d8de-4995-9434-67b537d9e33b)

Alternatively, if you feel like writing out the commands: 

-   **Mac users**: write `javac `**`src/main`**`/Main.java`.

-   **Windows users**: write `javac `**`src\main`**`\Main.java`.

Mac uses `/` forward-slash for paths. Windows uses backslash `\`.

## Good Luck!

--------
##### Subscribe to our [YouTube Channel](https://www.youtube.com/@RayanSlim087?sub_confirmation=1) and Discover More Valuable Content!