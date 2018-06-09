# note
MCU learning note

单片机最小系统：
1.	电源
2.	复位电路
3.	晶振电路
4.	单片机芯片

电阻读法，例：402 =40*102	

2018.6.9
C语言中i取值范围 0~65535

自定义函数： 延时函数delay（毫秒级）
void delay(unsigned int z)
{
    unsigned int x, y;
    for(x = z; x > 0; x-- )
        for(y = 114; y > 0 ; y--);
}

标准库函数： intrins.h
内部函数
字符型循环左移： _crol_
字符型循环右移： _cror_
#include <intrins.h>
void test_crol (void)
{
    unsigned char a
    unsigned char b
    a = 0xFE; // 11111110
    b = _crol_(a,1); // b now is 0xFD, 二进制形式11111101
}
