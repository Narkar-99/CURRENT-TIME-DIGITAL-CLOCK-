# CURRENT-TIME-DIGITAL-CLOCK-
#include<stdio.h>
#include<time.h>
#include<conio.h>
void main()
{  time_t now;
 struct tm *tm_now;
int hour,min,sec;
while(1)
{ system("clear");
now=time(NULL);
 tm_now=localtime(&now);
hour=tm_now->tm_hour;
min=tm_now->tm_min;
sec=tm_now->tm_sec;
    printf("\n%d:%d:%d",hour,min,sec);
    sleep(1);
    }
    getch();
}
