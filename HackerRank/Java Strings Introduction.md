## Java Strings Introduction
[Question Link](https://www.hackerrank.com/challenges/java-strings-introduction/problem?isFullScreen=true)
```java
import java.io.*;
import java.util.*;

public class Solution {

    public static void main(String[] args) {
        
        Scanner sc=new Scanner(System.in);
        String A=sc.next();
        String B=sc.next();
        System.out.println( A.length()+B.length());
        int compare = A.compareTo(B);
        if(compare > 0){System.out.println("Yes");}
        else{System.out.println("No");}
        String one = A.substring(0,1).toUpperCase() + A.substring(1);
        String two = B.substring(0,1).toUpperCase() + B.substring(1);
        System.out.println(one + " " + two);
    }
}
```