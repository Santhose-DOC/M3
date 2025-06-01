# NAME : SANTHOSE AROCKIARAJ J
# REGISTER NO: 212224230248 

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
#include<math.h>
void emi(float p,float r,float n)
{
    r=r/(100*12);
    n=n*12;
    float emi=p*r*pow(1+r,n)/(pow(1+r,n)-1);
    printf("Monthly EMI is= %.3f",emi);
}
int main()
{
    float p,n,r;
    scanf("%f %f %f",&p,&r,&n);
    emi(p,r,n);
}


```

## OUTPUT


![447615715-a088e829-8ab3-4f0c-8234-5ff5a3085ab9](https://github.com/user-attachments/assets/d4406465-bfca-4476-b4c7-186b65837c53)



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
#include<stdio.h>
void fibonacci(int n)
{
    int temp=-1,a=1,b=0;
    for (int i=1;i<=n;i++)
    {
        temp=a+b;
        a=b;
        b=temp;
        printf("%d ",a);
       
    }
}
int main()
{
    int num;
    scanf("%d",&num);
    fibonacci(num);
}
```

## OUTPUT

![447616308-b8b8dd7c-d49e-4845-86d1-0b58ae0d532b](https://github.com/user-attachments/assets/432bd607-697d-414d-8f64-0227c3a6171d)







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

#include<stdio.h>
int main()
{
    int n,i;
    scanf("%d",&n);
    int arr[n];
    for (i=0;i<n;i++)
    {
        scanf("%d",&arr[i]);
    }
    if (n>0) printf("%d\n",arr[n-1]);
    else printf(" ");   
}
```
## OUTPUT





![447616597-2426aa2f-d79e-44c8-b2a8-b9b9d3257453](https://github.com/user-attachments/assets/abc9b2d2-7dfb-4220-8ad7-0d0482499ec1)




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
#include<stdio.h>
int main()
{
    int n,i;
    scanf("%d",&n);
    int arr[n],count_pos=0,count_neg=0;
    for (i=0;i<n;i++)
    {
        scanf("%d",&arr[i]);
        if (arr[i]>0) count_pos++;
        else count_neg++;
    }
    printf("count  of positive numbers  in array: %d\n",count_pos);
    printf("count  of negative numbers  in array: %d",count_neg);
}

```

## OUTPUT


![447616705-810d3c65-1ce9-46e7-b11e-6cc87e3db047](https://github.com/user-attachments/assets/83af6f65-10a9-44f3-b6c8-a1a472333857)



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
    int n;
    scanf("%d", &n);

    int arr[n];
    for (int i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }

    for (int i = 0; i < n; i++) {
        if (arr[i] % 2 == 0) {
            arr[i] = 'E';  // Replacing even numbers with 'E'
        }
    }

    for (int i = 0; i < n; i++) {
        if (arr[i] == 'E') {
            printf("E ");
        } else {
            printf("%d ", arr[i]);
        }
    }

    return 0;
}
```
## Output:
 
![447616841-ebb4196b-0a0f-4a77-adc2-e3925ca1ac57](https://github.com/user-attachments/assets/94147ab8-8d80-4615-b685-2520534ef903)


## Result:

Thus, the program to replace all even elements with 'E' in one dimensional array was verified successfully.



