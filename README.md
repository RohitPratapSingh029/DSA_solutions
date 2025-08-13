# DSA_solutions

### Question 1
```
Integer x, y, z
Set x = 5, y = 3
if x > y then
    if y > 0 then
        z = x / y
    else
        z = x * y
    end if
else
    z = 0
end if
Print z
```
**Options:**
- a) 0
- b) 1
- c) 5
- d) 15


### Solution 1
```
public class Main {
    public static void main(String[] args) {
        Integer x, y, z;
        x = 5;
        y = 3;
        if (x > y) {
            if (y > 0) {
                z = x / y;
            } else {
                z = x * y;
            }
        } else {
            z = 0;
        }
        System.out.println(z);
    }
}

** Answer B)1
```

### Question 2
```
Integer x
Set x = 5
if __ then
    Print "Positive odd"
else
    Print "Other"
end if
```
**Options:**
- a) x > 0 AND x % 2 = 1
- b) x > 0 OR x % 2 = 1
- c) NOT (x > 0)
- d) x > 0 XOR x % 2 = 1

### Solution 2
```
public class Main {
    public static void main(String[] args) {
        Integer x = 5;

        if (x > 0 && x % 2 == 1) {
            System.out.println("Positive odd");
        } else {
            System.out.println("Other");
        }
    }
}

**Answer:** a
```


### Solution 3
```
public class Question3 {
    public static void main(String[] args) {
        int n = 2;
        switch (n) {
            case 1:
                System.out.println("One");
                break;
            case 2:
                n = n + 1; 
                System.out.println("Two");
                
            case 3:
                System.out.println("Three");
                
            default:
                System.out.println("Other");
        }
    }
}

Output-- (b)
Two  
Three  
Other
```
### Solution 5
```
public class Question5 {
    public static void main(String[] args) {
        int score = 85;
        if (score >= 90) {
            System.out.println("A");
        } else if (score >= 80) {
            System.out.println("B");
        } else {
            System.out.println("C");
        }
    }
}

Output-- (c) >=
```

### Solution 6
```
public class Q6 {
    public static void main(String[] args) {
        int sum = 0;
        for (int i = 1; i <= 5; i++) {
            sum = sum + i;
        }
        System.out.println(sum);  
    }
}

Output -- (b)  15
```
### Solution 7
```
public class Q7 {
    public static void main(String[] args) {
        int sum = 0;
        for (int i = 1; i <= 3; i++) {
            for (int j = 1; j <= i; j++) {
                sum = sum + j;
            }
        }
        System.out.println(sum);  
    }
}

Output -- (b) 10
```
### Solution 8
```
    public static void main(String[] args) {
        for (int i = 1; i <= 5; i++) {
            if (i == 3) {
                continue;
            }
            System.out.print(i + " ");  
        }
    }
}

Output -- (b) continue
```
### Solution 9
```
public class Q9 {
    public static void main(String[] args) {
        int value = 2;
        int sum = 0;
        while (value <= 10) {
            sum += value;
            value += 2;
        }
        System.out.println(sum);  
    }
}


Output (a) 30
```
### Solution  10
```
public class Q10 {
    public static void main(String[] args) {
        int count = 0;
        for (int i = 1; i <= 3; i++) {
            for (int j = 1; j <= 2; j++) {
                count++;
            }
        }
        System.out.println(count);  
    }
}

Output -- (c) 6
```
#### Solution 11
```
public class Q11 {
    public static void main(String[] args) {
        int x = 5, y = 3;
        int z = x + y * x - 2;
        System.out.println(z); 
    }
}

Output -- (a) 18
```
#### Solution 12
```
public class Q12 {
    public static void main(String[] args) {
        int x = 11, y = 4;
        int result = (x - y + 121) % x;
        System.out.println(result);  
    }
}


Output --(c) 7
```
### Solution 13
```
public class Q13 {
    public static void main(String[] args) {
        int x = 10, y = 4;
        int z = x * (x - y) % y / x;
        System.out.println(z); 
    }
}

Output --(d) 0
```
### Solution 14
```
public class Q14 {
    public static void main(String[] args) {
        int a = 2, b = 5;
        int c = (a + b) * (b - a);
        System.out.println(c);  
    }
}


Output --(a) 21
```
### Solution 15
```
public class Q15 {
    public static void main(String[] args) {
        int x = 8, y = 3;
        int z = x % y * 2;
        System.out.println(z);  
    }
}

Output --(b) 4
```

