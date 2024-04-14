#include <stdio.h>

int main(){
int numeros[10];
int repetidos[10];
int x;
int resto;
int reverso=0;
int soma=0;
int mediana=0;
int posicao=0;
int ordem=0;
int substituinte;
int repete= 1 ;
  
printf ("digite 10 numeros");
  for (int i =0; i<10; i++) {


scanf ("%d", &numeros[i]);
    }
printf ("escolha um caso de 0 a 14");
  scanf ("%d", &x);



switch(x) {
case 0:
    break;
case 1:
   printf ("digite uma posicao");
    scanf( "%d", &posicao);
  printf ("digite o numero p substituir");
  scanf ( "%d", &substituinte);
  for (int i =0; i<10; i++) {
    if (i==(posicao-1)) {
      numeros[i] = substituinte;
    }
    
  }
    for (int i =0; i<10; i++){
      printf ("%d", numeros[i]);
    }
  break;
case 2:
    for (int i=0; i<10; i++) {
        printf ("%d", numeros[i]);
    }
    break;
case 3:
  
   for (int i=9; i>=0; i--){
     // o ultimo numero é esta na posicao 9
     printf ("%d", numeros[i]);
     }

  
    break;

case 4:
    for (int i=0; i<10; i++) {
    soma = soma + numeros[i];
      }
  printf("%d", soma);
    break;

  case 5: 
  for (int i=0; i<10; i++) {
    for (int j=i+1; j<10; j++) {
    if (numeros[i]== numeros[j]) {
      posicao++;
    }
    }
    }
    printf ("%d", posicao);
  break; 

  case 6: 
  for (int i=0; i<10; i++) {
  for (int j=i+1; j<10; j++) {
  if (numeros[i] != numeros[j]) {
    printf ("%d", numeros[i]);
  }
  }
  }
break ;

    
  case 7: 
    for (int i=0; i<10; i++) {
      repete=1;
    for (int j=i+1; j<10; j++) {
      if (numeros[i]==numeros[j]) {
        repete++;
      }
    }
      printf ("%d- %d\n", numeros[i], repete);
    }

  break;
  case 8:
  for (int i=0; i<10; i++) {
    for (int j=i+1; j<10; j++) {
      if (numeros[i]>numeros[j]) {
        ordem=numeros[j];
        numeros[j]=numeros[i];
        numeros[i]=ordem;

      // valor minimo= num i [0]
      // valor maximo = num j [9]
      // valor medio= num [5]
        
        }
    
      }
        }
    printf("minimo-%d\n maximo-%d\n medio-%d", numeros [0], numeros[9], numeros[5]);
    
  break;
case 9:
    mediana= (numeros[4] + numeros[5])/2;
    printf("%d",mediana);
    break;

case 10:
    for (int i=0; i<10; i++) {
      for (int j=i+1; j<10; j++) {
        if (numeros[i]>numeros[j]) {
          ordem=numeros[i];
          numeros[i]=numeros[j];
          numeros[j]=ordem;
                }
              }
            }
      for (int i=0; i<10; i++){
        printf ("%d", numeros[i]);
            }
              break;
  case 11:
  for(int i=0; i<10; i++){
    for (int j=i+1; j<10; j++) {
      if (numeros[i]<numeros[j]) {
        ordem=numeros[j];
        numeros[j]=numeros[i];
        numeros[i]=ordem;
      }
    }
  }
  for (int i=0; i<10; i++) {
    printf ("%d\n", numeros[i]);
  }

 case 12: 
 for (int i = 0; i < 10; i++) {
   if (numeros[i] % 2 == 0 && numeros[i] != -1) {
       printf("PARES %d\n", numeros[i]);
       numeros[i] = -1; // p nao repetir
   }
 }
 for (int i = 0; i < 10; i++) {
   if (numeros[i] % 2 != 0 && numeros[i] != -1) {
       printf("IMPARES %d\n", numeros[i]);
       numeros[i] = -1; // p n repetir
   }
 }
   break;
   default:
   printf("invalido\n");
       }

       return 0;
   }





