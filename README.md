#include<stdio.h>
#include<ctype.h>

//字符转换成数字
int Myatoi(const char *str)
{
	int tmp=0;
	while(isdigit(*str))
	{
		tmp=tmp*10+(*str-'0');
		str++;
	}
	return tmp;
}

int main()
{
  printf("%d\n",Myatoi("1234"));//字符串转换成数字测试用例
	printf("%d\n",Myatoi("12ab34"));//字符串转换成数字测试用例
	printf("%d\n",Myatoi("ab1234"));//字符串转换成数字测试用例
  
  return 0
}
