# c-program-p5
/* WACP to generate n primes */
#include<stdio.h>
int main()
{
    int i,j,n;
    printf("enter the number till which you want generate the primes:\n",n);
    scanf("%d",&n);
    printf("prime number are up to %d are:\n",n);
    for(i=2;i<n;i++)
        {
            int c=0;
            for(j=1;j<=i;j++)
                {
                if(i%j==0)
                {
                    c++;
                }
                }
            if(c==2)
                printf("%d\t",i);
        }
}
