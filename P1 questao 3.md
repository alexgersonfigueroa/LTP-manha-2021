#include <stdio.h> 

int main() 
{
	int e_var_A,e_var_B,invert_var_A, invert_var_B;
	printf("favor entrar com variavel A:\t");
	scanf("%i", &e_var_A);
	printf("favor entrar com variavel b:\t");
	scanf("%i", &e_var_B);

	invert_var_A = e_var_B;
	invert_var_B = e_var_A;

	printf("Resultado Programação: %i,%i,%i,%i",e_var_A,e_var_B,invert_var_A,invert_var_B);
	
    return 0;
}
