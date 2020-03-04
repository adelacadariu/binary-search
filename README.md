#define_CRT_SECURE_NO_WARNINGS
#include<stdio.h>
#include<stdlib.h>
int main()
{
int n, pr,ul,mijl,i,căutat,a[100];
printf(“ dați nr de elemente: “);
scanf(“%d”,&n);
for(i=0;i<n;i++)
{
printf(“\n introduceți elementul %d”,i+1);
scanf(“%d,&a[i]);
}
printf(“\n elementul căutat : “);
scanf(“%d”,&căutat);
pr=0;
ul=n-1;
mijl=(pr+ul)/2;
while(pr<=ul)
{
if (a[mijl]<căutat)
pr=mijl+1;
else
 if(a[mijl]==căutat)
{ printf(“ elementul căutat este pe poziția %d”,mijl+1);
break;
}
else
ul=mijl-1;
mijl=(pr+ul)/2;
}
if(pr>ul)
printf(“\n elementul căutat nu se afla in șir”;
system(“pauze”);
return 0;
}