#### Medium-to-high level pseudocode questions on Functions 
### Category 1: (Recursive Functions) --- 
Q1. What will be the output of the following? 
function sum(n) 
if n == 1 
return 1 
return n + sum(n - 1) 
print(sum(5))
### Solution
```

public class RecursiveSum {
    public static int sum(int n) {
        if (n == 1) {
            return 1;
        }
        return n + sum(n - 1);
    }
    public static void main(String[] args) {
        System.out.println(sum(5));
    }
}
Output will be 15
```
### Q2. Predict the result: 
function mystery(a, b) 
if b == 0 
return 0 
return a + mystery(a, b - 1) 
print(mystery(3, 4)) 
### Solution
```
public class RecursiveMultiply {
    public static int mystery(int a, int b) {
        if (b == 0) {
            return 0;
        }
        return a + mystery(a, b - 1);
    }
    public static void main(String[] args) {
        System.out.println(mystery(3, 4)); 
    }
}
Output will be 12
```
### Q3. What is the output? 
function f(n) 
if n == 0 
return 0 
else 
return n + f(n - 2) 
print(f(6))


###solution
```
 public static int f(int n) {
        if (n == 0) {
            return 0;
        } else {
            return n + f(n - 2);
        }
    }
    public static void main(String[] args) {
        System.out.println(f(6)); 
    }
}
// Output: 12
```
### Q4. Output? 
function fun(x) 
if x == 0 
return 
fun(x - 1) 
print(x) 
fun(3) 

### Solution
```
    public static void fun(int x) {
        if (x == 0) {
            return;
        }
        fun(x - 1);  
        System.out.println(x); 
    }

    public static void main(String[] args) {
        fun(3);
    }
}

```
### Q5. Output of the code: 
function fact(n) 
if n == 0 
return 1 
return n * fact(n - 1) 
print(fact(4)) 
### Solution
```
    public static int fact(int n) {
        if (n == 0) {
            return 1; 
        }
        return n * fact(n - 1); 
    }

    public static void main(String[] args) {
        System.out.println(fact(4)); 
    }
}
Output will be 24
```
### Q6. What is returned? 
function fib(n) 
if n == 0 
return 0 
else if n == 1 
return 1 
return fib(n - 1) + fib(n - 2) 
print(fib(6))
### Solution
```
    public static int fib(int n) {
        if (n == 0) {
            return 0; 
        } else if (n == 1) {
            return 1;  
        }
        return fib(n - 1) + fib(n - 2); 
    }

    public static void main(String[] args) {
        System.out.println(fib(6));  
    }
}
Output: 8
```
### Q7. Predict output: 
function fun(n) 
if n <= 1 
return n 
return fun(n - 1) + fun(n - 3) 
print(fun(5)) 

### Solution
```
public class Main {
    public static int fun(int n) {
        if (n <= 1)
            return n;
        return fun(n - 1) + fun(n - 3);
    }

    public static void main(String[] args) {
        System.out.println(fun(5));
    }
}
Output: 1

```
### Q21. What is printed? 
function modify(x) 
x = x + 10 
return x 
a = 5 
modify(a) 
print(a) 
### Solution
```
public class Q21 {
    public static int modify(int x) {
        x = x + 10;
        return x;
    }
    public static void main(String[] args) {
        int a = 5;
        modify(a);
        System.out.println(a);  
    }
}

Output: 5
```
### Q22. Output? 
function update(arr, i) 
arr[i] = arr[i] + 5 
arr = [1, 2, 3] 
update(arr, 1) 
print(arr[1]) 
### Solution
```
public class Q22 {
    public static void update(int[] arr, int i) {
        arr[i] = arr[i] + 5;
    }

    public static void main(String[] args) {
        int[] arr = {1, 2, 3};
        update(arr, 1);
        System.out.println(arr[1]); 
    }
}
Output: 7

```

