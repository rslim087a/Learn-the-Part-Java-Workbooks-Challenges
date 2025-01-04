# `print` vs. `println`

Before you continue, you need to understand the difference between `print` and `println`.

 - `println()` prints text and moves to a new line.

```java
System.out.﻿println﻿(﻿" a "﻿)﻿;
System.out.﻿println﻿(﻿" b "﻿)﻿;
System.out.﻿println﻿(﻿" c "﻿)﻿;
```

`>> a`

`>> b`

`>> c`

- `print` prints text but it does not move to a new line. So, ensuing print calls print on the same line.

```java
System.out.﻿print﻿(﻿" a "﻿)﻿;
System.out.﻿print﻿(﻿" b "﻿)﻿;
System.out.﻿print﻿(﻿" c "﻿)﻿;
```

`>> a b c`

You can proceed to Workbook 5.3.

## See you there!
----------
##### Your Path to Cloud-Native Engineering (After Learning Java)
###### 1. Create Enterprise Java Apps With Spring Boot → [Spring Boot Bootcamp](https://www.udemy.com/course/the-complete-spring-boot-development-bootcamp/?couponCode=SPRING_BOOTCAMP)
###### 2. Ship Code Like A Tech Giant With Docker → [Docker Bootcamp](https://www.udemy.com/course/docker-bootcamp-conquer-docker-with-real-world-projects/?couponCode=DOCKER_BOOTCAMP)
###### 3. Build Production-Grade Cloud Systems → [Kubernetes Bootcamp](https://kubernetestraining.io/)
