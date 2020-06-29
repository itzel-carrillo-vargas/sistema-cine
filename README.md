# sistema-cine
actividad
#include <iostream>
#define Tope_20
 
using namespace std;
 
void menu();
void ventaEntradas();

struct clientes {
    string codigo;
    int cantidad;
    int salas;
    int tope;
} clientes;
 
 void menu();
 void venta_de_dulceria();
 
 struct dulceria{
 	int palomitas;
 	int bebidas;
 	int dulces;
 	int combos ;
 }dulceria;
 
int i=0;
 
int main() {
    menu();
    return 0;
}
 
//Funciones
void menu() {
    int opc;
 
    do {
        printf( "\n******************************" );
        printf("\n****** Menu de Opciones ******" );
        printf( "\n******************************" );
        printf("\n1. Venta de entradas" );
        printf( "\n2. Total Ingresos" );
        printf( "\n3. Dulceria" );
        printf("\n4. salir");
        printf( "\nSeleccione su opcion: ");
        scanf("%d",& opc);
 
        switch (opc) {
            case 1:
                ventaEntradas();
            break;
            case 2:
                //totalIngresos();
            break;
            case 3:
            	venta_de_dulceria();
            break;
        }
 
    } while (opc < 4);
 
}
 
//-----------------------------------------
void ventaEntradas() {
	
  {
        printf( "Codigo del cliente: ");
        scanf("%d" ,& clientes.codigo);
        printf("Cantidad de entradas: ");
        scanf("%d" ,&clientes.cantidad);
        printf( "Sala Nro: ");
        scanf("%d" ,& clientes.salas);
        
        printf( "Cliente registrado con exito");
    }
    
void venta_de_dulceria(){
	
  {  
  
        printf( "pedido del  cliente: ");
        scanf("%d" ,& cliente );
        printf("palomitas: ");
        scanf("%d" ,& dulceria.palomitas);
        printf( "bebidas ");
        scanf("%d" ,& dulceria.bebidas);
        printf( "dulceria ");
        scanf("%d" ,& dulceria.dulces);
        printf( "combos ");
        scanf("%d" ,& dulceria.combos);
        printf( "Cliente registrado con exito");
    }
}
