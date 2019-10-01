# Prueba1
#include<stdio.h>
#include<stdlib.h> 
#include<conio.h> 
#include<time.h> 
int main( )
{
 // Declaracion de variables
 int numero,cantidad,contador;
 int hora = time(NULL);
 char x;
 do
  {
  
 // numero base para srand();
 srand(hora);
 
 /* cantidad de numeros que quiere el usuario */
 
 printf("Ingrese la cantidad de numeros aleatorios que desea generar\n");
 scanf("%d",&cantidad);
 
 /* Bucle */
 
 for(contador = 0; contador<cantidad; contador++)
 {
 
 numero = rand()%100;
 printf("%d \n", numero);
 }
  printf("Desea continuar y/n? \n");
 scanf("%c",&x);
 getch(); 
 system("cls");
 } while (x = "y");
}
