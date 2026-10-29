# Starting out

* Java is case sensitive
* To run a program we need an entry point, a method called main in `public static void main(String[] args)`
* Printing requires explicit print statement 

```java
// WelcomeToJava is a Java class
class WelcomeToJava{

    // The main method is the kickoff point for Java applications
    public static void main(String[] args) {

        // Println statements output results to the screen shown below
        System.out.println("Hello Java!");
    }
}
```

* Every java program is inside a class
* A Class is a container of related code
* A Method is within a class
* Every line iside the method ends with `;`

## Starting with variables
* Variables store values
* Every variable has a type, a name, and a value
* `=` is an asignment operator 
* Variable names must start with a letter and cannot contain spaces, ecommended case is camel case.

```java
String variableName = "text in double quotation marks";

int age = 29;
```

## Primitive number types

Primites are core data types from which all other data is constructed:
* `int`: used most often for whole numbers (up to two million)
    * Other types:
    * `long`: used for very large numbers (up to quintillion)
    --> Need to add `L/l` at the end of the number that we are assigning to the variable
    * `short`: used for smaller numbers (up to 30 thousand)
    * `byte` : used for very small numbers (-127 to 128)
* `double`: used most often for decimal numbers (up to 16 decimal digits)
    * Other types:
    *  `float`: used for smaller numbers, less precise (up to 7 decimal digits) --> Need to add `F/f` at the end of the number that we are assigning to the variable 
* `boolean`: `true`or `false`. Variable names usually start with is e.g. `isOnSale`

* `char`: stores one character. Use a single quote (vs. strings that use double quotes) Example: `J` 

* `String`: is not a primitive datatype and it is a coolection of characters, so we uses double quotes

