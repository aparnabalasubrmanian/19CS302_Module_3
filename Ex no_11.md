
# EX 11 C Program to convert a given decimal value to binary using function without arguments with return type.
## DATE: 27.3.25
## AIM:
To write a C Program to convert a given decimal value to binary using function without arguments with return type.

## Algorithm
1. Start. 
2. Declare a integer variable 
3. Define a function named dectobin. 
4. Return the integer. 
5. Read the value using scanf. 
6. Convert decimal to binary value. 
7. Print the dectobin 
8. End. 

## Program:
```
/*
Developed by: Aparna RB
RegisterNumber:  212222220005
*/
#include <stdio.h>

int convert(int n)
{
    int bin = 0, base = 1;
    while (n > 0)
    {
        int r = n % 2;
        bin = bin + r * base;
        base *= 10;
        n /= 2;
    }
    return bin;
}

int main()
{
    int n;
    scanf("%d", &n);
    int binary = convert(n);
    printf("%d in decimal = %d in binary", n, binary);
    return 0;
}
 

```

## Output:
![image](https://github.com/user-attachments/assets/2cc91549-e7aa-4431-ac3e-17cead304549)



## Result:
Thus the program was executed and the output was verified successfully.
