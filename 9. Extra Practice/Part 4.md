# Part 4

From the `Java Bootcamp Resources`, launch **`Part 4`**.

![Untitled.png](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2F581153fc-1e33-4583-8d32-11a5d03110e6?alt=media&token=ac60bfd2-7695-49cb-b148-0cb665197de5)

## Task 1

Inside `Main`, define `Scanner` at the class level.
```java
public class Main {

    static Scanner scan = new Scanner(System.in);

    public static void main(String[] args) {
    
    //... 

```

Close `Scanner` at the end of the `main` method.
```java
    public static void main(String[] args) {



        scan.close();
    }
```
    

## Task 2

Create a method `contactData` that returns an array of `Contac`t objects with initial data.

```java
public static Contact[] contactData() {
    return new Contact[] {
            new Contact("John Doe", "555-123-4567", "1985-01-01"),
            new Contact("Jane Smith", "555-987-6543", "1990-02-14"),
            new Contact("Alice Johnson", "555-345-6789", "1975-03-30"),
            new Contact("Bob Brown", "555-567-8910", "2000-12-25"),
            new Contact("Charlie Davis", "555-111-2222", "1983-07-04"),
            new Contact("Diana White", "555-333-4444", "1997-11-18"),
            new Contact("Ethan Green", "555-555-6666", "1988-05-22"),
            new Contact("Fiona Black", "555-777-8888", "2002-10-31")
    };
}
```

## Task 3

In the `main` method, instantiate a `ContactManager` object with an initial array of `Contact` objects.

```java
   ContactManager contactManager = new ContactManager(contactData());
```

Create a method called `displayContacts` that takes a `ContactManager` object as a parameter and displays the contacts.

```java
public static void displayContacts(ContactManager contactManager) {
    for (int i = 0; i < 8; i++) {
        Contact contact = contactManager.getContact(i);
        System.out.println(contact);
        System.out.println("\n");
    }
}
```

Printing a `Contact` object relies on the `Contact` class having a `toString` method:
```java
    public String toString() {
        return "Name: " + this.name + "\n" +
            "Phone number: " + this.phoneNumber + "\n" +
            "Birth Date: " + this.birthDate + "\n" +
            "Age: " + this.age + " year old\n";
    }
```

## Task 4

Back inside the `main` method, display the contacts:

```java
public static void main(String[] args) {
    ContactManager contactManager = new ContactManager(contactData());
    displayContacts(contactManager);
    //...
}
```
Use breakpoints to visualize the `toString` method getting invoked whenever you print an object.


## Task 5

Add the following code inside the `main` method. If the user enters continue, the code loops endlessly asking them to choose an index.
```java
public static void main(String[] args) {

    ContactManager contactManager = new ContactManager(contactData());
    displayContacts(contactManager);

    // new code...
    System.out.print("\nYou have 8 contacts. Enter 'continue' to edit them: ");
    String status = scan.nextLine();

    while (status.equals("continue")) {
        System.out.print("\nChoose an index from 0 to 7: ");
        int index = scan.nextInt();
        scan.nextLine(); // throwaway nextLine

}
```
## Task 6

Create a method `editedContact` that prompts the user for a name, phone number, and birth date, and then returns a new Contact object with the provided information.

```java
public static Contact editedContact() {
    System.out.print("\tName: ");
    // pick up name
    System.out.print("\tPhone Number: ");
    // pick up number
    System.out.print("\tBirth Date: ");
    // pick up birth date

    // return a Contact object
}
```

## Task 7

Inside `main`, update the `ContactManager` by editing the contact at the index.
```java
public static void main(String[] args) {
    //Previous code

    while (status.equals("continue")) {
        System.out.print("\nChoose an index from 0 to 7: ");
        int index = scan.nextInt();
        scan.nextLine(); // throwaway nextLine        


        // 1. Edit contact at index and update the ContactManager

}
```

## Task 8

Finalize the loop by printing the updated contacts and asking if they want to continue


```java
        System.out.println("\n\nUPDATED CONTACTS\n\n");
        displayContacts(contactManager);
        System.out.print("Enter 'continue' to make more changes: ");
        status = scan.nextLine();
}
```

## Task 9


Test the `Main` class by running the program and interacting with the user prompts to edit contacts.



----------

##### Subscribe to our [YouTube Channel](https://www.youtube.com/@RayanSlim087?sub_confirmation=1) and Discover More Valuable Content!
