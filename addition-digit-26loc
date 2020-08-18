#include <stdio.h>
#include <stdlib.h>
#include <limits.h>



int checkInput(char MSG[], int MIN, int MAX)
{
    int n, check;
    char ch;
    do
    {
        printf(MSG);
        fpurge(stdin);
        check = scanf("%d%c", &n, &ch);
        if ((check == 2) && (ch == '\n'))
            {
                if (n > MIN && n <= MAX)
                    break;
                else
                {
                    printf("Please enter a decimal number");
                    continue;
                }
            }
        else
        {
            printf("Please enter a decimal again");
            continue;
        }
    } while (1);
    return n;
}

int main(int argc, char** argv)
{
    int n = checkInput("Enter an digit: ", 0, INT_MAX);
    printf("\n");
    int *a = (int *)malloc(n * sizeof(int));
    int sum = 0;
    while (n != 0)
    {
        sum = sum + n % 10;
        n = n / 10;
    }
    printf("Sum Digit = %d", sum);
    return 0;
}
