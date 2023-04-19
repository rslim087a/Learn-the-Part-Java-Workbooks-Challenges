# Workbook 3.7

From the `Java Bootcamp Resources`, launch the **`Workbook 3.7`** folder.

![Screen Shot 2022-10-16 at 7.13.08 PM.png](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F068d35b4-92c6-4d60-89d8-361110d5e737?alt=media&token=7726086e-dc1c-4e77-a7d7-8a6120bc5802)

## The Royal Bank of Java
----------------------

In this workbook, you work for the Royal Bank of Java. Your job is to approve customers for a loan if they:

-   Have **at least** $10,000 in their savings account.

-   Have **less than** $5,000 in credit card debt.

-   Have worked for **more than** 2 years.

The user will also need to provide their name.

Your task is to scan for values and use `if-else` to control how these statements print.

```java
public class Bank {
    public static void main﻿(﻿String[] args﻿) {
        Scanner scan = new Scanner﻿(System.in)﻿;
        System.out.﻿println﻿(﻿"\n****ROYAL BANK OF JAVA****"﻿)﻿;
        System.out.﻿println﻿(﻿"Are you here to get a mortgage? (yes or no)"﻿)﻿;
        System.out.﻿println﻿(﻿"\nGreat! In one line" +
                 "\nHow much money do you have in your savings?" +
                 "\nAnd, how much do you owe in credit card debt?"﻿)﻿;
        System.out.﻿println﻿(﻿"\nHow many years have you worked for?"﻿)﻿;
        System.out.﻿println﻿(﻿"What is your name?"﻿)﻿;
        System.out.﻿println﻿(﻿"Congratulations <name>, you have been approved!"﻿)﻿;
        System.out.﻿println﻿(﻿"Sorry, you are not eligible for a mortgage"﻿)﻿;
        System.out.﻿println﻿(﻿"\nOK. Have a nice day!"﻿)﻿;
        scan.﻿close﻿(﻿)﻿;
    }
}
```

## Task 1 - Pick up the user's decision

The code starts by asking the user if they're here to get a mortgage. Use `Scanner` to pick up their decision.

```java
        System.out.﻿println﻿(﻿"\n****ROYAL BANK OF JAVA****"﻿)﻿;
        System.out.﻿println﻿(﻿"Are you here to get a mortgage? (yes or no)"﻿)﻿;
        //Task 1 - ﻿Pick up﻿ ﻿the user's decision.

```

## Task 2 - `if - else`

If the decision is `'yes'`, ask the user about their savings and debt. If the decision is anything other than 'yes', print: `'OK. Have a nice day!'`.

```
   //Task 2
 -- Print this if the decision is "yes"
         System.out.println("\nGreat! In one line" +
            "\nHo﻿w much ﻿m﻿oney do you have in your savings?" +
            "\nAnd, how much do you owe in credit card debt?");

 -- Print this if the decision is not "yes"
          System.out.println("\nOK. Have a nice day!");

```

Output for `yes`:

![](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2Fc71c5d90-f601-4f0f-b95d-05200150868d?alt=media&token=d97ff4a2-53f4-41c4-9632-4fb8c22ac188)

Output for `else`:

![](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2Feb74f53a-1cfa-4fba-bbe4-b596f106cf11?alt=media&token=42b982f8-17e6-4d9b-a51e-58176160cab6)

## Task 3 - Pick up the savings and debt values
--------------------------------------------

Pick up and store the savings and debt values.

```java
        System.out.﻿println﻿(﻿"\nGreat! In one line" +
            "\nHow much money do you have in your savings?" +
            "\nAnd, how much do you owe in credit card debt?"﻿)﻿;
        // Task 3 - Pick up each value
```

![](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2Fc2eed793-3b7a-47fa-814d-401047e51304?alt=media&token=233e908c-c9ad-478f-b557-0dd53550cf19)

## Task 4 - Pick up the number of years

![](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2Fdecee013-3dca-4810-a05a-1effa5cd8d1c?alt=media&token=8a7c2e71-76a9-4688-bcd4-d638261e01b7)

## Task 5 - Pick up the user's name
Careful not to fall into the `nextLine()` trap.

![](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F4efa897d-1105-4c71-8546-f965e7cb05f2?alt=media&token=619ed064-e39a-45bc-a40e-dda8bd7c4e21)


## Task 6 - Logical Operator
-------------------------

Use a logical operator to check if the user has

-   **at least** $10,000 in their savings account.

-   **less than** $5,000 in credit card debt.

-   **more than** 2 years of work experience.

If they meet the requirements, print:

> `Congratulations <name>, you have been approved!`

Otherwise, print:

> `Sorry, you are not eligible for a mortgage.`

Finally, use these values:

-   `savings: 20000`

-   `debt: 1500`

-   `years: 7`

**Final Ouput:**
![](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2Ff2495206-fc97-47cb-a1b9-4f712efeab55?alt=media&token=c1e47b3a-dbcb-4851-8d3e-ec4b3fae4fc8)

## Visualizing the Runtime

After you solve this workbook, I still recommend watching the video solution on Udemy.

![Screen Shot 2022-10-17 at 3.00.31 PM.png](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F48408342-8c58-405c-bc67-ebf9f3896bf4?alt=media&token=8aee36f7-169c-4ad1-819e-74301d190d5f)

It will show you how to visualize the runtime using Visual Studio Code.

----------
##### Subscribe to our [YouTube Channel](https://www.youtube.com/@RayanSlim087?sub_confirmation=1) and Discover More Valuable Content!