# code-
#include <stdio.h>

int main()
{
    char a[100]="sjhdcbdd$fffbhhg;hhggj$hdvj;hf";
    for(int i=0;i<100;i++)
    {
        if (a[i]=='$')
        {
            for (int k=i;k<=100;k++)
            {
                if(a[k]=='$')
                break;
            }
            
            for(int j=i;j<100;j++)
            {
                if(a[j]!=';')
                {
            printf("%c",a[j]);
                }
                else
                {
                    printf(";");
                    break;
                }
            }
        }
    }

    return 0;
}
