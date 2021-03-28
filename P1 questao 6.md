#include <stdio.h>
#include <math.h>
#include <conio.h>

#define PI 3.14
#define ALFA_AG 0.038
#define ALFA_CU 0.039
#define ALFA_AU 0.034
#define ALFA_AL 0.039
#define ALFA_TG 0.045
#define RO_AG 1.59
#define RO_CU 1.72
#define RO_AU 2.44
#define RO_AL 2.92
#define RO_TG 5.6

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
			
	 
	if ((material_escolhido > 0) && (material_escolhido < 6))
	{switch (material_escolhido)
	{case 1: calc_area = PI * pow((diametro_cabo/2),2);
		calc_ro = (RO_AG *  (1 + ALFA_AG * ( temperatura_uso - 20)));
		calc_resistividadeFio = ((calc_ro*comprimento_cabo)/calc_area);
		printf("Resistividade do fio de Prata (micro Ohms): %.2f",calc_resistividadeFio);
		break;
	
	case 2: calc_area = PI * pow((diametro_cabo/2),2);
		calc_ro = (RO_CU *  (1 + ALFA_CU * ( temperatura_uso - 20)));
		calc_resistividadeFio = ((calc_ro*comprimento_cabo)/calc_area);
		printf("Resistividade do fio de Cobre (micro Ohms): %.2f",calc_resistividadeFio);
		break;

	case 3: calc_area = PI * pow((diametro_cabo/2),2);
		calc_ro =( RO_AU *  (1 + ALFA_AU * ( temperatura_uso - 20)));
		calc_resistividadeFio = ((calc_ro*comprimento_cabo)/calc_area);
		printf("Resistividade do fio de Ouro (micro Ohms): %.2f",calc_resistividadeFio);
		break;

	case 4: calc_area = PI * pow((diametro_cabo/2),2);
		calc_ro = (RO_AL *  (1 + ALFA_AL * ( temperatura_uso - 20)));
		calc_resistividadeFio = ((calc_ro*comprimento_cabo)/calc_area);
		printf("Resistividade do fio de Aluminio (micro Ohms): %.2f",calc_resistividadeFio);
		break;

	case 5: calc_area = PI * pow((diametro_cabo/2),2);
		calc_ro =( RO_TG *  (1 + ALFA_TG * ( temperatura_uso - 20)));
		calc_resistividadeFio = ((calc_ro*comprimento_cabo)/calc_area);
		printf("Resistividade do fio de Tungstenio (micro Ohms): %.2f",calc_resistividadeFio);
		break;}

	
		
	}else{  printf("*******CODIGO MATERIAL INVALIDO*******");
		}
	    
	
		   	 		  	 	
    return 0;
}
