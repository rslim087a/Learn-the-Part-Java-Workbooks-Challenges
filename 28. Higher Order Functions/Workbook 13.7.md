# Workbook 13.7

From the `Java Bootcamp Resources`, launch **starter**.

![starter.png](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F87bced44-2cd9-4db0-9a76-22125c478254?alt=media&token=7dc717de-b9d3-40c6-9ec2-32908aa28976)

## Task 1

Use `Files.lines(path)` to create a stream of `String` elements from the data source.

## Task 2

Process the stream in a pipeline of operations:

**1. `filter`**: uses the method [**`startsWith`**](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html#startsWith(java.lang.String)) to remove `Spam` emails.

**2. `forEach()`**: prints every element in the stream.

```
>>: Primary: Just checking in, how was your weekend?
>>: Social: You have been invited to join the DEF group!
>>: Social: You have been invited to join the ABC network!
>>: Social: You have been added to the ABC group!
>>: Primary: I hope you're doing well!
>>: Primary: Just wanted to catch up, how have you been?
>>: Primary: Hi, how are you doing?
>>: Promotions: 20% off all shoes!
>>: Promotions: Get a free gift with your next purchase!
>>: Social: You have been invited to join the XYZ network!
>>: Social: You have a new follower on XYZ!
>>: Primary: How has your week been going?
>>: Promotions: 50% off your first purchase!
>>: Promotions: 10% off your next vacation!
>>: Promotions: New clearance sale at XYZ store!
```

--------
##### Your Path to Cloud-Native Engineering (After Learning Java)
###### 1. Create Enterprise Java Apps With Spring Boot → [Spring Boot Bootcamp](https://www.udemy.com/course/the-complete-spring-boot-development-bootcamp/?couponCode=SPRING_BOOTCAMP)
###### 2. Ship Code Like A Tech Giant With Docker → [Docker Bootcamp](https://www.udemy.com/course/docker-bootcamp-conquer-docker-with-real-world-projects/?couponCode=DOCKER_BOOTCAMP)
###### 3. Build Production-Grade Cloud Systems → [Kubernetes Bootcamp](https://kubernetestraining.io/)