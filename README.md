# 3.5
求解简单的四则运算表达式
#include <stdio.h>
main()
{
    double value1, value2;
    char operator;
    printf("Type in an expression: ");    /* 提示输入一个表达式 */
    scanf("%lf%c%lf", &value1, &operator, &value2);
    switch(operator)
    {
        case '+': 
            printf("%.2f\n", value1+value2);
            break;
        case '-': 
            printf("%.2f\n", value1-value2);
            break;
        case '*': 
            printf("%.2f\n", value1*value2);
            break;
        case '/': 
            printf("%.2f\n", value1/value2);
            break;
        default:  
            printf("Unknown operator\n");
            break;
    }

    getch();
}
