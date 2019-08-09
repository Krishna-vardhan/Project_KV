#include <stdio.h>

int main()
{
    int a[2],price,cost,i;
    for(i=0;i<2;i++)
    {
        scanf("%d",&a[i]);
    }
    price=a[0];
    cost=a[0];
    a[1]=100-a[1];
    
    while(price != 0)
    {
        price=(price/100)*a[1];
        
        cost=cost+price;
    }
    printf("%d",cost);
    

    return 0;
}
