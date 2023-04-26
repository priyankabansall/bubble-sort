# bubble-sort
#include<stdio.h>
 void Bubblesort(int [],int );
 void main()
 {
 int ele;
 int arr[5]={32,5,7,3,6};
 Bubblesort(arr,5);
 printf("\n Enter element to be searched \n ");
 scanf("%d",&ele);int result;
 result= BinarySearch(arr,5,ele);
 if(result==-1)
 {
     printf("Element not found");
 }
 else
     printf("Element found at index %d",result);
 }

 void Bubblesort(int arr[],int n)
 {
     int passes=n-1;
     int comparisons=n-1;
     int i,j,temp;
     for(i=0;i<passes;i++)
     {
         for(j=0;j<comparisons-i;j++)
         {
           if(arr[j]>arr[j+1])
           {
             temp=arr[j];
             arr[j]=arr[j+1];
             arr[j+1]=temp;
           }  
         }
     }printf("\n Array sorted by Bubble sort: \n");
     for(i=0;i<n;i++)
     {
         printf(" %d ",arr[i]);
     }
 }
