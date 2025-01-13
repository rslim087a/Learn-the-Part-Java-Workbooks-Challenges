# Workbook 11.1

From the `Java Bootcamp Resources`, launch **`starter`**.

![starter.png](https://img-c.udemycdn.com/redactor/raw/article_lecture/2025-01-03_19-03-59-e94444e749037b861a66df16f719c842.png)


## Task 1

Use the position values inside `main()` to fill up the `Position` `enum` with constants. 

```java
public enum Position {

    
}
```

## Task 2

Update the `players` field inside `Team` to store `Position` keys rather than `String`.

```java
    private Map<String, String> players;
```

## Task 3

Update `getPlayer()` to receive a `Position` enum constant rather than a `String`.
```java
    public String getPlayer(String position) <----
``` 

## Task 4
Update `setPlayer()` to receive a `Position` enum constant rather than a `String`.
```java
public void setPlayer(String position, String player)
```
The enum type is guaranteed to be one of five constants. So remove the safety mechanisms.

```java
if (!position.equals("SHOOTING_GUARD") || !position.equals("SMALL_FORWARD") || !position.equals("POWER_FORWARD") ...
    throw new IllegalArgumentException("INVALID POSITION");
```
Although you should still ensure that a `null` doesn't get passed in.
```java
        if (position == null)
            throw new IllegalArgumentException("Position cannot be null");
```

## Task 5
enum constants are implicitly `static` and `final`. Import every constant into `Main` and fill in the `main()` method.

## Task 6

Import every constant into `Game` and fill in the `begin()` method.

----------

##### **Go From Zero to DevOps Master**: *[Java → Spring Boot → Docker → Kubernetes](https://rslim087a.github.io/zero-devops-roadmap/)*