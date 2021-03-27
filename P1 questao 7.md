#include <stdio.h> 
#include <math.h> 

int main()
{
	int e_resist1,e_resist2,e_resist3,e_resist4,soma_invert,resultado_soma;


	
	printf("Programa de SOMA de RESISTORES em PARALELO\n");
	printf("Entre com valor Resistor 1\t");
	scanf("%i", &e_resist1);
	printf("Entre com valor Resistor 2\t");
	scanf("%i", &e_resist2);
	printf("Entre com valor Resistor 3\t");
	scanf("%i", &e_resist3);
	printf("Entre com valor Resistor 4\t");
	scanf("%i", &e_resist4);
		
resultado_soma = e_resist1 + e_resist2 + e_resist3 + e_resist4;

printf("Resultado Soma de Resistores em Paralelo (em ohms): %i",resultado_soma);
	
return 0;
}
