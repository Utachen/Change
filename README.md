Change
======
#include<stdio.h>
#include<STRING.h>
#include<stdlib.h>
#include<iostream>
using namespace std;
int main()
{
char tem[10],flag;
int n;
double x,y;
cout<<"please input the temperature: ";
gets(tem);
n=strlen(tem);
flag=tem[n-1];
tem[n-1]='\n';
x=atof(tem);
if (flag=='f'||flag=='F')//华氏转摄氏
{
y=(x-32)/1.8;
} 
else if (flag=='c'||flag=='C')//摄氏转华氏
{
y=1.8*x+32;
}
printf("%.1f\n",y);
}
