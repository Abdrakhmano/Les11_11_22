### Task №1(8kyu)

Write function RemoveExclamationMarks which removes all exclamation marks from a given string.

[Task_link](https://www.codewars.com/kata/57a0885cbb9944e24c00008e)

#### Solution
~~~ Java
class Solution {
    static String removeExclamationMarks(String s) {
        for (int i = 0; i <= s.length() - 1; i++) {
            if (s.charAt(i) == '!') {
                s = s.replace("!","");
            }
        }
        return s;
    }
}
~~~

#### Fav Solution
~~~ Java
class Solution {
    static String removeExclamationMarks(String s) {
        return s.replaceAll("!", "");
    }
}
~~~

### Task №2(7kyu)

When provided with a String, capitalize all vowels

For example:

Input : "Hello World!"

Output : "HEllO WOrld!"

Note: Y is not a vowel in this kata.

[Task_link](https://www.codewars.com/kata/5831c204a31721e2ae000294)

#### Solution
~~~ Java
public class Solution {
    public static String swap(String st) {
        for (int i = 0; i <= st.length() - 1; i++) {
            if (st.charAt(i) == 'e' || st.charAt(i) == 'u' || st.charAt(i) == 'i' || st.charAt(i) == 'o' || st.charAt(i) == 'a') {
                st = st.replace("e", "E");
                st = st.replace("u", "U");
                st = st.replace("i", "I");
                st = st.replace("o", "O");
                st = st.replace("a", "A");
            }
        }
        return st;
    }
}
~~~

#### Fav Solution
~~~ Java
public class Kata {
    public static String swap(String st){
      return st.replace("a","A").replace("e","E").replace("i","I").replace("o","O").replace("u","U");
    }
}
~~~
