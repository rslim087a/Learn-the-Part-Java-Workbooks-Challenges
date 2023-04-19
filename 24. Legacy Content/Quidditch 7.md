# Quidditch – Part 7
**Goal**: Glue everything together inside `Main.java`.  
## Task 1

Create two constants:
```java
static final String TEAMS_FILE = "RELATIVE PATH";
static final String PLAYS_FILE = "RELATIVE PATH";
```
Right-click on each file and copy its relative path. Your relative path should be `src/main/file.txt`.

## Task 2

Create a function that retrieves the data from `TEAMS_FILE`
```java
    /**
     * Function name: getData
     * @return (String[][])
     * @throws FileNotFoundException
     * 
     * Inside the function:
     *   1. Returns data from TEAMS_FILE as a String[][] array.
     */
```
## Task 3

Inside `main()`, create a `Game` object from the data you extracted in Task 2.
```java
new Game(
  new Team(data[0][0], data[0][1], data[0][2], new String[] {data[0][3], data[0][4], data[0][5]}),
  new Team(data[1][0], data[1][1], data[1][2], new String[] {data[1][3], data[1][4], data[1][5]})
);
```
## Task 4
Create a function that starts the game of Quidditch.
```
  /** Function name: startGame
   * 
   * Inside the function:
   *    1. Grabs each play from plays.txt and call game.simulate(play);
   *    2. Prints the result from game.simulate(play): println("\n" + <result> + "\n");
   */
```
Call the function from `main()`:
```
>>: Harper starts with the quaffle, speeds off towards the goal posts, and scores! 10 points!

>>: Malcolm gains the pass, belts up the field and scores, 10 points!

>>: Harper gets the next pass, flies like an eagle. Nice dive around the goalposts, and scores! 10 points.

>>: Oliver sees the quaffle racing towards the post. But, they're quick to it. Great save!

>>: Harper gains the pass, dives into the goalposts, and scores! 10 points!

>>: Harry sees the snitch, dives downwards, and catches the snitch! 150 POINTS!!!
```
## Task 5
Create a function that prints the final result:
```
/** Function name: printResult()
 * 
 * Inside the function:
 *    1. Prints the final score: println("\nGRYFFINDOR: " + <gryffindor score> + " SLYTHERIN: " + <slytherin score>);
 *    2. Prints the winner: println("\n" + <winner team name> + " WINS!");
 *  
 */
```
Call the function from `main()`:

```
>>: Harper starts with the quaffle, speeds off towards the goal posts, and scores! 10 points!

>>: Malcolm gains the pass, belts up the field and scores, 10 points!

>>: Harper gets the next pass, flies like an eagle. Nice dive around the goalposts, and scores! 10 points.

>>: Oliver sees the quaffle racing towards the post. But, they're quick to it. Great save!

>>: Harper gains the pass, dives into the goalposts, and scores! 10 points!

>>: Harry sees the snitch, dives downwards, and catches the snitch! 150 POINTS!!!

GRYFFINDOR: 150 SLYTHERIN: 40

GRYFFINDOR WINS!
```

## Task 6

Create a function that makes the code "sleep" for X seconds.
```
    /**
     * Function name: wait
     * @param sec
     * 
     * Inside the function:
     *  1. Make the code sleep for X seconds.
     */
```
**Hint**: look into `TimeUnit`.

## Task 7

Call `wait(3)` before printing each play.

**Final output**

![Untitled.gif](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F521c19cb-3e2f-4bdb-95bc-b591ac46a51e?alt=media&token=dbf7ae7a-362c-4125-8f9c-5eb1790f532f)


--------
##### Subscribe to our [YouTube Channel](https://www.youtube.com/@RayanSlim087?sub_confirmation=1) and Discover More Valuable Content!