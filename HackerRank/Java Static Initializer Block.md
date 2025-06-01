## Java Static Initializer Block
[Question Link](https://www.hackerrank.com/challenges/java-static-initializer-block/problem?isFullScreen=true)
```java
import java.io.*;
import java.util.*;
import java.text.*;
import java.math.*;
import java.util.regex.*;

public class Solution {
    Scanner s = new Scanner(System.in);
    static int B = .nextInt();
    static int H = s.nextInt();
    static{
        Scanner s = new Scanner(System.in);
        int B = s.nextInt();
        int H = s.nextInt();
        if(  B <=0 || H <= 0){
            System.out.println("java.lang.Exception: Breadth and height must be positive");
        }
    }

public static void main(String[] args){
		if(flag){
			int area=B*H;
			System.out.print(area);
		}
		
	}

}
```