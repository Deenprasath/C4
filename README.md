write a program to print the perfect subset from the starting point of the string example input missisipi out put miss

#include <stdio.h>
#include<string.h>
int main()
{
   
   char str[100], sstr[100];
   
   int i=0,n,j=0;
   printf("\n enter the string");
   scanf("%s",str);
   printf("\n enter the no of char to copy");
   scanf("%d",&n);
   j=strlen(str)-n;
   while (str[j] !='\0')
   {
       sstr[i] = str[j];
       i++;j++;
   }
   sstr[i]='\0';
   printf("the substring is:");
   puts(sstr);
   return 0;
}
