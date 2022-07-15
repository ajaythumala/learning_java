# Notes:
### Program to print hello world :)
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
System.out.println("Hello" + "World");
```
- '+' operator will concatenate the strings

``` java
System.out.println();
System.out.print();
```
- println() will print with a new line character at the end and print() will not

### Program to initialize an array, traverse it and compute the average of its integer elements
``` java
class Array
{
  public static void main(String[] args)
  {
    int array[] = {1, 2, 3, 4, 5};
    
    // traversing an array
    for(int i = 0; i < array.length; i++)
        System.out.print(array[i] + " ");
    
    // calculating average
    float sum = 0;
    for(int i = 0; i < array.length; i++)
        sum += array[i];
        
    System.out.println("");
    System.out.print("average = " + sum / array.length);
  }
}
```
### Program to create and initialize a 3D array
``` java
class ThreeDArray
{
  public static void main(String[] args)
  {
    int array [][][] = new int [3][4][5];
    int sum = 0;
    for(int i = 0; i < 3; i++)
    {
        for(int j = 0; j < 4; j++)
        {
            for(int k = 0; k < 5; k++)
            {
                array[i][j][k] = sum;
                sum += 1;
                System.out.print(array[i][j][k] + " ");
            }
            System.out.println("");
        }
        System.out.println("");
    }
  }
}
```
