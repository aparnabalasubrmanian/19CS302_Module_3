
# EX 12 C program to check whether the given number is prime or not using function without return type and with arguments.
## AIM:
To write a C program to check whether the given number is prime or not using function without return type and with arguments.

## Algorithm
1. Start 
2. Declare the variable i. 
3. Read the value given using scanf. 
4. Check whether the given number is prime or not using if-else statement condition. 
5. If true,print ("%d is a prime number.",i). 
6. If false, print ("%d is not a prime number.",i). 
7. End.
   
## Program:
```
/*
Developed by: Aparna RB
RegisterNumber:  212222220005
*/

#include <stdio.h>
void checkPrime(int n);

int main()
{
    int num;
    scanf("%d", &num);

    checkPrime(num); 
    return 0;
}
void checkPrime(int n)
{
    int i, flag = 0;

    if (n <= 1) {
        printf("%d is not a prime number", n);
        return;
    }

    for (i = 2; i <= n / 2; i++) {
        if (n % i == 0) {
            flag = 1;
            break;
        }
    }

    if (flag == 0)
        printf("%d is a prime number", n);
    else
        printf("%d is not a prime number", n);
}

```

## Output:
![image](https://github.com/user-attachments/assets/8a30ffee-099f-4226-a72f-3d4ebe61c38b)



## Result:
Thus the program was executed and the output was verified successfully.
