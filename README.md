// Hacer una tabla que muestre las ventas de 100 productos en 12 meses.

#include<stdio.h>

struct inventario{
	char producto[20];
	int cantidad;
}productos[100][12];

int main () {
	int i;
	int j;
	for(i=0;i<99;i++){
		for(j=0;i<11;j++){
		   fflush(stdin);
	    	printf("%i. digite su producto: ", i+1);
	        gets(productos[i][j].producto);
        	printf("%i. digite su cantidad: ", i+1);
        	scanf("%i", &productos[i][j].cantidad);
        }
	}
	for(i=0;i<99;i++){
		for(j=0;i<11;j++){
		printf("\n%i. su proucto es: %s", productos[i][j].producto);
		printf("\n%i. la cantidad de productos que tiene es : %i", productos[i][j].cantidad);
		printf("\n");
	}
	}
	return 0;
}
