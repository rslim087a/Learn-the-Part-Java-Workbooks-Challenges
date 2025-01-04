# Global Superstore 3

**Prerequisite:** You wrote the solution for Part 2.


## Task 1
-----
Remove this line of code:

     System.out.println("Access Denied. We apologize for the inconvenience. Have a good day " + name + ".");

After the user enters their information, the `main` thread must wait for the worker threads to die. Then, you can present the user with sales data:
```java
    System.out.println("\nThank you " + <name> + ". The average sales for Global Superstore are:\n");
    System.out.println("Average Furniture Sales: " + <furniture sales>);
    System.out.println("Average Technology Sales: " + <tech sales>);
    System.out.println("Average Office Supplies Sales: " + <office sales>);
    System.out.println("Total Average: " + <total>);
```

Your output should appear as follows:


```
>>: Please enter your name to access the Global Superstore dataset: Rayan

>>: Thank you Rayan. The average sales for Global Superstore are:

>>: Average Furniture Sales: 9799.21280813723
>>: Average Technology Sales: 9854.096986549781
>>: Average Office Supplies Sales: 9540.319577001303
>>: Total Average: 9651.778039610392
```
## Good Luck!
--------
##### Your Path to Cloud-Native Engineering (After Learning Java)
###### 1. Create Enterprise Java Apps With Spring Boot → [Spring Boot Bootcamp](https://www.udemy.com/course/the-complete-spring-boot-development-bootcamp/?couponCode=SPRING_BOOTCAMP)
###### 2. Ship Code Like A Tech Giant With Docker → [Docker Bootcamp](https://www.udemy.com/course/docker-bootcamp-conquer-docker-with-real-world-projects/?couponCode=DOCKER_BOOTCAMP)
###### 3. Build Production-Grade Cloud Systems → [Kubernetes Bootcamp](https://kubernetestraining.io/)