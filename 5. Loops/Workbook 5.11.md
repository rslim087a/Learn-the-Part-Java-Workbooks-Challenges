# Workbook 5.11

From the `Java Bootcamp Resources`, launch **`Workbook 5.11`**.

![11.png](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F7fdaa8e4-9c26-47be-88aa-e7de6c039712?alt=media&token=602c928a-94a4-48fd-81a1-b8ff83c504d3)

Task 1
------

Print the rules to the user:

`>> Let's play Rolling Java. Type anything to start.`

**`scan.nextLine`**

`>> Great, here are the rules:\n`

`>> - If you roll a 6, the game stops.`

`>> - If you roll a 4, nothing happens.`

`>> - Otherwise, you get 1 point.\n`

`>> You must collect at least 3 points to win. Enter anything to roll:`

**`scan.nextLine`**


Task 2
------

Make a `while` loop that runs forever.

Place your second `scan.nextLine()` from **Task 1** as the first line in your loop. Print `hey` in your loop's second line.

![](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F293c1686-3f2f-48c3-b35b-c38ecccf004d?alt=media&token=8130ee77-4478-435a-8bb6-5425760e1a74)

After testing your code, remove the `hey` print.

Task 3
------

Define the `rollDice` function.

```java
/**
 * Function name: rollDice
 * @return randomNumber (int)
 *
 * Inside the function:
 *  - return a random number between one and six. 
 */
```

Task 4
------

During each run, call `rollDice()` and store the value in `diceRoll`. Print each dice roll: `You rolled a <diceRoll>.`.

![](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2Fda2d821f-3e00-41f8-b6f2-7ef4f804a88a?alt=media&token=8ef6c1fd-d325-4cfb-93ee-9953aa2d8e84)

Task 5
------

Whenever the user rolls a **6**:
   -   print: `End of game.`
   -   stop the game.

Whenever the user rolls a 4:
  -   print: `Zero points. Keep rolling.`

When the user rolls anything else:
  -   update the `score` variable by 1

  -   print: `One point. Keep rolling`.

![](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F2dac03b7-ff67-4738-82d0-296d4f4905aa?alt=media&token=db4cda64-8f17-439e-b481-67c67ffb716b)

Task 6
------

After the game ends, check the user's points. If the score is greater than or equal to 3, print:

  - `Wow, that's lucky. You win!`

Otherwise, print:

  - `Tough luck, you lose :(`

**Winning scenario:**
![](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2Fe9d90fd7-fda0-4db2-bd6b-73dbd47dc93d?alt=media&token=3a06d786-812d-4508-a393-4f81391ce7aa)

**Losing scenario:**

![](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2Fb70e60ca-3bb9-401f-b967-8d3667a4bfc5?alt=media&token=d8250c00-4eac-4514-96e8-4853a1cf101f)

## Visualizing the Runtime

After you solve this workbook, I still recommend watching the video solution on Udemy.

![11.png](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F86c491f7-f3a8-4de1-a65d-b8c288d9b8ce?alt=media&token=640bc09c-f531-4fa3-a91c-cf5dc8abc19c)

It will show you how to visualize the runtime using Visual Studio Code.

----------
##### Subscribe to our [YouTube Channel](https://www.youtube.com/@RayanSlim087?sub_confirmation=1) and Discover More Valuable Content!