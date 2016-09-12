# GoFor

      LINEAR SEARCH                                              BINARY SEARCH
{
int a[10]={11,2,9,313,57,27,17,1,90,3}      |       int binaryS (int a[],int n,int value)
int num,i;                                  |       {
printf("enter number to search");           |       int first=0, last=n-1, middle;
scanf("%d",num);                            |       while ( first < last)
for(i=0;i<10;i++)                           |       {
{                                           |       middle  = (first+last)/2;
if(a[i]==num)                               |       if ( a[middle]==value)
break;                                      |       {
}                                           |       return middle;
if(i==10)                                   |       }
printf("number is not there");              |       else if ( a[middle]>value)
else                                        |        last = middle-1;
printf("number is in %d position");         |       else
}                                           |       first = midlle+1;
                                                    }
