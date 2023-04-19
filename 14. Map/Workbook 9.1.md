# Workbook 9.1

From the `Java Bootcamp Resources`, launch **`starter`**.

![starter.png](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F87bced44-2cd9-4db0-9a76-22125c478254?alt=media&token=7dc717de-b9d3-40c6-9ec2-32908aa28976)

## Task 1

The `Team` class contains two fields.

```java
    private String name;
    private Map<String, String> players;
```
Fill in the logic for the constructor.
```java
    public Team(String name) {
        // set the name.
        // set players equal to a new HashMap.
    }
```
## Task 2

Fill in the logic for the getters and setters

```java
    public String getName() {
        // return the name
    }

    public void setName(String name) {
        // set the name

    }

    public String getPlayer(String position) {
       // return a player from the HashMap.
    }

    public void setPlayer(String position, String player) {
        // Add a <String, String> entry into the HashMap
    }

```

## Task 3

The `Game` class contains two fields. 

```java
    private String arena;
    private LocalDate date;
```
The `LocalDate` class provides the **[`now()`](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/time/LocalDate.html#now())** method.

```java
public class LocalDate {
    
    public static LocalDate now() {
        return now(Clock.systemDefaultZone());
    }

}
```
The `static` keyword allows you to call the method from the class itself.

```java
LocalDate.now()
```

Use this information to fill the logic in the `Game` constructor. 

```java
    public Game(String arena) {
        // set the arena.
        // set the date equal to the current date.
    }
```

## Task 4

The `LocalDate` class provides the following methods.

```java
public class LocalDate {
    
    public int getYear() {
        return year;
    }

    public int getMonthValue() {
        return month;
    }

    public int getDayOfMonth() {
        return day;
    }

}
```
You can invoke these methods from any object of the `LocalDate` class.

```java
date.getDayOfMonth();
date.getMonthValue();
date.getYear();
```

Use this information to fill the first line inside `begin()`.
```java
"\n - This matchup takes place at the " + this.arena + " arena on " + "<day/month/year>" + ".";
```
Execute your code.
```
>>: - This matchup takes place at the Etihad Stadium arena on 04/01/2023.
>>: ...
>>: ...

```

## Task 5

Task 4 familiarized you with `LocalDate` getters. In this case, favor calling `format`.

```java
String formattedDate = this.date.format(DateTimeFormatter.ofPattern("dd/MM/yyyy"));
```
Execute your code.
```
>>: - This matchup takes place at the Etihad Stadium arena on 04/01/2023.
>>: ...
>>: ...

```


## Task 6

Consider that `main()` already populates two teams with players. 
```java
        Team bulls = new Team("Chicago Bulls");
        bulls.setPlayer("SHOOTING_GUARD", "Michael Jordan");
        bulls.setPlayer("SMALL_FORWARD", "Scottie Pippen");
        bulls.setPlayer("POWER_FORWARD", "Dennis Rodman");
        bulls.setPlayer("CENTER", "Bill Wennington");
        bulls.setPlayer("POINT_GUARD", "Randy Brown");

        Team pistons = new Team("Detroit Pistons");
        pistons.setPlayer("SHOOTING_GUARD", "Joe Dumars");
        pistons.setPlayer("SMALL_FORWARD", "Grant Hill");
        pistons.setPlayer("POWER_FORWARD", "Otis Thorpe");
        pistons.setPlayer("CENTER", "William Bedford");
        pistons.setPlayer("POINT_GUARD", "Isiah Thomas");
```

Use this information to fill the remaining lines inside `begin()`.

----------
##### Subscribe to our [YouTube Channel](https://www.youtube.com/@RayanSlim087?sub_confirmation=1) and Discover More Valuable Content!