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
