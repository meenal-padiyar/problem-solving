## Java Int to String
[Question Link](https://www.hackerrank.com/challenges/java-int-to-string/problem?isFullScreen=true)
```java
import java.io.*;
import java.util.*;

public class Solution {

    public static void main(String[] args) {
        Scanner s = new Scanner(System.in);
        int a = s.nextInt();
        String str = Integer.toString(a);
        if(a.isString(str)){
            System.out.println("Good job");
        }
        else{
            System.out.println("Wrong Answer");
        }
    }
}
```