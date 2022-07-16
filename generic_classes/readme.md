# Notes
### Program to create a generic print method
``` java
class Main
{
    public static void main(String[] args)
    {
        Generic.generic_print("generic hello world ^.^");
    }
}

class Generic
{
    static <T> void generic_print(T input)
    {
        System.out.println(input.getClass().getName());
    } 
}
```

### Need for generic classes, an example:
``` java
class Generic_Array
{
    int[] a;
    
    Generic_Array(int [] array)
    {
        this.a = array;
    }
    
    void print_array()
    {
        for (int x : this.a)
            System.out.println(x);
    }
    
    void reverse_array()
    {
        int i = 0, j = this.a.length - 1;
        while(i < j)
        {
            int temp = this.a[i];
            this.a[i] = this.a[j];
            this.a[j] = temp;
            i++; 
            j--;
        }
        
        print_array();
    }
}
class Main {
    public static void main(String[] args) {
        int[] array = {1, 2, 3, 4, 5, 6};
        Generic_Array object = new Generic_Array(array);
        object.reverse_array();
        
    }
}
```


