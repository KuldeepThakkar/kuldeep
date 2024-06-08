#include<stdio.h>
#include<conio.h>
#define p printf
#define s scanf
void main()
{
 int i,j,a[100],n,temp;
 clrscr();
 p("enter your no of alementd= ");
 s("%d",&n);

 for(i=0;i<n;i++)
 {
  p("enter your [%d]no= ",i+1);
  s("%d",&a[i]);
 }

 for(i=0;i<n;i++)
 {
  for(j=0;j<n-1;j++)
  {
   if(a[j]>a[j+1])
   {
    temp=a[j];
    a[j]=a[j+1];
    a[j+1]=temp;
   }
  }

 }

 for(i=0;i<n;i++)
 p("%d ,",a[i]);
getch();
}
