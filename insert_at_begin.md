![insert_at_begin](https://user-images.githubusercontent.com/92702328/149530233-d4ad9379-1618-4bbb-a194-55688dd0a7c9.png)
<b><font size="5">Write a C program to insert a element at <u>beginning of array</u></b></font>
```

#include<stdio.h>
int main()
{
    int n,a[10],i,ele;
    printf("Enter size of array: ");
    scanf("%d",&n);
    printf("\nEnter array elements:\n ");
    for(i=0;i<n;i++)
    {
      scanf("\n%d",&a[i]);
    }
    printf("\nArray elements are: ");
     for(i=0;i<n;i++)
    {
      printf("\n%d",a[i]);
    }
    n++;
    printf("\nEnter element which is to be inserted at beginning: ");
    scanf("%d",&ele);
    for(i=n;i>1;i--)
    {
        a[i-1]=a[i-2];
    }
    a[0]=ele;
    printf("\nAfter inserting array elements are: ");
     for(i=0;i<n;i++)
    {
      printf("\n%d",a[i]);
    }
    return 0;
}
```
<b><u><font size="6">OUTPUT</u></b></font>

![][output](insert_at_begin.png)
