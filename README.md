# DSA_solutions

#question
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


### Solution 
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

##Question 2
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

###Solution 
```public class Main {
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



