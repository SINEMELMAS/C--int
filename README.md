# C--int
#include <stdio.h>
unsigned int mystery(unsigned int a, unsigned int b)
{
if (1==b)
{
   return b;
}
else
{
   return a+ mystery(a,b-1);
}
}
int main (void)
{
   unsigned int x;
   unsigned int y;
   printf("Enter two positive integers: ");
   scanf("%u%u", &x, &y);
   printf("The result is %u\n", mystery(x, y));
}
