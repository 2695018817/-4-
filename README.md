实验四 循环结构程序设计
一、实验目的
1、熟悉用 while 语句，do-while 语句和 for 语句实现循环的方法。
2、掌握在程序设计中用循环的方法实现各种算法（如穷举、迭代、递推等）。
3、掌握 continue 语句和 break 语句的使用。
4、熟练掌握循环结构的嵌套。
5、练习调试与修改程序。
二、实验准备
1、复习 while、do-while 和 for 语句的特点和适用条件。
2、复习 break 和 continue 的区别。
三、实验内容
以下程序是用来计算 S=1+2+3+4+...+10，请更正以下程序的错误，并上机调试。
1、
#include<stdio.h>
void main()
{
int i=1;
while(i<10)
sum+=i;
++i;
printf(“sum=%d\n”,sum);
}
修改后的程序为：

![YWZ) S58KUH$AG16H0CE}BQ](https://github.com/user-attachments/assets/defa806f-aede-492c-93bf-1995b84848a1)
2、
#include <stdio.h> 
void main()
{
int i=sum=0;
do{
sum+=i;
++i;
}while (i<10)
printf("sum=%d\n",sum);
修改后的程序为：
#include <stdio.h> 
int main() {
	int i = 0,sum = 0;
	do {
		sum += i;
		++i;
	} while (i < 10);
	printf("sum=%d\n", sum);
	return 0;
}
![1 671PUNSEDN`6OV P 8)XT](https://github.com/user-attachments/assets/92bbe2e4-3715-4004-bf45-455498f15c96)
3、
#include <stdio.h>
void main()
{
int i=sum=0;
do{
sum+=i;
++i;
}while(i<10)
printf ("sum=%d\n" ,sum);
}
修改后的程序为：
#include <stdio.h>
void main()
{
	int i = 0,sum = 0;
	do {
		sum += i;
		++i;
	} while (i < 10);
		printf("sum=%d\n", sum);
		return 0;
}
![}4OM$4)`$42``M6SVQ5} (B](https://github.com/user-attachments/assets/8e52db7f-503f-4b14-9492-5881d9b8424f)
4、输入并运行下面的程序，观察程序的运行结果。
#include <stdio.h>
void main()
{
int n;
while (1)
{
printf("'Enter a number:");
scanf ("%d" ‚n);
if (n%2==1)
{
printf("I said");
continue;
} break;
}
printf("Thanks. I needed that！");
}
修改后的程序为：
#include <stdio.h>
int main()
{
	int n;
	while (1)
	{
		printf("'Enter a number:");
		scanf_s("%d" ,&n);
		if (n % 2 == 1)
		{
			printf("I said");
			continue;
		} 
		else {
			break;
		}
	}
	printf("Thanks. I needed that！");
	return 0;
}
![V~R$UJ_7USBP%OA{~T{~_QF](https://github.com/user-attachments/assets/89f79870-290a-4bc5-a3f3-af28ef207ec0)
