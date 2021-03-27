#include <stdio.h>
#include <math.h>
#include <conio.h>
int main()
{
	int material_escolhido,temperatura_uso;
	float diametro_cabo,comprimento_cabo,calc_prata,calc_cobre,calc_ouro,calc_aluminio,calc_tungstenio,calc_area,calc_ro,calc_resistividadeFio;
	printf("Lista de Cabos\n");
	printf("**************\n");
	printf("CODIGO     MATERIAL   \n");
	printf("******     ********\n");
	printf("  1         Prata\n");
	printf("  2         Cobre\n");
	printf("  3         Ouro\n");
	printf("  4         Alumínio\n");
	printf("  5         Tungstenio\n");
	printf("Digite o código do material desejado:\t");
	scanf("%i", &material_escolhido);
	printf("Digite diâmetro do cabo (mm):\t");
	scanf("%f", &diametro_cabo);
	printf("Digite comprimento do cabo (m):\t");
	scanf("%f", &comprimento_cabo);
	printf("Digite temperatura de uso do cabo (oC):\t");
	scanf("%i", &temperatura_uso);
			
	if (material_escolhido == 1)
		{calc_area = 3.141592654 * pow((diametro_cabo/2),2);
		calc_ro = 0.00000159 * (1 + 0.038 * ( temperatura_uso - 20));
		calc_resistividadeFio = (calc_ro*comprimento_cabo)/calc_area;
		printf("Resistividade do fio de Prata: %f",calc_resistividadeFio);}
	
	
	else
	    {if (material_escolhido == 2)
		{calc_area = 3.141592654*pow((diametro_cabo/2),2);
		calc_ro = 0.00000172 * (1+ 0.039 * (temperatura_uso- 20));
		calc_resistividadeFio = (calc_ro*comprimento_cabo)/calc_area;
		printf("Resistividade do fio de Cobre: %f",calc_resistividadeFio);}
	     else
		    {if (material_escolhido == 3)
		{calc_area = 3.141592654*pow((diametro_cabo/2),2);
		calc_ro = 0.00000244 * (1+ 0.034 * (temperatura_uso- 20));
		calc_resistividadeFio = (calc_ro*comprimento_cabo)/calc_area;
		printf("Resistividade do fio de Ouro: %f",calc_resistividadeFio);}
		    else
		   	 {if (material_escolhido == 4)
		{calc_area = 3.141592654*pow((diametro_cabo/2),2);
		calc_ro = 0.00000292 * (1+ 0.039 * (temperatura_uso- 20));
		calc_resistividadeFio = (calc_ro*comprimento_cabo)/calc_area;
		printf("Resistividade do fio de Aluminio: %f",calc_resistividadeFio);}
			  else
		  	 	 {if (material_escolhido == 5)
		{calc_area = 3.141592654*pow((diametro_cabo/2),2);
		calc_ro = 0.0000056 * (1+ 0.045 * (temperatura_uso- 20));
		calc_resistividadeFio = (calc_ro*comprimento_cabo)/calc_area;
		printf("Resistividade do fio de Tungstenio: %f",calc_resistividadeFio);}}
		   	 }}}
    return 0;
}
