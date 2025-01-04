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
##### Your Path to Cloud-Native Engineering (After Learning Java)
###### 1. Create Enterprise Java Apps With Spring Boot → [Spring Boot Bootcamp](https://www.udemy.com/course/the-complete-spring-boot-development-bootcamp/?couponCode=SPRING_BOOTCAMP)
###### 2. Ship Code Like A Tech Giant With Docker → [Docker Bootcamp](https://www.udemy.com/course/docker-bootcamp-conquer-docker-with-real-world-projects/?couponCode=DOCKER_BOOTCAMP)
###### 3. Build Production-Grade Cloud Systems → [Kubernetes Bootcamp](https://kubernetestraining.io/)