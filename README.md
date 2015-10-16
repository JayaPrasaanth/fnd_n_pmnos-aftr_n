#include <stdio.h>
int isprime(int);
int main() {
    int n1,n2,i,c=0;
	scanf("%d %d", &n1, &n2);
	for(i=n1+1;;i++)
      {
          if(isprime(i))
           {
               c++;
               if(c==n2)
               {
                   printf("%d\n",i);
                   break;
               }
           }
      }
}

int isprime(int i)
 {
     int a=0,n;
     for(n=1;n<=i/2;n++)
      {
          if(i%n==0)
           a++;
      }
      if(a==1)
       {
           return 1;
       }
       else
       {
           return 0;
       }
 }
