# EX-11-EMI-CALCULATOR

## AIM

To write a program to prepare EMI calculator using function without return type and with arguments.

## ALGORITHM

1.	Start the program.
2.	Read principal amount, rate of interest and months.
3.	Pass these values as arguments to function.
4.	Calculate EMI using the formula, amt=(prpow(1+r,t))/(pow(1+r,t)-1)
5.	Display the result.
6.	Stop the program.

## PROGRAM

```

#include <stdio.h>
#include <math.h>

void emi(float p, float r, int n) {
    float m, i, x;
    i = r / 1200;
    x = pow(1 + i, n);
    m = (p * i * x) / (x - 1);
    printf("EMI = %.2f\n", m);
}

int main() {
    float a, b;
    int c;
    scanf("%f%f%d", &a, &b, &c);
    emi(a, b, c);
    return 0;
}

```


## OUTPUT

![Screenshot 2025-05-17 131657](https://github.com/user-attachments/assets/342ee303-a0b8-4686-9c2e-ab676a5fe5d3)


## RESULT

Thus the program to prepare EMI calculator using function without return type with arguments has been executed successfully
 
 


# EX-12-FIBONACCI-SERIES
## AIM
To write a C program to generate the Fibonacci series for the value 6.

## ALGORITHM
1.	Start the program.
2.	Read number of terms to display.
3.	Add the previous two terms and store it in new term.
4.	Assign 2nd term to 1st term and 3rd term to 2nd term.
5.	Repeat steps 3 and 4 n number of times.
6.	Display the result.
7.	Stop the program.

## PROGRAM

```

#include <stdio.h>

int main() {
    int n = 6, a = 0, b = 1, c, i;
    printf("%d %d ", a, b);
    for(i = 2; i < n; i++) {
        c = a + b;
        printf("%d ", c);
        a = b;
        b = c;
    }
    return 0;
}

```

## OUTPUT

![Screenshot 2025-05-17 131946](https://github.com/user-attachments/assets/1552e546-7a9a-4b98-9f0c-89367f1ac3f3)


## RESULT
Thus the program to generate the Fibonacci series for the value 6 has been executed successfully.
 
 


# EX-13-ONE-DIMENSIONAL-ARRAY
## AIM
To write a C program to read n elements as input and print the last element of the array.

## ALGORITHM
1.	Start the program.
2.	Read a variable.
3.	Read the array values n number of times.
4.	Print the last element.
5.	Stop the program.

## PROGRAM
```

#include <stdio.h>

int main() {
    int n, i, a[100];
    scanf("%d", &n);
    for(i = 0; i < n; i++)
        scanf("%d", &a[i]);
    printf("%d", a[n-1]);
    return 0;
}

```
## OUTPUT

![Screenshot 2025-05-17 132151](https://github.com/user-attachments/assets/818efc52-ea8b-4a07-949f-282c917d075a)


## RESULT
Thus the program to read n elements as input and print the last element of the array has been executed successfully.
 
 


# EX-14-POSITIVE-ARRAY-ELEMENTS
## AIM
To write a C Program to count total number of positive elements in an array.

## ALGORITHM
1.	Start the program.
2.	Read a variable.
3.	Read the array values n number of times.
4.	If the array value can be divided by 2 then increment count by 1.
5.	Display result.
6.	Stop the program.

## PROGRAM

```

#include <stdio.h>

int main() {
    int n, i, a[100], c = 0;
    scanf("%d", &n);
    for(i = 0; i < n; i++) {
        scanf("%d", &a[i]);
        if(a[i] > 0)
            c++;
    }
    printf("%d", c);
    return 0;
}

```

## OUTPUT

![image](https://github.com/user-attachments/assets/c2c0edb9-96bf-41fe-b071-98bea47ed9bc)




## RESULT
Thus the program to count total number of positive elements in an array has been executed successfully.





 
 


# EX -15 - Replace All Even Elements With 'E' In One Dimensional Array

## Aim:
To write a C program to replace all even elements with 'E' in one dimensional array

## Algorithm:
1.	Input the array:
  Read the size of the array.
  Input the elements of the array.
2.	Iterate through the array:
 	For each element of the array, check if the element is even (i.e., if the element modulo 2 equals 0).
3.	Replace even elements with 'E':
     If an element is even, replace that element with the character 'E'.
4.	Output the updated array:
 Print the updated array after replacements.

## Program:

```
#include <stdio.h>

int main() {
    int n, i, a[100];
    scanf("%d", &n);
    for(i = 0; i < n; i++)
        scanf("%d", &a[i]);
    for(i = 0; i < n; i++) {
        if(a[i] % 2 == 0)
            printf("E ");
        else
            printf("%d ", a[i]);
    }
    return 0;
}

```

## Output:
 
![Screenshot 2025-05-17 142321](https://github.com/user-attachments/assets/3005a619-8d10-4687-aa6d-c8f36b59d67a)

## Result:

Thus, the program to replace all even elements with 'E' in one dimensional array was verified successfully.



