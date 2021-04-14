#include<stdio.h>
#include<conio.h>
int main()
{
    int a,b,n,i,sum=0;
    printf("No of orders - ");
    scanf("\n%d", &n);
    for(i=0;i<n;i++)
    {
        printf("Order %d",i+1);
        printf("\nLength - ");
        scanf("%d", &a);
        printf("\nBreath - ");
        scanf("%d", &b);
        if((a<=210 && b<=297) || (a<=297 && b<=210))
        {
            sum=sum+10;
        }
        else if((a<=297 && b<=420) || (a<=420 && b<=297))
        {
            sum=sum+15;
        }
        else if((a<=420 && b<=594) || (a<=594 && b<=420))
        {
            sum=sum+20;
        }
        else if((a<=594 && b<=841) || (a<=841 && b<=594))
        {
            sum=sum+25;
        }
    }
    printf("Rs%d ",sum);
    return 0;
}

