#include<stdio.h>
int power(int n)
{
    int a;
    printf("Enter the power : ");
    scanf("%d",&a);
    for(int i=1;i<a;i++)
    {
        n=n*n;
    }
    return n;
}
int main()
{
    int n,c;
    printf("Enter the number : ");
    scanf("%d",&n);
    c=power(n);
    printf("%d\n",c);
}
