# Project-1
LCD interface
#include<reg51.h>
void delay (void);
sbit led1=P1^1;
sbit led2=P1^2;
void main()
{
	led1=0;
	led2=0;
	while(1)
	{
		led1=1;
		led2=0;
		delay();
		led1=0;
		led2=1;
		delay();
	}
}
void delay (void)
{
	int i,j;
	for (i=0;i<500;i++)
	for (j=0;j<500;j++);
