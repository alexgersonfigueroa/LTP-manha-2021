#include <stdio.h>

int main() 
{ 
  int e_nro_1,e_nro_2,e_nro_3; 
  printf("favor entrar com primeiro numero:\t"); 
  scanf("%i", &e_nro_1); 
  printf("favor entrar com segundo numero:\t"); 
  scanf("%i", &e_nro_2); 
  printf("favor entrar com terceiro numero:\t"); 
  scanf("%i", &e_nro_3); 
  if (e_nro_1 > e_nro_2) 
    { if (e_nro_2 > e_nro_3) 
    {printf("numeros ordem crescente: %d, %d, %d",e_nro_3,e_nro_2,e_nro_1);
  }else{ 
    if (e_nro_1 > e_nro_3) {printf("numeros ordem crescente: %d, %d, %d",e_nro_2,e_nro_3,e_nro_1);
      }else{ 
      printf("numeros ordem crescente: %d, %d, %d",e_nro_2,e_nro_1,e_nro_3);
      } } 
   }else{ 
      if(e_nro_1 > e_nro_3){ printf("numeros ordem crescente: %d, %d, %d",e_nro_3,e_nro_1,e_nro_2); 
      }else{ 
        if (e_nro_2 > e_nro_3){ printf("numeros ordem crescente: %d, %d, %d",e_nro_1,e_nro_3,e_nro_2); 
         }else{
        printf("numeros ordem crescente: %d, %d, %d",e_nro_1,e_nro_2,e_nro_3);
      } 
    } 
  } 
  return 0;
  }
