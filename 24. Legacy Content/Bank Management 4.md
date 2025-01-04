# Bank Management - Part 4
----

> **Interface**: a contract of behavior.

A class that implements an interface must override all of its methods.
## Task 1
------
Based on the requirements, `Chequing` implements a `Taxable` interface. Add a `void tax(double income)` method inside `Taxable` and override it inside `Chequing`.

## Task 2
------
Create a unit test named `incomeTax()`.
- deposit `$4,000` into the chequing account.
- call `tax()` for an income of `$4,000`.
- assert the resulting balance is `5374.51`.

You can find the taxable income and tax rate inside `requirements.txt`. 

## Good Luck!
--------
##### Your Path to Cloud-Native Engineering (After Learning Java)
###### 1. Create Enterprise Java Apps With Spring Boot → [Spring Boot Bootcamp](https://www.udemy.com/course/the-complete-spring-boot-development-bootcamp/?couponCode=SPRING_BOOTCAMP)
###### 2. Ship Code Like A Tech Giant With Docker → [Docker Bootcamp](https://www.udemy.com/course/docker-bootcamp-conquer-docker-with-real-world-projects/?couponCode=DOCKER_BOOTCAMP)
###### 3. Build Production-Grade Cloud Systems → [Kubernetes Bootcamp](https://kubernetestraining.io/)