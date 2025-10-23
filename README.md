# Module-3 Day-3 SEB
## AIM:
To write a C program to accept N numbers and arrange them in an ascending order

## For example:

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
