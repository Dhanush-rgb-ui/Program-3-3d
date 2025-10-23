# Module-3 Day-4 SEB
## AIM:
To write a C program to accept N numbers and arrange them in an ascending order

## For example:
<img width="525" height="182" alt="image" src="https://github.com/user-attachments/assets/ae0fac67-6218-4407-9e99-ac6f79630341" />

## Program:
```c
#include<stdio.h>
int main(){
    int n,i,j,temp=0;
    scanf("%d",&n);
    int a[n];
    for(i=0;i<n;i++){
        scanf("%d",&a[i]);
    }
    printf("The numbers arranged in ascending order are given below\n");
    for(i=0;i<n-1;i++){
        for(j=i+1;j<n;j++){
            if(a[i]>a[j]){
                temp=a[i];
                a[i]=a[j];
                a[j]=temp;
            }
        }
    }
    for(i=0;i<n;i++){
        printf("%d\n",a[i]);
    }
    return 0;
}
```
## Result:
<img width="1055" height="180" alt="image" src="https://github.com/user-attachments/assets/fe482072-868e-4b78-b282-c69bc33fa477" />
