# Global Superstore 7

**Prerequisite**: You wrote the solution for part 6.

## Task 1
----- 
Locks can make your code hard to read. Use atomic variables to enforce thread safety. Your final output should remain:

`>>: The sample size is: 1522889`

`>>: The quantity sold is: 8818065`

### Final Remarks:
When possible, favor `Atomic` types over locks. When several threads are updating a variable, `Atomic` ensures the updates are synchronized.

## Good Luck!
--------
##### Become a Java Web Developer with our [Spring Boot Course](https://udemy-redirect-app.herokuapp.com/spring) (86% Sale).