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
### Category 1: Recursive Functions 
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








