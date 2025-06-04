## Java Loops II
[Question Link](https://www.hackerrank.com/challenges/java-loops/problem?isFullScreen=true)
```java
import java.util.*;
import java.io.*;

class Solution{
    public static void main(String []argh){
        Scanner in = new Scanner(System.in);
        int t=in.nextInt();
        int power =0;
        int store = 0 ,v;
        for(int i=0;i<t;i++){
           int a = in.nextInt();
           int b = in.nextInt();
           int n = in.nextInt();
        
        for(int j = 0; j < n ; j++){
            
             v = 0;
             power = 0;
             
            for(int k = 1; k <= j + 1  ; k++ ){
            
            store =(int) Math.pow(2 ,power );
            v += (store*b);
            power++;
            
            }
             
            System.out.print(a+v + " ");
            
        }
         System.out.println("");
        }
        
        
        in.close();
    }
}

```