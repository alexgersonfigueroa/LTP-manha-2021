#include <stdio.h> 

int main() 
{
	int e_nro_A,e_nro_B;
	printf("favor digitar valor 10 para primeiro numero:\t");
	scanf("%i", &e_nro_A);
	printf("favor digitar valor 20 para segundo numero:\t");
	scanf("%i", &e_nro_B);
	e_nro_A=e_nro_A*0+e_nro_B;
	e_nro_B=e_nro_B-10;

	printf("numeros impressos em ordem invertida: %d, %d",e_nro_A,e_nro_B);
	    
    return 0;
}
