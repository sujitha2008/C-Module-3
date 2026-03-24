# C-Module-3
# Program 1:
## AIM: 
To write a C program to convert a decimal number to binary number. 
## ALGORITHM: 
```
1) Get a decimal number as input from the user. 
2) Divide the number again and again by 2 and store the remainder in an array. 
3) Print the elements of the array in reverse using for loop. 
```
## PROGRAM: 
``` 
#include <stdio.h> 
int tobinary(int ); 
int tobinary(int num) 
{ 
    int bin[32],ind=0; 
    while(num>0) 
    { 
        bin[ind]=num%2; 
        num/=2; 
        ind++; 
    } 
    for(int j=ind-1;j>=0;j--) 
    { 
        printf("%d",bin[j]); 
    } 
    return 0; 
} 
int main() 
{ 
    int num; 
    scanf("%d",&num); 
    printf("%d in decimal = ",num); 
    tobinary(num); 
    printf(" in binary"); 
     
} 
``` 
## OUTPUT: 
<img width="811" height="197" alt="Screenshot 2025-10-20 101351" 
src="https://github.com/user-attachments/assets/2182c8cf-3dbb-4466-bce7-20dc1e74d26d" 
/> 
## RESULT: 
Thus the C program to convert the given decimal number to binary number is executed 
successfully.  
# Program 2:
## AIM: 
To write a C program to check whether a given number is a armstrong number or not. 
## ALOGRITHM: 
```
1) Get a number as input from the user. 
2) Check whether the number is armstrong or not by using looping statements. 
3) print the result using printf() function.
```
## PROGRAM: 
``` 
#include<stdio.h> 
#include<math.h> 
int main() 
{ 
    int num,org,n=0,sum=0; 
    scanf("%d",&num); 
    org=num; 
    for(int i=num;i!=0;i/=10) 
    { 
     n++;    
    } 
    for(int i=num;i!=0;i/=10) 
    { 
       sum+=pow(num%10,n);  
    } 
    if(sum==org) 
    printf("%d is a armstrong number",org); 
    else 
    printf("%d is not a armstrong number",org); 
     
} 
```
## OUTPUT: 
<img width="729" height="135" alt="Screenshot 2025-10-20 102944" 
src="https://github.com/user-attachments/assets/0f6ed030-6a03-48ad-bf3f-672d88139a46" 
/> 
## RESULT: 
Thus the C program to check whether the given number is a armstrong number of not is 
executed successfully. 
# Program 3:
## AIM: 
To write a C program to read the elements of an array and print the first element of each row. 
## ALGORITHM: 
```
1) Get an array as input from the user. 
2) print the first element of each row using for loop and index positions of the array elements. 
```
## PROGRAM: 
``` 
#include <stdio.h> 
 
int main() 
{ 
    int n; 
     
    scanf("%d",&n); 
    int a[n][n]; 
    for(int i=0;i<n;i++) 
    { 
       for(int j=0;j<n;j++) 
       { 
        scanf("%d",&a[i][j]); 
       } 
    } 
        for(int i=0;i<n;i++) 
        printf("a[%d][0] is %d\n",i,a[i][0]); 
 
    return 0; 
} 
```
## OUTPUT: 
<img width="724" height="306" alt="Screenshot 2025-10-20 104156" 
src="https://github.com/user-attachments/assets/32605a17-d2e7-45d0-8871-dff5ffa846dc" /> 
## RESULT: 
Thus the c program to get an array as input and print the first element of each row is 
executed successfully. 
# Program 4:
## AIM: 
To write a C program to get an array and a element as input and search the element in that 
array. 
## ALOGORITHM: 
```
1) Get an array as input from the user. 
2) get an element to search. 
3) Search the element in that array using for loop. 
4) Print the index position of the element. 
```
## PROGRAM:  
``` 
#include<stdio.h> 
int main() 
{ 
    int num; 
    scanf("%d",&num); 
    int arr[num]; 
    for(int i=0;i<num;i++) 
    { 
        scanf("%d",&arr[i]); 
    } 
     
     
    for(int i=0;i<num;i++) 
    { 
        if(arr[i]==5) 
        printf("5 is found at position %d",i+1); 
    } 
} 
``` 
## OUTPUT: 
<img width="800" height="112" alt="Screenshot 2025-10-20 105522" 
src="https://github.com/user-attachments/assets/2c1e58f3-3b08-4213-b44c-c72469ab6b29" 
/>  
## RESULT: 
Thus the c program to get an array as input and search an element in that array is executed 
successfully. 
# Program 5:
## AIM: 
To write a C program to count the number if odd and even elements in an array. 
## ALGORITHM: 
```
1) Get an array as input from the user. 
2) Count the number of odd and even elements by using for loop and if else statements. 
3) Print the number of odd and even elements  using printf() function. 
```
## PROGRAM: 
``` 
#include<stdio.h> 
int main() 
{ 
    int num,odd=0,even=0; 
    scanf("%d",&num); 
    int arr[num]; 
    for(int i=0;i<num;i++) 
    { 
        scanf("%d",&arr[i]); 
    } 
    for(int j=0;j<num;j++) 
    { 
        if(arr[j]%2==0) 
        even++; 
        else 
        odd++; 
         
    } 
    printf("Total even elements: %d\n",even); 
    printf("Total odd elements: %d",odd);  
} 
``` 
## OUTPUT: 
<img width="773" height="126" alt="Screenshot 2025-10-20 110415" 
src="https://github.com/user-attachments/assets/02888641-2331-4312-95c0-385611fc323c" 
/> 
## RESULT: 
Thus the C program to count the number of odd and even elements in a given array is 
executed successfully. 

 
