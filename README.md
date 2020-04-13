# pointers
Developed by Gunjan Narkhede
#include<stdio.h>
int main()
{
    int arr[3][3],*p,i,j,sum=0;
    printf("enter the nine elements of matrix");
    for(i=0;i<=2;i++)
    {
    	for(j=0;j<=2;j++)
    	{
    		scanf("%d",&arr[i][j]);   	    
        }
     }
    for(p=&arr[0][0];p<=&arr[2][2];p++)
    {
    	printf("%d",*p);
    }
    printf("\n sum of diagonal elements is:");
     for(p=&arr[0][0];p<=&arr[2][2];p+=2)   
     {
     	sum+=*p;
     }
     printf("%d",sum);
    return 0;
}
   
