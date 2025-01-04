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
##### Your Path to Cloud-Native Engineering (After Learning Java)
###### 1. Create Enterprise Java Apps With Spring Boot → [Spring Boot Bootcamp](https://www.udemy.com/course/the-complete-spring-boot-development-bootcamp/?couponCode=SPRING_BOOTCAMP)
###### 2. Ship Code Like A Tech Giant With Docker → [Docker Bootcamp](https://www.udemy.com/course/docker-bootcamp-conquer-docker-with-real-world-projects/?couponCode=DOCKER_BOOTCAMP)
###### 3. Build Production-Grade Cloud Systems → [Kubernetes Bootcamp](https://kubernetestraining.io/)