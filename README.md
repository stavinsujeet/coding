# coding
include <stdio.h>

{
  int i,limit,num,num2[100],digit,j,k,sum,num3,b,temp;
  scanf("%d",&limit);
  
  for(i=0;i<limit;i++)
  {
    sum=0;
    scanf("%d",&num);
  j=0;
    while(num!=0)
    {
     b=num%10;
      temp=b+1;
    num2[j]=temp;
      j++;
    num=num/10;
    }
    for(k=j-1;k>=0;k--)
    {
      sum=sum*10+num2[k];
    }
    printf("%d\n",sum);
  }

  
    return 0;
}
