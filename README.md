# Roman-System
//sum and multiplication in binary
#include <stdio.h> 
int display(int);
int main() 
{   
    int num1,num2,sum,product;
    
    printf("Enter two numbers: ");
    scanf("%d %d", &num1,&num2);
    sum = num1+num2;
    product = num1*num2;
    printf("In arabic system,sum=%d",sum);
    printf("\nIn roman system,sum=");
    
    display(sum);
    printf("\n\nIn arabic system,product=%d",product);
    printf("\nIn roman system,product=");
    display(product);
}
int display(int num)
{
    while(num != 0)
    {

        if (num >= 1000)       // 1000 - m
        {
           printf("m");
           num -= 1000;
        }

        else if (num >= 900)   // 900 -  cm
        {
           printf("cm");
           num -= 900;
        }        

        else if (num >= 500)   // 500 - d
        {           
           printf("d");
           num -= 500;
        }

        else if (num >= 400)   // 400 -  cd
        {
           printf("cd");
           num -= 400;
        }

        else if (num >= 100)   // 100 - c
        {
           printf("c");
           num -= 100;                       
        }

        else if (num >= 90)    // 90 - xc
        {
           printf("xc");
           num -= 90;                                              
        }

        else if (num >= 50)    // 50 - l
        {
           printf("l");
           num -= 50;                                                                     
        }

        else if (num >= 40)    // 40 - xl
        {
           printf("xl");           
           num -= 40;
        }

        else if (num >= 10)    // 10 - x
        {
           printf("x");
           num -= 10;           
        }

        else if (num >= 9)     // 9 - ix
        {
           printf("ix");
           num -= 9;                         
        }

        else if (num >= 5)     // 5 - v
        {
           printf("v");
           num -= 5;                                     
        }

        else if (num >= 4)     // 4 - iv
        {
           printf("iv");
           num -= 4;                                                            
        }

        else if (num >= 1)     // 1 - i
        {
           printf("i");
           num -= 1;                                                                                   
        }

    }

    
}
