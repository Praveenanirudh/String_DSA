# Check if a String is Subsequence of Other

Given two strings A and B, find if A is a subsequence of B. A subsequence is a sequence that can be derived from another sequence by deleting some elements without changing the order of the remaining elements.


 ```java
import java.util.*;

class DSA {
    static boolean isSubsequence(String s1, String s2) {
        int j = 0;

        for (int i = 0; i < s1.length() && j < s2.length(); i++) {
            if (s1.charAt(i) == s2.charAt(j)) {
                j++;
            }
        }
        return (j == s2.length());

    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        String s1, s2;

        s1 = sc.next();
        s2 = sc.next();

        System.out.println(isSubsequence(s1, s2));

    }

}
```
