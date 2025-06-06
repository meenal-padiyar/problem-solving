## Java Generics
[Question Link](https://www.hackerrank.com/challenges/java-generics/problem?isFullScreen=true)
```java

import java.io.IOException;
import java.lang.reflect.Method;

class Printer <dt1>
{
   private dt1 a;
   public <dt1> void printArray(dt1[] a ){
    for(dt1 e : a){
        System.out.println(e);
    }
   }
 
}

public class Solution {


    public static void main( String args[] ) {
        Printer myPrinter = new Printer();
        Integer[] intArray = { 1, 2, 3 };
        String[] stringArray = {"Hello", "World"};
        myPrinter.printArray(intArray);
        myPrinter.printArray(stringArray);
        int count = 0;

        for (Method method : Printer.class.getDeclaredMethods()) {
            String name = method.getName();

            if(name.equals("printArray"))
                count++;
        }

        if(count > 1)System.out.println("Method overloading is not allowed!");
      
    }
}
```