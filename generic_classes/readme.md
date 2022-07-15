# Notes
### Program to create a generic print function
``` java
class Main
{
    public static void main(String[] args)
    {
        Generic object = new Generic();
        object.generic_print("generic hello world ^.^");
    }
}

class Generic
{
    <T> void generic_print(T input)
    {
        System.out.println(input);
    } 
}
```
