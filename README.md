# 05-pi-to-the-nth-digit-alechavez26
05-pi-to-the-nth-digit-alechavez26 created by GitHub Classroom
/*
 * Alejandra Chávez Cruz
 * A01411970@itesm.mx
 * 7/sept/18
 */

#include <stdio.h>
#include <math.h> // This library includes the pow function

int main() {

    //Declare the variables
    double pi;
    int v;

    pi=0;

    printf("Write how many decimals do you want ");
    scanf("%d", &v);


    for (int a=0; a<=v; a++) {

        //Keep the values in pi
        pi+=((pow(16,-a))*(4/(8.0*a+1)-2/(8.0*a+4)-1/(8.0*a+5)-1/(8.0*a+6)));
    }


    printf("%.*f", v, pi);

    return 0;
}
