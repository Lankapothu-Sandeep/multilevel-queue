#include<stdio.h>
int main()
{
int arrival_TIme11[10],Burst_TIme11[10],array[10],Endt,i,shortest;
int left=0,n,TIme11,s_wiat=0,s_turn_arn_d=0;
printf("****************************SIMULATION OF SROT AND RR IN MULTILEVEL QUEUE ***********************************\n");
printf("**********************************************WELCOME********************************************************\n");
printf("*****************************ENTER THE DETAILS ABOUT THE PROCESSES***************************************\n\n");
printf("PLEASE ENTER THE NO OF PROCESSES");
scanf("%d",&n);
for(i=0;i<n;i++)
{	
printf("NOW ENTER THE ARRIVAL TIME OF PROCESS P%d : ",i+1);
scanf("%d",&arrival_TIme11[i]);
printf("NEXT ENTER THE BURST TIME OF PROCESS P%d : ",i+1);
scanf("%d",&Burst_TIme11[i]);
array[i]=Burst_TIme11[i];
}
printf("\n\nPROCESS\t|TURNAROUND TIME| WAITING TIME\n\n");
array[9]=9999;
for(TIme11=0;left!=n;TIme11++)
{
shortest=9;
for(i=0;i<n;i++)
{
if(arrival_TIme11[i]<=TIme11 && array[i]<array[shortest] && array[i]>0)
{
shortest=i;
}}
        
array[shortest]--;
if(array[shortest]==0)
{
left++;
Endt=TIme11+1;
printf("\nP[%d]\t|\t%d\t|\t%d",shortest+1,Endt-arrival_TIme11[shortest],Endt-Burst_TIme11[shortest]-arrival_TIme11[shortest]);
s_wiat+=Endt-Burst_TIme11[shortest]-arrival_TIme11[shortest];
s_turn_arn_d+=Endt-arrival_TIme11[shortest];
}
}
printf("\n\nAverage waiting TIme11 = %f\n",s_wiat*1.0/n);
printf("Average Turnaround TIme11 = %f",s_turn_arn_d*1.0/5);
return (0);
} 
