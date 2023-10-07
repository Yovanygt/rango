<h3>Ejercicio 3: en estadística descriptiva, se define el rango de un conjunto de datos reales como la
diferencia entre el mayor y el menor de los datos.

Por ejemplo, si los datos son: [5.96, 6.74, 7.43, 4.99, 7.20, 0.56, 2.80], entonces el rango es 7.43 − 0.56
= 6.87
Escriba un programa que
a) Pregunte al usuario cuántos datos serán ingresados
b) Pida al usuario ingresar los datos uno por uno, y Entregue como resultado el rango de los datos.</h3>


<h1>c++</h1>

``````c++
#include<iostream>
#include<limits>
using namespace std;
int main(){
	int datos;
	
	double minimo = numeric_limits<double>::infinity(); // Inicializar con un valor positivo infinito
	double maximo = -numeric_limits<double>::infinity(); // Inicializar con un valor negativo infinito

		cout<<"Cuantos desea ingresar  ";
		cin>>datos;
		
		for(int i=0; i < datos; i++){
			double numeros;
			cout<<"ingrese el dato   " <<i+1 <<"   :    ";
			cin>>numeros;
				if(	numeros <minimo){
			minimo=numeros;
		}
	
		if(numeros > maximo){
			maximo=numeros;
		}
	
	}
		double rango = maximo-minimo;
			cout<<"El rango de los datos ingresados es   " <<rango <<endl;			
	return 0;
}
``````

<H1>PHYTON</H2>

``````C++
import sys

datos = int(input("Cuantos desea ingresar: "))

minimo = sys.float_info.max  # Inicializar con un valor máximo en punto flotante
maximo = -sys.float_info.max  # Inicializar con un valor mínimo en punto flotante

for i in range(datos):
    numeros = float(input(f"Ingrese el dato {i + 1}: "))
    
    if numeros < minimo:
        minimo = numeros
    
    if numeros > maximo:
        maximo = numeros

rango = maximo - minimo
print(f"El rango de los datos ingresados es: {rango}")
#   r a n g o  
 