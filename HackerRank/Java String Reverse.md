## Java String Reverse
[Question Link](https://www.hackerrank.com/challenges/java-string-reverse/problem?isFullScreen=true)
```java
import java.io.*;
import java.util.*;

public class Solution {

    public static void main(String[] args) {
        
        Scanner sc=new Scanner(System.in);
        String A=sc.next();
        char []arr = A.toCharArray();
        int e = 0 , flag = 0;
        int f = A.length()-1;
        while(e < f){
            if(arr[e] == arr[f]){
                flag = 1;
            }
            else if(arr[e] != arr[f]){
                flag =0;
            }
            e++;
            f--;
        }
        if( flag == 1 || e == f){
            System.out.println("Yes");
        }
        else if (flag == 0){
            System.out.println("No");
        }
    
        
    }
}
```