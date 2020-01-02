# sum-of-rows-in-a-2-d-array

#include<stdio.h>
#include<conio.h>
   void main()
  {
    int m,n,i,j,sum=0;
     printf("Enter how many rows and column ");
     scanf("%d%d", &m,&n);
    int a[m][n];
    printf("Enter the elements ");
      for(i=1;i<=m;i++)
        for(j=1;j<=n;j++)
          scanf("%d",&a[i][j]);
          printf("The entered array is\n");
           for(i=1;i<=m;i++)
            {
              for(j=1;j<=n;j++)
              {
              printf("%3d", a[i][j]);
              }
              printf("\n");
             }
                for(i=1;i<=m;i++)
                   {
                      for(j=1;j<=n;j++)
                        {
                          sum+=a[i][j];
                         }
                          printf("The sum of %d row is %d",i,sum);
                          printf("\n");
                          sum=0;
                       }
      }
                          
                          
    
