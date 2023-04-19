# Part 3

From the `Java Bootcamp Resources`, launch **`Part 3`**.

![3.png](https://firebasestorage.googleapis.com/v0/b/learnthepart-75aed.appspot.com/o/images%2Fb482a4c6-07ab-4d4b-94a6-f3f2f662d3ea?alt=media&token=fdb5d33b-1e9f-412f-9353-e2a54e897162)


## Task 1
Create a new file named `ContactManager.java`. Inside the file, create the `ContactManager` class.

```java
public class ContactManager {

}
```

The `ContactManager` class will define the following field:

```java
    private Contact[] contacts; // array of Contact objects
```

## Task 2

Create a constructor for the `ContactManager` class that takes an array of `Contact` objects as a parameter.

```java
public ContactManager(Contact[] contacts) {


}
```

The constructor must initialize the `contacts` field with deep copies of the objects.


```java
public ContactManager(Contact[] contacts) {
   // 1. set field equal to a new array with the same length as the parameter
   // 2. Set each element in the field equal to a deep copy of an object in the contacts parameter
}
```

## Task 3

Create a `getContact` method that takes an index as a parameter and returns a deep copy of the `Contact` object at that index.

```java
public Contact getContact(int index) {
   // return deep copy of object at that index.
}
```

## Task 4

Create a `setContact` method that takes a `Contact` object and an index and sets the `Contact` object at the specified index to a deep copy of the given object.


```java
public void setContact(Contact contact, int index) {
    this.contacts[index] = new Contact(contact);
}
```

## Task 5

Test the `ContactManager` class by creating a few Contact objects, initializing a `ContactManager` object with those contacts, and then using the `getContact` and `setContact` methods to manipulate the contacts.

```java
public static void main(String[] args) {
    Contact contact1 = new Contact("Alice", "123-456-7890", "1990-01-01");
    Contact contact2 = new Contact("Bob", "234-567-8901", "1992-02-02");

    Contact[] contacts = {contact1, contact2};
    ContactManager contactManager = new ContactManager(contacts);

    // Test the getContact method
    Contact retrievedContact = contactManager.getContact(0);
    System.out.println(retrievedContact.getName());

    // Test the setContact method
    Contact newContact = new Contact("Charlie", "345-678-9012", "1994-03-03");
    contactManager.setContact(newContact, 0);

    // Verify that the contact was updated
    retrievedContact = contactManager.getContact(0);
    System.out.println(retrievedContact.getName());
}
```

## Task 6
Use breakpoints to visualize how the `ContactManager` class is handling the deep copying of `Contact` objects when using the `getContact` and `setContact` methods.

----------

##### Subscribe to our [YouTube Channel](https://www.youtube.com/@RayanSlim087?sub_confirmation=1) and Discover More Valuable Content!


