#include <stdio.h> 

int main()
{
	int genero_escolhido;
	float altura_,calc_masculino,calc_feminino;
	printf("Descubra Seu Peso Ideal\n");
	printf("Gênero Masculino - código 0.\n");
	printf("Gênero Feminino - código 1.\n");
	printf("Escolha seu gênero, numero 0 ou numero 1?\t");
	scanf("%i", &genero_escolhido);
	printf("favor digitar sua altura (em metros):\t");
	scanf("%f", &altura_);
		
	if (genero_escolhido == 0)
		{calc_masculino = ((altura_*72.7)-58);
		printf("peso ideal para o homem (Kg): %f",calc_masculino);}
	else
	    {if (genero_escolhido == 1)
	        {calc_feminino = ((altura_*62.1)-44.7);
			printf("peso ideal para a mulher (Kg): %f",calc_feminino);}
		else
		    {printf("Opção Gênero Inválido.\n");}}
    return 0;
}
