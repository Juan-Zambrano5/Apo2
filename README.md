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
		int x=Integer.parseInt(JOptionPane.showInputDialog(null,"Ingrese el primer numero"));
		int y=Integer.parseInt(JOptionPane.showInputDialog(null,"Ingrese el segundo numero"));
		int t=suma(x,y);
		int z=resta(x,y);
		int m=multiplicacion(x,y);
		int d=division(x,y);
		JOptionPane.showMessageDialog(null,"El total de la suma es: " + t ,"suma",1);
		JOptionPane.showMessageDialog(null,"El total de la resta es: " + z,"resta",1);	
		JOptionPane.showMessageDialog(null,"El total de la multiplicacion es: " + m,"multiplicacion",1);
		JOptionPane.showMessageDialog(null,"El total de la division es: " + d,"division",1);
	}
		public static int suma(int a,int b) {
			return a+b;
			
		}
		
		public static int resta(int x,int y) {
			return x-y;
			
			
		}
		public static int multiplicacion(int a,int b) {
			return a*b;
	}
		public static int division(int a,int b) {
			return a/b;
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
