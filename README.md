// hackerrank-operator-30-days-of-code
#include<stdio.h>
#include<stdlib.h>
int tax(int n,int mealcost)
{
    float tax_;
    tax_=n*mealcost/100;
    return (tax_);
}
float tip(int n,int mealcost)
{
    float tip_;
    tip_=n*mealcost/100;
    
    return(tip_);
}
int main()
{
   float mealcost;
   int tipper;
   int taxper;
   int sum=1;
   scanf("%f",&mealcost);
   scanf("%d",&tipper);
   scanf("%d",&taxper);
   sum= tip(taxper,mealcost)+tax(taxper,mealcost)+mealcost;



   printf("%d",sum);
}
