# Notes:
``` java
class HelloWorld
{
  public static void main(String[] args)
  {
    System.out.println("Hello World :)");
  }
}
```

1. S in String[args] and System.out.println is uppercase
1. "public static void main(String[] args)"
    - The public keyword is an access specifier - Hence, the method can be directly accessed outside the class
    - The static keyword indicates that the method is called using the class name, not using an instance of the class
    - The void keyword indicates that the method does not return anything
    - String[] args is string array arguments - the command line input is passed in here when the method is called

``` java
System.out.println("Hello" + "World")
```
'+' operator will concatenate the strings
