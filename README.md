# Apo2
![Logo Java](https://seeklogo.com/images/J/java-logo-7833D1D21A-seeklogo.com.png)

# Apo2 Funciones.

Se creo en eclipse un programa que le pide al usuario ingresar dos numero enteros para con estos valores multiplicar, resta, dividir y sumar.  

## Empezando

Estas instrucciones le permitirán obtener una copia del proyecto en funcionamiento en su máquina local para fines de desarrollo y prueba. Consulte implementación para obtener notas sobre cómo implementar el proyecto en un sistema en vivo.

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

Termine con un ejemplo de cómo sacar algunos datos del sistema o usarlos para una pequeña demostración.

## Ejecutando las pruebas

Explicar cómo ejecutar las pruebas automatizadas para este sistema.

### Dividir en pruebas de principio a fin

Explique qué prueban estas pruebas y por qué.

```
Este proyecto nos ayuda a solucinar operaciones primarias
Como resta, suma, multiicacion y division
Ingresando numeros por teclado
```

### Y pruebas de estilo de codificación.


Explique qué prueban estas pruebas y por qué.

```
package proyecto;

import javax.swing.JOptionPane;
//se importa una nueva libreria que permite ingresar datos de manera manual

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
//define z como resta y esta misma como un valor entero
		int m=multiplicacion(x,y);
//define m como multiplicacion y esta misma como un valor entero
		int d=division(x,y);
//define m como division y esta misma como un valor entero
		JOptionPane.showMessageDialog(null,"El total de la suma es: " + t ,"suma",1);
		JOptionPane.showMessageDialog(null,"El total de la resta es: " + z,"resta",1);
		JOptionPane.showMessageDialog(null,"El total de la multiplicacion es: " + m,"multiplicacion",1);
		JOptionPane.showMessageDialog(null,"El total de la division es: " + d,"division",1);
//Se muestra un mensaje de lo que hara el programa
	}
		public static int suma(int a,int b) {
			return a+b;
// esto permite hacer la operacion y llamar en los parametos para pder generar la suma 
		}
		
		public static int resta(int x,int y) {
			return x-y;
// esto permite hacer la operacion y llamar en los parametos para pder generar la resta
			
		}
		public static int multiplicacion(int a,int b) {
			return a*b;
// esto permite hacer la operacion y llamar en los parametos para pder generar la multiplicacion 
	}
		public static int division(int a,int b) {
			return a/b;
// esto permite hacer la operacion y llamar en los parametos para pder generar la division
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
