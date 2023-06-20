# Pro_carniceria
#PROMEDIO DE VENTAS CARNICERIA
***
 En su labor como programador de software ha sido elegido para el desarrollo de una aplicación que necesita un administrador de una carniceria, que desea calcular el promedio de ventas diarias de su negocio. Como información básica de cada cliente se debe registrar el numero de identificación, su nombre y la compra realizada.
\
**Aclaraciones:**
+ Se supondrá que la aplicación solo se requiere para calcular el promedio de un dia en especifico. 
+ Para efectos de mantener la simplicidad del ejemplo no se contemplan manejar persistencia en el almacenamiento de los datos. 
+ No se realiza validación, ni se verifica calidad en los datos ingresados 

**Historia de usuario**
\
![](https://github.com/jjlo21/Pro_carniceria/blob/main/2023-06-15%20(6).png?raw=true)

***
## CASO DE USO

**Nombre:** Calculador del Promedio de ventas diario
\
**Actores:** Administrador carniceria
\
**Propósito:** Guardar identificación, nombre, compra
\
**Curso Normal de Eventos:**
1. El Ferretero ingresa la cantidad de productos a evaluar.
2. El Ferretero ingresa la identificación, nombre, curso, y el valor del producto.
3. Se calcula el promedio a partir de:
( Σ(Precio del producto 1, Precio del producto 2, Precio del producto 3, Precio del producto n) / Total ventas) / Cantidad productos
4. Se Muestra el promedio de las ventas obtenidas
Postcondiciones: Promedio de ventas 
![](https://github.com/Deison12/Taller1.github.io/blob/f6ab787bf3e6a6cad4f5ac1c25dde117bc776b9e/Diagrama%20en%20blanco.png)

***
##Aproximación Seudocódigo
\
 Algoritmo Ferreteria
 
	Definir CantidadProductos Como Entero
	Definir promedio como real
	Escribir "INGRESE LA CANTIDAD DE PRODUCTOS A EVALUAR"
	Leer CantidadProductos
	Dimension  identificacion[CantidadProductos], nombres[CantidadProductos]
	Dimension  precio[CantidadProductos]		
	Para i=1 Hasta CantidadProductos Con Paso 1
		Escribir "INGRESE LA IDENTIFICACION DEL PRODUCTO " ,i
		Leer id
		identificacion[i] = id
		Escribir "INGRESE EL NOMBRE DEL PRODUCTO " ,i
		Leer name
		nombres[i] = mame
		Escribir "INGRESE EL VALOR DE VENTA DEL PRODUCTO " ,i
		Leer price
		precio[i] = price
	FinPara
	Para i=1 hasta CantidadProductos con paso 1
		promedio = promedio + precio[i] / CantidadProductos
				
	finPara
	
	Imprimir "El promedio de ventas es: ",promedio	
FinAlgoritmo
***


