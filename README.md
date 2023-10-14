# Apo2
![Logo Java](https://seeklogo.com/images/J/java-logo-7833D1D21A-seeklogo.com.png)

# Apo2 Funciones.

Se crearon proyectos para dar soluciones a diferentes problemas de la vida contidiana en distintos ambitos. 

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

```
Este proyecto nos ayuda a solucinar operaciones primarias
Como resta, suma, multiicacion y division
Ingresando numeros por teclado

```

## Primer proyecto de java 
```
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


```
## Segundo proyecto en Java
```
// se importa la librería de scanner 
package ejercicio;
import java.util.Scanner;

// Dentro de la public class se crea el public static void main

public class pesosADolares {
	public static void main(String[]args).{

// Se muestra en pantalla el mensaje ingrese el valor en pesos

System.out.print("ingrese el valor de pesos: ");

// Se establece la variable dolares como un float, inicializa desde 0 y se le pide el valor al usuario

float dolares=0;
		float pesos=sc.nextFloat();

// Se establece la variable dolares, siendo la division de pesos entre 4150, es decir su conversion

dolares=(pesos/4150);

//Se muestra en pantalla la cantidad de pesos en dolares

System.out.print("la cantidad en dolares es: "+dolares);
}
}
```
## Tercer proyecto en Java
```
// Este programa permite obtener el promedio de n notas.
package clase;

import javax.swing.JOptionPane;

public class promedio {
	public static void main(String[]args) {
		
		// creamos la contenedora Array y pedimos las notas con JOptionPane
		double [] Array = new double[3];
		JOptionPane.showMessageDialog(null, "Ingresa una nota");
		Array [0] = Double.parseDouble(JOptionPane.showInputDialog(null, "Ingrese un numero"));
		JOptionPane.showMessageDialog(null, "Ingresa una nota");
		Array [1] = Double.parseDouble(JOptionPane.showInputDialog(null, "Ingrese un numero"));
		JOptionPane.showMessageDialog(null, "Ingresa una nota");
		Array [2] = Double.parseDouble(JOptionPane.showInputDialog(null, "Ingrese un numero"));
		// definimos la varibale suma como un double.
		double suma;
		// definimos la variable promedio como un double.
		double promedio;
		// establecemos suma como array0+array1+array2.
		suma = Array[0]+Array[1]+Array[2];
		// establecemos promedio como el resultado de suma divido en 3.
		promedio = suma/3;
		// con JOptionPane mostramos el resultado del promedio
		JOptionPane.showMessageDialog(null, "El promedio es de: " + promedio);
	
	} 

}


```
## Cuarto proyecto en Java
// Este programa permite obtener el promedio de distintas notas e identificar la nota minima y maxima.
```
// primero se importa el JOptionPane con la correspondiente clase 

Import javax.swing.JOptionPane;

public class Asignaturas {
	// Se define la variable notas brindando la opción de que el usuario ingresé la cantidad de notas requerida 

	public static void main(String[] args) {

	//Auto-generated method stub
		int totalNotas= Integer.parseInt(JOptionPane.showInputDialog(null, "Ingresa el número de notas: "));
	// Definimos las contenedoras en el proceso para hacer el promedio de notas

    double notas [] = new double [totalNotas];
	// El primer paso es realizar la suma de las notas ingresadas 

     double suma=0;
		for(int i=0; i<totalNotas;i++) {

			// El usuario por teclado Ingresa las notas 
        notas[i]=Double.parseDouble(JOptionPane.showInputDialog(null, "Ingresa tus  notas: \n"));
		suma=suma+notas[i];

		}

		// Se establece en el programa la nota máxima 

        double notaMax=notas[0];
		for(int i=0; i<notas.length;i++) {
			if (notas[i] > notaMax) {
	                notaMax = notas[i];
			}
		}

		JOptionPane.showMessageDialog(null, "Tu nota máxima es: "+notaMax,"Max", 1);

		// Definimos en el programa la nota mínima 

		double notaMin=notas[0];
		for(int i=0; i<notas.length;i++) {
			if (notas[i] < notaMin) {
				notaMin = notas[i];
			}
		}

		JOptionPane.showMessageDialog(null, "Tu nota mínima es: "+notaMin,"Min", 0);

		// Con los datos registrados se realiza la suma y la división total de notas 

        double promedio;
		promedio=suma/totalNotas;

		// Se agrega la restricción con if para el mensaje de respronaste el promedio con menor de 0

        if (promedio<=29)
			JOptionPane.showMessageDialog(null, "Repobraste, tu promedio es: "+promedio,"Promedio", 0);
			
		else
		// Con esta opción se entiende los parámetros de la aprobación de la materia 

        JOptionPane.showMessageDialog(null, "Aprobaste, tu promedio es: "+promedio,"Promedio", 1);		
		
	}

}


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
## Construido con

Eclipse IDE for Java

## Versionado

Version de Eclipse IDE for Java Developers-2023-06

## Autores

* **Juan Zambrano**
* **Danna Lagos**
* **Anyeli Jaramillo** 


## Licencia

Este proyecto tiene la licencia MIT; consulte el archivo LICENSE.md para obtener más detalles.

## Expresiones de gratitud (Acknowledgments)

- Nos gustaria agradecer al profesor Gustavo Willyn Sánchez Rodriguez por haber hecho posible el correcto funcionamiento de este repositorio gracias a sus enseñanzas.
- Espero el contenido del repositorio haya sido util para resolver algunos problemas de la vida cotidiana