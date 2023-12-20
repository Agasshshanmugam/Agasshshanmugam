#include<stdio.h>
int main()
{
    int n;
    printf("Enter the number : ");
    scanf("%d",&n);
    printf("The given number is %d\n",n);
    inc(n);
    printf("After increement is %d\n",n);
}
void inc(int n)
{
    n=n+1;
    printf("Increement = %d\n",n);
}
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
/with no arguement and no return type
#include<stdio.h>
int main()
{
    as();
}
void as()
{
    int a;
    printf("Enter the side of the square : ");
    scanf("%d",&a);
    a=a*a;
    printf("The area of the square is %d",a);
}


//with arguement and no return type
#include<stdio.h>
int main()
{
    int a;
    printf("Enter the side of the square : ");
    scanf("%d",&a);
    as(a);
}
void as(int a)
{
    a=a*a;
    printf("The area of the sqaure is %d",a);
}


//with return type and no arguement
#include<stdio.h>
int main()
{
    as();
    printf("The area of square is %d",as());
}
int as()
{
    int a;
    printf("Enter the side of the square : ");
    scanf("%d",&a);
    a=a*a;
    return a;
    
}


//with arguement and return type
#include<stdio.h>
int main()
{
    int a;
    printf("Enter the side of the square : ");
    scanf("%d",&a);
    as(a);
    printf("The area of sqaure is %d",as(a));
}
int as(int a)
{
    a=a*a;
    return a;
}
#include<stdio.h>
int main()
{
    int n;
    printf("Enter the number : ");
    scanf("%d",&n);
    printf("The given number is %d\n",n);
    inc(&n);
    printf("After increement is %d\n",n);
}
void inc(int *n)
{
    *n=*n+1;
    printf("Increement = %d\n",*n);