### Q23. Output of the code: 
x = 100 
function check() 
x = 50 
print(x) 
check() 
print(x)
### Solution
```
    static int x = 100;
    public static void check() {
        int x = 50;
        System.out.println(x); 
    }
    public static void main(String[] args) {
        check();
        System.out.println(x); 
    }
}

Output:50
       100

``` 
### Q24. What will be the output? 
a = 10 
function test() 
global a 
a = a + 5 
test() 
print(a)
### Solution
```
    static int a = 10;
    public static void test() {
        a = a + 5;
    }
    public static void main(String[] args) {
        test();
        System.out.println(a);  
    }
}
Output: 15
```
### Q25. Trace the output: 
function modify(x) 
x = x * 2 
return x 
x = 4 
x = modify(x) 
print(x) 
### Solution
```
public class Q25 {
    public static int modify(int x) {
        x = x * 2;
        return x;
    }
    public static void main(String[] args) {
        int x = 4;
        x = modify(x);
        System.out.println(x);  
    }
}
Output: 8
```
### Q26. What is printed? 
x = 5 
function demo(x) 
x = x + 1 
print(x) 
demo(x) 
print(x) 
### Solution
```
    public static void demo(int x) {
        x = x + 1;
        System.out.println(x);  
    }

    public static void main(String[] args) {
        int x = 5;
        demo(x);
        System.out.println(x);  
    }
}
Output: 6
        5


```
### Q27. Predict the output: 
function add(val) 
val = val + 10 
a = 3 
add(a) 
print(a) 
### Solution
```
    public static void add(int val) {
        val = val + 10;
    }

    public static void main(String[] args) {
        int a = 3;
        add(a);
        System.out.println(a); 
    }
}
Output: 3
```
### Q28. What will be the output? 
function fun(x) 
y = x + 10 
return y 
y = 5 
z = fun(y) 
print(y, z)
### Solution
```
    public static int fun(int x) {
        int y = x + 10;
        return y;
    }

    public static void main(String[] args) {
        int y = 5;
        int z = fun(y);
        System.out.println(y + " " + z);
    }
}

Output: 5 15
``` 
### Q29. Scope analysis – What’s printed? 
x = 1  
function outer() 
    x = 2 
    function inner() 
        print(x) 
    inner() 
outer() 
 ### Solution
```
    static int x = 1;
    public static void outer() {
        int x = 2;
        class Inner {
            void inner() {
                System.out.println(x); 
            }
        }
        new Inner().inner();
    }
    public static void main(String[] args) {
        outer(); 
    }
}
Output: 2
```
### Q30. Output? 
x = 10  
function show() 
    print(x) 
    x = 20 
show() 
### Solution
```
```
### Q.Print pattern using recursion
### Solution
```
public class Main {
    public static void pattern(int n) {
        if (n == 0) return;  
        pattern(n - 1);      
        for (int i = 0; i < n; i++)
            System.out.print("*");
        System.out.println();
    }
    public static void main(String[] args) {
        pattern(4);  
    }
}
Output:
*
**
***
****
```
### Recursive power function
## Solution
```
public class Main {
    public static int power(int base, int exp) {
        if (exp == 0) return 1;
        return base * power(base, exp - 1);
    }
    public static void main(String[] args) {
        System.out.println(power(2, 5));
    }
}
Output: 32
```
### Find String Code 
### Solution
```
import java.io.*;
import java.util.*;

class UserMainCode {
    public int findStringCode(String input1) {
        String[] words = input1.toUpperCase().split(" ");
        StringBuilder result = new StringBuilder();

        for (String word : words) {
            int sum = 0;
            int left = 0;
            int right = word.length() - 1;

            while (left <= right) {
                int leftVal = word.charAt(left) - 'A' + 1;
                int rightVal = word.charAt(right) - 'A' + 1;
                if (left == right) {
                    // middle letter for odd length words — add directly
                    sum += leftVal;
                } else {
                    sum += Math.abs(leftVal - rightVal);
                }
                left++;
                right--;
            }

            result.append(sum);
        }

        return Integer.parseInt(result.toString());
    }
}

```
### GetCodeThroughStrings
### Solution
```
```










