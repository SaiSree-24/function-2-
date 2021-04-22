# function-2-
created by saisree to check prime numbers

#include<stdio.h>
int prime(int, int);
int main()
{
    int num=456,check;
    check=prime(num,num/2);
    if (check==1)
    {
        printf("%d is a prime number",num);
    }
    else
    {
        printf("%d is not a prime number",num);
    }
    return 0;
}
int prime(int num,int i)
{
    if(i==1)
    {
        return 1;
    }
    else
    {
        if (num%i==0)
        {
            return 0;
        }
    
      else
      {
         return prime(num,i-1);
       }
    }
}
