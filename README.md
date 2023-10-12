# Apo2
![Logo Java](https://seeklogo.com/images/J/java-logo-7833D1D21A-seeklogo.com.png)

# Apo2 Funciones.

Se creo en eclipse los trees proyectos siguientes 

## Empezando

Estas instrucciones le permitirán obtener una copia del proyecto en funcionamiento en su máquina local para fines de desarrollo y prueba

### Requisitos previos

Instalar Eclipse en tu computador

```
Link de instalación de Eclipse: https://www.eclipse.org/downloads/
```

### Instalación

Importar la libreria JOptionPane.


```
import javax.swing.JOptionPane es para que funcione JOptionPane
```

## Ejecutando las pruebas

```
Para ejecutar las pruebas, debemos darle control+f11 para iniciar la aplicación.
```

### Dividir en pruebas de principio a fin


// Este proyecto nos ayuda a solucinar operaciones primarias
Como resta, suma, multiicacion y division
Ingresando numeros por teclado

```
// Se agrego el primer proyecto de java 

Package proyecto;

import javax.swing.JOptionPane;

public class proyecto3 {
	public static void main(String[]args) {

// Con el siguiente paso podemos establecer el proceso de que el usuario ingrese los numeros entreros que desea operar 

JOptionPane.showMessageDialog(null,"Digite un valor\n");
		int x=Integer.parseInt(JOptionPane.showInputDialog(null,"Ingrese el primer numero"));
		int y=Integer.parseInt(JOptionPane.showInputDialog(null,"Ingrese el segundo numero"));

// Se define suma, resta, multiplicacion y division como valores enteros
		int t=suma (x,y)
		int z=resta(x,y);
		int m=multiplicacion(x,y);
		int d=division(x,y);
		

// ShowMessageDialog se lo utiliza para poder enviar un mensaje al usuario 

JOptionPane.showMessageDialog(null,"El total de la suma es: " + t ,"suma",1);
		JOptionPane.showMessageDialog(null,"El total de la resta es: " + z,"resta",1);	
		JOptionPane.showMessageDialog(null,"El total de la multiplicacion es: " + m,"multiplicacion",1);
		JOptionPane.showMessageDialog(null,"El total de la division es: " + d,"division",1);
// Se llama a cada una de las operaciones dando su total 

	}

// Se realiza la operacion de los numeros ingresados por el usuario que es suma
		public static int suma(int a,int b) {
			return a+b;
			
		}
// Se realiza la operacion de los numeros ingresados por el usuario que es resta
		public static int resta(int x,int y) {
			return x-y;
			
			
		}
// Se realiza la operacion de los numeros ingresados por el usuario que es la multiplicacion
		public static int multiplicacion(int a,int b) {
			return a*b;
	}
// Se realiza la operacion de los numeros ingresados por el usuario para hacer la division 
		public static int division(int a,int b) {
			return a/b;
}
}



// segundo proyecto

// se importa la librería de scanner 
package ejercicio;
import java.util.Scanner;

// Dentro de la public class se crea el public static void main

public class pesosADolares {
	public static void main(String[]args){
		
```

### Y pruebas de estilo de codificación.

``` 
package proyecto;

import javax.swing.JOptionPane;
//Se importa una nueva libreria que permite ingresar datos de manera manual

public class proyecto3 {
	public static void main(String[]args) {
		JOptionPane.showMessageDialog(null,"Digite un valor\n");
//Se muestra un mensaje de lo que hara el programa
		int x=Integer.parseInt(JOptionPane.showInputDialog(null,"Ingrese el primer numero"));
//Se pide al usuario que ingrese un valor entero
		int y=Integer.parseInt(JOptionPane.showInputDialog(null,"Ingrese el segundo numero"));
//Se pide al usuario que igrese el segundo valor entero
		int t=suma(x,y);
//Se define t como suma y esta misma como un valor entero
		int z=resta(x,y);
//Define z como resta y esta misma como un valor entero
		int m=multiplicacion(x,y);
//Define m como multiplicacion y esta misma como un valor entero
		int d=division(x,y);
//Define m como division y esta misma como un valor entero
		JOptionPane.showMessageDialog(null,"El total de la suma es: " + t ,"suma",1);
		JOptionPane.showMessageDialog(null,"El total de la resta es: " + z,"resta",1);
		JOptionPane.showMessageDialog(null,"El total de la multiplicacion es: " + m,"multiplicacion",1);
		JOptionPane.showMessageDialog(null,"El total de la division es: " + d,"division",1);
//Se muestra un mensaje de lo que hara el programa
	}
		public static int suma(int a,int b) {
			return a+b;
//Esto permite hacer la operacion y llamar en los parametos para poder generar la suma 
		}
		
		public static int resta(int x,int y) {
			return x-y;
//Esto permite hacer la operacion y llamar en los parametos para poder generar la resta
			
		}
		public static int multiplicacion(int a,int b) {
			return a*b;
//Esto permite hacer la operacion y llamar en los parametos para poder generar la multiplicacion 
	}
		public static int division(int a,int b) {
			return a/b;
//Esto permite hacer la operacion y llamar en los parametos para poder generar la division
}
}

```

## Despliegue (Deployment)

Agregue notas adicionales sobre cómo implementar esto en un sistema en vivo


## Construido con

Dropwizard : el marco web utilizado
Maven - Gestión de dependencias
ROMA : se utiliza para generar canales RSS

## Versionado

Usamos Git para el control de versiones. Para conocer las versiones disponibles, consulte las etiquetas en este repositorio .

## Autores

* **Juan Zambrano**
* **Danna Lagos**
* **Anyeli Jaramillo** 


## Licencia

Este proyecto tiene la licencia MIT; consulte el archivo LICENSE.md para obtener más detalles.

## Expresiones de gratitud (Acknowledgments)


* Un consejo para cualquiera cuyo código se haya utilizado
* Inspiración
* etc
