# Tribonacci

#include <stdio.h>

int main(void)
{
    int array[20];
    array[0] = 0;
    array[1] = 0;
    array[2] = 1;

    for(int i = 3; i < 20; i++)
    {
        array[i] = array[i - 1] + array[i - 2] + array[i - 3];
    }

    for(int i = 0; i < 20; i++)
    {
        printf("%d ", array[i]);
    }
    
    return 0;
}
