# Deletion-of-array-in-C-language
#include <stdio.h>
int main()
{
   int arr[100],a,c,n;
   printf("Enter number of elements in array\n");
   scanf("%d",&n);
   printf("Enter %d elements\n",n);
   for(c=0;c<n;c++)
      scanf("%d",&arr[c]);
   printf("Enter the loc.where element u want to delete\n");
   scanf("%d",&a);
   if (a>=n+1)
      printf("Delete error\n");
   else
   {
      for (c=a-1;c<n-1;c++)
         arr[c]=arr[c+1];
      printf("the array is\n");
      for(c=0;c<n-1;c++)
         printf("%d\n",arr[c]);
   }
   return 0;
}
