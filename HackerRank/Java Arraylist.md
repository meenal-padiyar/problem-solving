## Java Arraylist
[Question Link](https://www.hackerrank.com/challenges/java-arraylist/problem?isFullScreen=true)
```java
import java.io.*;
import java.util.*;
import java.text.*;
import java.math.*;
import java.util.regex.*;

public class Solution {

    public static void main(String[] args) {
        Scanner s = new Scanner(System.in);
        int n = s.nextInt();
        List<List<Integer>> L = new ArrayList<>();

        for(int i = 0; i < n ; i++){
        int d = s.nextInt();
        ArrayList <Integer> row = new ArrayList<>(d);

        for(int j = 0 ; j < d ; j++){
            int v = s.nextInt();
            row.add(v);
        }

        L.add(row);

      }
        int q = s.nextInt();
        for(int i = 0; i < q ; i++){
        int x = s.nextInt()-1;
        int y = s.nextInt()-1;

        if(x < L.size() && y < (L.get(x).size())){
            System.out.println(L.get(x).get(y));
        }

        else{
            System.out.println("ERROR!");
        }

        }
    }
    
}
```