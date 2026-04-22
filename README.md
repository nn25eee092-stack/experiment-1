#include <stdio.h>
#include <stdlib.h>

int main()
{
    float a,b,c,d,r1,r2,realpart,imagpart;
    printf("enter any value:\n");
    scanf("%f%f%f",&a,&b,&c);
    d=b*b-4*a*c;
    if(d>0)
    {
     r1=(-b+sqrt(d))/(2*a);
     r2=(-b-sqrt(d))/(2*a);
     printf("the roots are equal and distinct and their values are r1 and r2%f\n%f\n",r1,r2);
     }
     else
     if(d==0)
     {
     r1=r2=((-b)/(2*a));
     printf("the roots are real and equal r1==r2 and their value is %f\n",r1,r2);
     }
     else
     {
     realpart=(-b/(2*a));
     imagpart=sqrt(-d)/(2*a);
     printf("the roots are imaginary:%f+%fi and %f-%fi\n",realpart,imagpart,realpart,imagpart);
     }
    return 0;
}
