# Desarrollando la lógica de programación

## ¿Qué es un algoritmo?

Es una serie finita de pasos para resolver un problema.

Siempre que se desee resolver un problema hay que plantearse qué algoritmo utilizar. La respuesta a esta cuestión puede depender de numerosos factores, a saber, el tamaño del problema, el modo en que está planteado y el tipo y potencia del equipo disponible para su resolución.

## Características de un algoritmo

1. **Entrada:** definir lo que necesita el algoritmo.
2. **Salida:** definir lo que produce.
3. **No ambiguo:** explícito, siempre sabe qué comando ejecutar.
4. **Finito:** el algoritmo termina en número finito de pasos.
5. **Correcto:** hace lo que se supone que debe hacer.
6. **Efectividad:** cada instrucción se completa en tiempo finito. Cada instrucción debe ser lo suficientemente básica como para que pueda ser ejecutada por cualquier persona usando papel y lápiz.
7. **General:** debe ser lo suficientemente general como para contemplar todos lo casos de entrada.

<img src="C:\Users\Wilder z'A\Downloads\algoritmos.png" style="zoom: 40%;" />

## Formulación y resolución de problemas

Los algoritmos son los procedimientos que se construyen para la resolución de cualquier problema. De este modo, cuando se refiere al desarrollo de un programa, nos estamos refiriendo a la construcción de un algoritmo.

Los algoritmos los ejecutamos a lo largo de nuestras actividades diarias; por ejemplo, cuando hacemos una llamada telefónica, tenemos en cuenta un conjunto de instrucciones mínimas y el orden en el cual debemos ejecutarlas para conseguir comunicarnos con alguien en particular; o cuando consultamos un diccionario, cuando se prepara un menú, entre otros.

## Pasos para la solución de un problema

* **Definición del problema:** debe tenerse un enunciado entendible.
* **Análisis del problema:** se hace el planteamiento matemático y lógico de la solución del problema, por lo tanto es necesario identificar los datos de entrada, los datos de salida y el proceso que debe realizarse.
* **Crear el algoritmo:** hacer una descripción de los pasos lógicos que dan solución al problema, hasta obtener los resultados requeridos.
* **Prueba de escritorio:** permite detectar los posibles errores que se presenten en el algoritmo.

## Tipos de datos

|  Nombre  |                         Significado                          |                           Ejemplo                            |
| :------: | :----------------------------------------------------------: | :----------------------------------------------------------: |
|  Entero  | Es aquel que puede tomar por valor un número perteneciente al conjunto de los números enteros (Z), el cual está formado por los números naturales, su opuestos (números negativos) y el cero. |        La edad de una persona y el año de nacimiento.        |
|   Real   | Es aquel que puede tomar por valor un número perteneciente al conjunto de los números reales (R), el cual está formado por los números racionales e irracionales. |                    El peso y la estatura.                    |
|  Lógico  | Es aquel que puede tomar un valor (verdadero o falso) ya que representan el resultado de una comparación entre otros datos (numéricos o alfanuméricos). |                                                              |
| Carácter | Es aquel que puede tomar por valor un símbolo perteneciente al conjunto de los caracteres que puede representar el ordenador, va delimitado con comilla sencilla. | Caracteres alfanuméricos (‘a’, ‘b’, ‘c’…’z’)<br />Caracteres numéricos (‘1’, ‘2’…’0’)<br />Caracteres especiales (‘+’, ‘*’, ‘-’) |
|  Cadena  | Es aquel que pueden tomar por valor una secuencia de caracteres. Va delimitado con comilla doble. | El título de un libre, el nombre de una persona, direcciones, etc. |

## Tipos de campos

* **Campos variables:** son aquellos que permiten que el contenido almacenado en el espacio de memoria asignado, pueda ser alterado en el transcurso de la ejecución del algoritmo, es decir, en un momento tiene un valor y mas adelante puede tener otro distinto, pero nunca mas de un valor al mismo tiempo.

  ```
  contador       →     Entero
  edad           →     Entero
  direccion      →     Cadena de carácteres
  salarioBruto   →     Real
  opcion         →     Carácter
  ```

  La declaración de variables es un proceso que consiste en listar al principio del algoritmo todas las variables que se usarán, además de colocar el nombre de la variable se debe decir qué tipo de variable es.

* **Campo constante:** es otra forma de manejar los elementos almacenados en memoria, pero que a diferencia de las variables, su contenido no puede cambiar durante el proceso.

  ```
  Pi      →	3.14159
  Msg     →	Presione una tecla y continue
  altura  →	1.70
  ```

  En el momento de declarar constantes debe indicarse que lo es y colocarse su respectivo valor.

## Aspectos importantes a tener en cuenta

- Los nombres de las variables deben ser únicos: no pueden representar dos cosas al mismo tiempo.
- Una variable solo puede almacenar un único valor.
- Una variable no puede almacenar tipos de información distintos. Los números son diferentes como tales y como caracteres (1 es diferente de ‘1’).
- Es necesario diferenciar el nombre de la variable y el contenido que esta tiene en un momento determinado.
- Es aconsejable que los nombres de las variables se asemejen a lo que representan.

## Operadores aritméticos

|  Operador  | Prioridad |                Significado                 |
| :--------: | :-------: | :----------------------------------------: |
| (), [], {} |     Primer nivel de ejecución      | Paréntesis, corchetes y llaves                 |
|  **, ó, ^  |   Mayor   |                Potenciación                |
| * , /, MOD |   Media   | Multiplicación, división, residuo (módulo) |
|   + , –    |   Menor   |                Suma, resta                 |
|     =      |           |                 Asignación                 |

**¿Qué es la jerarquía de operaciones y cuál es su orden?**

En otras palabras, en cualquier problema de matemáticas debes empezar resolviendo los paréntesis, luego los exponentes; luego las multiplicaciones y divisiones y luego las sumas y restas.  Cuando  las  operaciones  son del mismo nivel, se resuelven de izquierda a derecha.

### Ejemplos:

```
9 + 3 - 4 / 2 * 8 + (14 - 9 / 3)
9 + 3 - 4 / 2 * 8 + (14 - 3)
9 + 3 - 4 / 2 * 8 + 11
9 + 3 - 16 + 11
7
```

```
14 - 12 / 4 * 2 + (8 - 2 * 9) * 3 + 2
14 - 12 / 4 * 2 + (8 - 18) * 3 + 2
14 - 12 / 4 * 2 + (-10) * 3 + 2
14 - 12 / 4 * 2 - 10 * 3 + 2
14 - 6 - 30 + 2
-20
```

```
-7 + (4 * 8 / 2 - (12 + 3)) * 3 - 9 + 15 / 5
-7 + (4 * 8 / 2 - 15) * 3 - 9 + 15 / 5
-7 + (16 - 15) * 3 - 9 + 15 / 5
-7 + 1 * 3 - 9 + 15 / 5
-7 + 3 - 9 + 15 / 5
-7 + 3 - 9 + 3
-10
```

## Operadores relacionales

Los operadores relacionales son símbolos que se usan para comparar dos valores. Si el resultado de la comparación es correcto la expresión considerada es verdadera, en caso contrario es falsa.

| Operador |    Significado    |
| :------: | :---------------: |
|    ==    |     Igualdad      |
|    >     |     Mayor que     |
|    <     |     Menor que     |
|    >=    | Mayor o igual que |
|    <=    | Menor o igual que |

# Estructura secuencial

La **estructura secuencial** es aquella en la que una acción (instrucción) sigue a otra en secuencia. Las tareas se suceden de tal modo que la salida de una es la entrada de la siguiente y así sucesivamente hasta el fin del proceso.

## Partes de un algoritmo

* **Inicio y fin:** una de las características de los algoritmos es que debe ser finito, por lo tanto debe especificarse donde comienza y donde termina. 

* **Declaración de variables:** los datos son una parte muy importante en un algoritmo, pues son ellos el punto de partida y sufren las transformaciones que darán los resultados deseados. Por esta razón deberán almacenarse en un espacio de memoria dentro del algoritmo, este espacio es llamado variable. Este se define con un nombre que permita identificarlo fácilmente y se le asigna el tipo de dato.

* Las variables se definen con un nombre que permita identificarlo fácilmente y se le asigna el tipo de dato.

  ```
  Inicio
      Cadena nombre, apellido
      Enero edad
      Real peso, estatura, imc
      Caracter sexo
      …
      …
  Fin
  ```

* **Entrada de datos:** corresponde al insumo, a los datos necesarios que requiere el proceso para ofrecer los resultados esperados. 

  ```
  Inicio
      Entero num1, num2
      Imprima  "Ingrese el primer número."
      Lea num1
      Imprima "Ingrese el segundo número."
      Lea num2
      …
      …
  Fin
  ```

- **Procesamiento de datos:** son los pasos necesarios para obtener la solución al problema planteado.

  ```
  Inicio
      Entero num1, num2, total
      Imprima "Ingrese el primer número."
      Lea num1
      Imprima “Ingrese el segundo número.”
      Lea num2
      total = num1 + num2
      …
  Fin
  ```

- **Salida de datos:** resultado arrojado por el proceso como solución.

  ```
  Inicio
      Entero num1, num2, total
      Imprima “Ingrese el primer número.”
      Lea num1
      Imprima “Ingrese el segundo número.”
      Lea num2
      total = num1 + num2
      Imprima “La suma de los dos números ingresados es: ”, total
  Fin
  ```

## Aspectos a tener en cuenta

- En un algoritmo a las variables se les da valor, bien sea por una asignación o por una
  instrucción de entrada.
- El valor que se le asigna a una variable en cualquiera de los casos debe ser del mismo tipo de
  dato que la variable.
- En la prueba de escritorio se deben mostrar los cambios que sufren todas las variables del
  algoritmo.
- La instrucción de asignación no puede ser tomada como una igualdad, ya que la variable que
  recibe el valor puede aparecer también al lado derecho de la expresión.
- Si una variable aparece en más de una instrucción de entrada o asignación, su valor es
  destruido cada que se ejecuta una nueva instrucción.

## Ejercicios propuestos

1. Hacer un algoritmo que lea dos números, calcule e imprima la suma, la resta, la multiplicación y la división.

	  ```
	Inicio
		Real A, B, suma, resta, multiplicacion, division

		Imprima "Ingrese el primer número."
		Lea A
		Imprima "Ingrese el segundo número."
		Lea B
	   
		suma = A + B
		resta = A - B
		multiplicacion = A * B
		division = A / B
	   
		Imprima "La suma de los 2 números es: ", suma
		Imprima "La resta de los 2 números es: ", resta
		Imprima "La multiplicación de los 2 números es: ", multiplicacion
		Imprima "La división de los 2 números es: ", division
	Fin
	 ```
	 
	### Prueba de escritorio:
	   
	|  A   |  B   | suma | resta | multiplicacion | division |
	| :--: | :--: | :--: | :---: | :------------: | :------: |
	|  20  |  7   |  27  |  13   |      140       |   2.85   |
	| 2.5  | 2.5  |  5   |   0   |      6.25      |    1     |
   
2. Hacer un algoritmo que lea 4 notas e imprima su promedio.

	  ```
	Inicio
		Real N1, N2, N3, N4, promedio
	       
		Imprima "Ingrese la primera nota."
		Lea N1
		Imprima "Ingrese la segunda nota."
		Lea N2
		Imprima "Ingrese la tercer nota."
		Lea N3
		Imprima "Ingrese la cuarta nota."
		Lea N4
	       
		promedio = (N1 + N2 + N3 + N4) / 4
	       
		Imprima "El promedio de las 4 notas es: ", promedio
	Fin
	 ```

	 ### Prueba de escritorio:
	 
	|  N1  |  N2  |  N3  |  N4  | promedio |
	| :--: | :--: | :--: | :--: | :------: |
	| 4.7  | 4.1  | 3.5  | 2.3  |   3.65   |
	| 3.9  | 2.5  | 4.1  | 3.3  |   3.45   |
   
3. Hacer un algoritmo que calcule e imprima:

   * El área de un triángulo.
   * El perímetro de un triángulo.


	```
	Inicio
		Real base, altura, lado1, lado2, lado3, area, perimetro
	       
		Imprima "Ingrese la medida de la base del triángulo."
		Lea base
		Imprima "Ingrese la medida de la altura del triángulo."
		Lea altura
	       
		area = (base * altura) / 2
	       
		Imprima "Ingrese la medida del primer lado del triángulo."
		Lea lado1
		Imprima "Ingrese la medida del segundo lado del triángulo."
		Lea lado2
		Imprima "Ingrese la medida del tercer lado del triángulo."
		Lea lado3
	       
		perimetro = lado1 + lado2 + lado3
	       
		Imprima "El área del triángulo es: ", area
		Imprima "El perimetro del triángulo es: ", perimetro
	Fin
	 ```
	
	### Prueba de escritorio:
	
	| base | altura | lado1 | lado2 | lado3 | area | perimetro |
	| :--: | :----: | :---: | :---: | :---: | :--: | :-------: |
	|  7   |   12   |  14   |  26   |   9   |  42  |    49     |
	|  14  |   2    |   4   |   7   |   5   |  14  |    16     |

4. En un almacén venden camisas a $35.000 cada una. Hacer un algoritmo que lea la cantidad de camisas que una persona va a comprar e imprima:

   * Valor inicial de la compra.
   * El valor del IVA que corresponde al 19% del valor inicial.
   * El valor del descuento que equivale al 25% del valor inicial.
   * El total a pagar que equivale al valor inicial, menos el descuento, más el IVA.
   
    ```
	Inicio
		Entero cantidadCamisas
		Real valorInicial, IVA, descuento, total
	       
		Imprima "¿Cuántas camisas desea llevar?"
		Lea cantidadCamisas
	       
		valorInicial = cantidadCamisas * 35000
		IVA = valorInicial * 0,19
		descuento = valorInicial * 0,25
		total = valorInicial + IVA - descuento
	       
		Imprima "El valor inicial de la compra es: ", valorInicial
		Imprima "El valor del IVA es: ", IVA
		Imprima "El valor del descuento es: ", descuento
		Imprima "El total a pagar es: ", total
	Fin
	 ```

	### Prueba de escritorio:
	
	| cantidadCamisas | valorInicial |  IVA   | descuento |  total  |
	| :-------------: | :----------: | :----: | :-------: | :-----: |
	|        4        |   140.000    | 26.600 |  35.000   | 131.600 |

5. Hacer un algoritmo que lea el valor por hora y el número de horas trabajadas por un empleado. Calcular e imprimir:

   * Salario bruto
   * EPS
   * Pensión
   * Salario neto
   
	```
	Inicio
		Real valorHora, horasTrabajadas, salarioBruto, EPS, pension, salarioNeto
	   	
	   	Imprima "Ingrese el valor de la hora."
	   	Lea valorHora
	   	Imprima "Ingrese el número de horas trabajadas por el empleado."
	   	Lea horasTrabajadas
	   	
	   	salarioBruto = horasTrabajadas * valorHora
	   	EPS = salarioBruto * 0,04
	   	pension = salarioBruto * 0,04
	   	salarioNeto = salarioBruto – EPS – pension
	   	
	   	Imprima "El valor del salario bruto es: ", salarioBruto
	   	Imprima "El valor del aporte para la EPS es: ", EPS
	   	Imprima "El valor del aporte para la pensión es: ", pension
	   	Imprima "El valor del salario neto del empleado es: ", salarioNeto
	Fin
	```
	### Prueba de escritorio:

	| valorHora | horasTrabajadas | salarioBruto |  Eps  | pension | salarioNeto |
	| :-------: | :-------------: | :----------: | :---: | :-----: | :---------: |
	|   2.600   |       78        |   202.800    | 8.112 |  8.112  |   186.576   |

6. A la mamá de Juan le preguntan su edad y contesta: tengo 3 hijos, pregúntale a Juan su edad; Alberto tiene 2/3 de la edad de Juan, Ana tiene 4/3 de la edad de Juan y mi edad es la suma de las tres. Hacer un algoritmo que calcule la edad de los cuatro.

	```
	Inicio
		Entero juan, alberto, ana, mama
	       
		Imprima "Ingrese la edad de Juan."
		Lea juan
	       
		alberto = (juan * 2) /3
		ana = (juan * 4) / 3
		mama = juan + alberto + ana
	       
		Imprima "La edad de Juan es: ", juan
		Imprima "La edad de Alberto es: ", alberto
		Imprima "La edad de Ana es: ", ana
		Imprima "La edad de la madre es: ", mama
	Fin
	```
	
	### Prueba de escritorio:
		
	| juan | alberto | ana  | mama |
	| :--: | :-----: | :--: | :--: |
	|  9   |    6    |  12  |  27  |
		
7. Hacer un algoritmo que lea un número e imprima el contrario.
   

   ```
	Inicio
		Real numero, contrario
   	
		Imprima "Ingrese un número."
		Lea numero
   	
		contrario = numero * -1
   	
		Imprima "El contrario del número ingresado es: ", contrario
   Fin
   ```

	### Prueba de escritorio:
	
   | numero | contrario |
   | :----: | :-------: |
   |   7    |    -7     |

8. En una alcaldía se cuenta con una disponibilidad presupuestal de $120.000.000. Esta debe ser repartida entre la cabecera municipal y 2 veredas así:

   * 50% para la cabecera municipal.
   * 30% para la vereda #1.
   * 20% para la vereda #2.

   Hacer un algoritmo que imprima cuánto dinero le corresponde a la cabecera y a las 2 veredas.
   
	```
	Inicio
		Entero cabeceraMunicipal, veredaUno, veredaDos
	       
		cabeceraMunicipal = 120000000 * 0,5
		veredaUno = 120000000 * 0,3
		veredaDos = 120000000 * 0,2
	       
		Imprima "La cantidad de dinero para la cabecera es: ", cabeceraMunicipal
		Imprima "La cantidad de dinero para la vereda #1 es: ", veredaUno
		Imprima "La cantidad de dinero para la vereda #2 es: ", veredaDos
	Fin
	```
	
	### Prueba de escritorio:

	| cabeceraMunicipal | veredaUno  | veredaDos  |
	| :---------------: | :--------: | :--------: |
	|    60.000.000     | 36.000.000 | 24.000.000 |
   
9. Hacer un algoritmo que calcule el área y el perímetro de un cuadrado.

	```
	Inicio
       Real lado, area, perimetro
       
       Imprima "Ingrese la medida de uno de los lados del cuadrado."
       Lea lado
       
       area = lado * lado
       perimetro = lado * 4
       
       Imprima "El área del cuadrado es: ", area
       Imprima "El perímetro del cuadrado es: ", perimetro
	Fin
	```

	### Prueba de escritorio:

	| lado | area | perimetro |
	| :--: | :--: | :-------: |
	|  7   |  49  |    28     |
   
10. Hacer un algoritmo que calcule e imprima el valor a pagar por una matrícula, teniendo en cuenta que hay un descuento del 25%. Imprimir el valor del descuento y el valor a pagar.

	```
	Inicio
        Entero matricula, descuento, total
        
        Imprima  "Ingrese el valor de la matrícula."
        Lea matricula
        
        descuento = matricula * 0,25
        total = matricula - descuento
        
        Imprima"El valor del descuento es: ", descuento
        Imprima "El valor total a pagar es: ",, total
    Fin
	```

	### Prueba de escritorio:	
    
    | matricula | descuento |   total   |
    | :-------: | :-------: | :-------: |
    | 2.000.000 |  700.000  | 2.100.100 |
    
11. Diseñar un algoritmo que muestre en días, horas, minutos y segundos una cantidad de tiempo que inicialmente fue capturada en segundos.

	```
	Inicio
    	Real tiempoInicial, dias, horas, minutos
    	
    	Imprima "Ingrese la cantidad tiempo inicial en segundos"
    	Lea tiempoInicial
    	
    	dias = 120 * (1 / 60) * (1 / 60) * (1 / 24)
    	horas = 120 * (1 / 60) * (1 / 60)
    	minutos = 120 * (1 / 60)
    	
    	Imprima "La cantidad de segundos ingresados fueron: ", tiempoInicial;
    	Imprima "El equivalente en días es: ", dias
    	Imprima "El equivalente en horas es:", horas
    	Imprima "El equivalente en horas es:", minutos
    Fin
	```

	### Prueba de escritorio:
	
    | TiempoInicial | dias |   horas   | minutos |
    | :-------: | :-------: | :-------: | :-------: |
    |      450      | 0.001388888 | 0.033333333 |    2    |

# **Estructura condicional simple**



Las estructuras condicionales simples se les conoce como: Toma de decisiones. Estas tomas de decisiones tienen la siguiente forma:

```
Si (Condicion) Entonces
	<Instrucciones>
Fin Si
```

- **Si:** indica el comando de comparación.
- **Condición:** indica la condición a evaluar.
- **Entonces:** precede a las acciones a realizar cuando se cumple la condición.
- **Instrucción(es):** son las acciones a realizar cuando se cumple o no la condición.
- **Fin Si:** indica el fin del comando de comparación.

## Aspectos a tener en cuenta

- Las variables que hacen parte de una expresión de tipo lógico deben tener un valor previo
  asignado.
  
- Cuando se conforma un registro de entrada de datos, los valores de los campos deben ir separados al menos por un espacio en blanco. Si el campo es de tipo real, el punto debe estar presente y todo carácter que esté entre comillas hará parte de una constante alfanumérica. Si el campo indica miles, millones, etc., no debe estar presente el punto para indicar estas cantidades. El punto sólo se debe utilizar para indicar la parte decimal. Por ejemplo, 1.000.000 (un millón), debe indicarse como 1000000.

- Si un campo indica porcentaje, los caracteres que lo determinan(%, $) no deben estar presentes en el registro de entrada. Serán erróneas las expresiones: a > $100, P = 30%, k > 33%, etc.

- Si la comparación en una condición involucra constantes alfanuméricas, éstas deben estar entre comillas; por ejemplo NOMBRE = “ISABEL”.


## Ejercicios propuestos

1. Leer un número e imprimir si es par.

   
   ```
   Inicio
   	Entero numero
   
       Imprima "Ingrese un número."
       Lea numero
   
       Si (numero MOD 2 == 0) Entonces
       	Imprima "El número ingresado es par."
       Fin Si
   Fin
   ```
   
   |  N   |           Mensaje           |
   | :--: | :-------------------------: |
   |  12  | El número ingresado es par. |
   |  5   |                             |
   
2. Leer un número e imprimir si es impar.

   ```
Inicio
   	Real numero
   	
   	Imprima "Ingrese un número."
   	Lea numero
   	
   	Si (numero MOD 2 <> 0) Entonces
   		Imprima "El número ingresado es impar."	
   	Fin Si
   Fin
   ```
   
   |  N   |            Mensaje            |
| :--: | :---------------------------: |
   |  3   | El número ingresado es impar. |
   |  10  |                               |
   
3. Hacer un algoritmo que lea un número y si este es múltiplo de 4 imprima su triple.

   ```
Inicio
    	Real numero, triple
      	
      	Imprima "Ingrese un número."
      	Lea numero
      	
      	Si (numero MOD 4 == 0) Entonces
      		triple = numero * 3
      		Imprima "El triple del número ingresado es: ", triple
      	Fin Si
   Fin
   ```
   
   | numero | triple |
| :----: | :----: |
   |   17   |        |
   |  180   |  540   |
   
4. Hacer un algoritmo que lea dos números e imprima su suma, si el primero es mayor que el segundo.

   ```
Inicio
   	Real A, B, suma
   	
   	Imprima "Ingrese un número."
   	Lea A
   	Imprima "Ingrese otro número."
   	Lea B
   	
   	Si (A > B) Entonces
   		suma = A + B
   		Imprima "La suma de los dos números es: ", suma
   	Fin Si
   Fin
   ```
   
   |  A   |  B   | suma |
| :--: | :--: | :--: |
   |  4   |  7   |      |
   |  16  |  2   |  18  |
   
5. Hacer un algoritmo que lea el valor total de una compra y si el sexo de comprador es femenino, se hará un descuento del 30%. Imprimir el valor a pagar por cada cliente.

   ```
Inicio
      	Real compra, descuento
      	Cadena sexo
      	
      	Imprima "Ingrese el valor de la compra."
      	Lea compra
      	Imprima "Ingrese el sexo del comprador."
      	Lea sexo
      	
      	Si (sexo == "Femenino") Entonces
      		descuento = compra * 0.3
      		compra = compra - descuento
      	Fin si
      	
      	Imprima "El total a pagar es: ", compra
    Fin
   ```
   
   |  compra   |   sexo    | descuento |
| :-------: | :-------: | :-------: |
   | ~~1.000~~ | Femenino  |    300    |
   |    700    |           |           |
   |   2.000   | Masculino |  - - - -  |
   
6. Hacer un algoritmo que lea 3 notas, calcular su definitiva en un rango de 0 – 5 e imprimir un mensaje donde diga si el alumno aprobó.

   ```
   Inicio
      	Real N1, N2, N3, definitiva
      	
      	Imprima "Ingrese la primer nota."
      	Lea N1
      	Imprima "Ingrese la segunda nota."
      	Lea N2
      	Imprima "Ingrese la tercer nota."
      	Lea N3
      	
      	definitiva = (N1 + N2 + N3) / 3
      	
      	Si (definitiva >= 3.5) Entonces
      		Imprima "El alumno aprobó."
      	Fin Si
   Fin
   ```
   
   |  N1  |  N2  |  N3  | definitiva | Mensaje |
   | :--: | :--: | :--: | :--------: | :-----: |
   |  4   | 3.2  | 2.7  |    3.3     | Aprobó  |
   
7. Elabore un algoritmo que lea un número y si este es mayor a 10 devuelva el triple de este.

   ```
   Inicio
      	Real numero, triple
      	
      	Imprima "Ingrese un número."
      	Lea numero
      	
      	Si (numero > 10 ) Entonces
      		triple = numero * 3
      		Imprima "El triple del número ingresado es: ", triple
      	Fin Si
   Fin
   ```
   
   | numero | triple |
   | :----: | :----: |
   |   15   |   45   |
   |   4    |        |
   
8. Hacer un algoritmo que lea la estatura de una persona y si esta es mayor a 1,70, imprimir que es alta.

   ```
Inicio
      	Real estatura
      	
      	Imprima "Ingrese la estatura de la persona."
      	Lea estatura
      	
      	Si (estatura > 1.70) Entonces
      		Imprima "La persona es alta."
      	Fin si
   Fin
   ```
   
   | estatura |       Mensaje       |
| :------: | :-----------------: |
   |   1.70   | La persona es alta. |

9. Hacer un algoritmo que lea un número y si es negativo, lo imprima con signo contrario.

   ```
   Inicio
      	Real numero, contrario
      	
      	Imprima "Ingrese un número."
      	Lea numero
      	
      	Si (numero < 0) Entonces
      		contrario = numero * -1
      		Imprima "El contrario del número ingresado es: ", contrario
      	Fin Si
   Fin
   ```
   
   | numero | contrario |
   | :----: | :-------: |
   |   -7   |     7     |
   |   2    |           |

# **Estructura condicional doble**



Las estructuras condicionales dobles permiten elegir entre dos opciones o alternativas posibles en función del cumplimiento o no de una determinada condición. 

   ## Estructura

   ```
   Si (Condición) Entonces
   	<Instrucciones>
   Si no
   	<Instrucciones>
   Fin Si
   ```

- **Sino:** precede a las acciones a realizar cuando no se cumple la condición.

Dependiendo de si la comparación es cierta o falsa, se pueden realizar una o más acciones.

   ## Ejercicios propuestos

   1. Hacer un algoritmo que lea dos números, si el primero es mayor que el segundo imprimir la resta, de lo contrario imprimir la suma.
      

      ```
      Inicio
      	Real N1, N2, resta, suma
      	
      	Imprima "Ingrese el primer número."
      	Lea N1
      	Imprima "Ingrese el segundo número."
      	Lea N2
      	
      	Si (N1 > N2) Entonces
      		resta = N1 - N2
      		Imprima "La resta de los 2 números es: ", resta
      	Sino
      		suma = N1 + N2
      		Imprima "La suma de los 2 números es:", suma
      	Fin Si
      Fin
      ```

      |  N1  |  N2  | resta | suma |
      | :--: | :--: | :---: | :--: |
      |  18  |  22  |       |  40  |
      |  12  |  2   |  10   |      |

   2. Hacer un algoritmo que lea un número, si es múltiplo de 8 debe imprimir la mitad, de lo contrario debe imprimir el doble.

      ```
Inicio
      	Real numero, mitad, doble
      	
      	Imprima "Ingrese un número."
      	Lea numero
      	
      	Si (numero MOD 8 == 0) Entonces
      		mitad = numero / 2
      		Imprima "La mitad es: ", mitad
      	Sino
      		doble = numero * 2
      		Imprima "El doble es: ", doble
      	Fin Si
      Fin
      ```
      
      | numero | mitad | doble |
| :----: | :---: | :---: |
      |   16   |   8   |       |
      |   23   |       |  46   |
      
   3. Leer 4 notas de un estudiante, calcular el promedio e imprimir un mensaje indicando si aprobó o reprobó.

      ```
Inicio
      	Real N1, N2, N3, N4, promedio
      	
      	Imprima "Ingrese la primer nota."
      	Lea N1
      	Imprima "Ingrese la segunda nota."
      	Lea N2
      	Imprima "Ingrese la tercer nota."
      	Lea N3
      	Imprima "Ingrese la cuarta nota."
      	Lea N4
      	
      	promedio = (N1 + N2 + N3 + N4) / 4
      	
      	Si (promedio >= 3.5) Entonces
      		Imprima "El estudiante aprobó."
      	Sino
      		Imprima "El estudiante reprobó."
      	Fin si
      Fin
      ```
      
      |  N1  |  N2  |  N3  |  N4  | promedio |        Mensaje         |
| :--: | :--: | :--: | :--: | :------: | :--------------------: |
      | 3.8  | 2.9  |  4   | 4.2  |   3.7    | El estudiante aprobó.  |
      | 2.3  |  1   | 2.6  | 3.2  |   2.2    | El estudiante reprobó. |
      
   4. Hacer un algoritmo que lea el valor de una compra, si este es superior a $1.000.000, se hace un descuento del 30%, de lo contrario se hace un descuento del 20%. Imprimir el valor inicial de la compra, el valor del descuento y el valor final.
      

      ```
      Inicio
          Real valorInicial, descuento, valorFinal
          
          Imprima “Ingrese el valor de la compra.”
          Lea valorInicial
          
          Si (valorInicial > 1000000) Entonces
          	descuento = valorInicial * 0,3
          Sino
          	descuento = valorInicial * 0,2
          Fin Si
          
          valorFinal = valorInicial – descuento
          
          Imprima “El valor inicial de la compra es: ”, valorInicial
          Imprima “El valor del descuento es: ”, descuento
          Imprima “El valor final de la compra es: ”, valorFinal
      Fin
      ```

      | valorInicial | descuento | valorFinal |
      | :----------: | :-------: | :--------: |
      |  1.850.000   |  555.000  | 1.295.000  |
      |   600.000    |  120.000  |  480.000   |


# **Estructura condicional compuesta o anidada**



Las estructuras de comparación múltiples, son tomas de decisión especializadas que permiten comparar una variable contra distintos posibles resultados, ejecutando para cada caso una serie de instrucciones especificas. La forma común es la siguiente:

```
Si (Condicion) Entonces
	<Instrucciones>
	Sino
		si (Condicion) Entonces
			<Instrucciones>
			Sino
				.
				. <Varias condiciones>
				.
```

# **Ejercicios propuestos**

1. Hacer un algoritmo que lea 3 números e imprima un mensaje si todos son mayores a 10.

   ```
   Inicio
   	Real n1, n2, n3
   	
   	Imprima “Ingrese el primer número."
   	Lea n1
   	Imprima “Ingrese el segundo número.”
      	Lea n2
      	Imprima “Ingrese el tercer número.”
      	Lea n3
      	
      	Si ((n1 > 10) y (n2 > 10) y (n3 > 10)) Entonces
      		Imprima “Todos los números son mayores a 10.”
      	Fin Si
   Fin
   ```

   |  n1  |  n2  |  n3  |               Mensaje               |
   | :--: | :--: | :--: | :---------------------------------: |
   |  24  |  37  |  52  | Todos los números son mayores a 10. |
   |  9   |  22  |  16  |                                     |

2. Hacer un algoritmo que lea 4 números e imprima la suma del mayor y el menor.

   ```
Inicio
      	Real n1, n2, n3, n4, mayor, menor, suma
   	
   	Imprima "Ingrese el primer número."
   	Lea n1
   	Imprima "Ingrese el segundo número."
   	Lea n2
   	Imprima "Ingrese el tercer número."
   	Lea n3
   	Imprima "Ingrese el cuarto número."
   	Lea n4
   	
   	Si ((n1 > n2) y (n1 > n3) y (n1 > n4)) Entonces
   		mayor = n1
   	Sino 
   		Si ((n2 > n1) y (n2 > n3) y (n2 > n4)) Entonces
   			mayor = n2
   		Sino 
   			Si ((n3 > n1) y (n3 > n2) y (n3 > n4)) Entonces
   				mayor = n3
   			Sino
   				mayor = n4
   			Fin Si
   		Fin Si
   	Fin Si
   	
   	Si ((n1 < n2) y (n1 < n3) y (n1 < n4)) Entonces
   		menor = n1
   	Sino
   		Si ((n2 < n1) y (n2 < n3) y (n3 < n4)) Entonces
   			menor = n2
   		Sino 
   			Si ((n3 < n1) y (n3 < n2) y (n3 < n4)) Entonces
   				menor = n3
   			Sino
   				menor = n4
   			Fin Si
   		Fin Si
   	Fin si
   	
   	suma = mayor + menor
   	
   	Imprima "La suma del número mayor y menor es: ", suma
   Fin
   ```
   
   |  n1  |  n2  |  n3  |  n4  | mayor | menor |
| :--: | :--: | :--: | :--: | :---: | :---: |
   |  5   |  20  |  7   |  14  |  20   |   5   |
   
3. En una universidad se encuentran en periodo de matrículas, el valor del semestre es de $3.500.000 para todos los programas. Se hace un descuento dependiendo del estrato y de los ingresos familiares, así:

   * Estratos 1 o 2 e ingresos iguales o inferiores a $2.500.000, 35% de descuento.

   * Estratos 1 o 2 e ingresos superiores a $2.500.000, 30% de descuento.

   * Estratos 3 o 4 e ingresos iguales o inferiores a $2.500.000, 25% de descuento.

   * Estratos 3 o 4 e ingresos superiores a $2.500.000, 20% de descuento.

   * De lo contrario, no hay descuento.

   
   Imprimir el valor del descuento y el valor final a pagar.

   ```
   Inicio
     	Entero estrato
     	Real ingresos, descuento, total 
     	
     	Imprima "¿Cuál es su estrato?"
     	Lea estrato
     	Imprima "¿Cuánto son sus ingresos familiares?"
     	Lea ingresos
     	
     	Si ((estrato == 1) o (estrato == 2) y (ingresos <= 2500000)) Entonces
     		descuento = 3500000 * 0.35
     	Sino
     		Si ((estrato == 1) o (estrato == 2) y (ingresos > 2500000)) Entonces
     			descuento = 3500000 * 0.3
     		Sino
     			Si ((estrato == 3) o (estrato == 4) y (ingresos <= 2500000)) Entonces
     				descuento = 3500000 * 0.25
     			Sino
     				Si ((estrato == 3) o (estrato == 4) y (ingresos > 2500000)) Entonces
     					descuento = 3500000 * 0.20
     				Sino
     					descuento = 0
     				Fin Si
     			Fin Si
     		FinSi
     	Fin Si
     	
     	total = 3500000 - descuento
     	
     	Imprima "El valor des descuento es: ", descuento
     	Imprima "El total a pagar es: ", total
   Fin
   ```
   
   | estrato | ingresos  | descuento |   total   |
| :-----: | :-------: | :-------: | :-------: |
   |    2    | 1.100.000 | 1.225.000 | 2.275.000 |
   |    3    | 3.800.000 |  700.000  | 2.800.000 |


4. Leer cuatro notas de un estudiante, calcular el promedio e imprimir un mensaje de acuerdo al resultado, así:

    * Si es igual a 5: “Excelente”.
    * Mayor o igual a 4 y menor a 4.9: “Sobresaliente”.
    * Mayor o igual a 3.5 y menor a 4: “Aceptable”.
    * De lo contrario: “Insuficiente”.

    ```
    Inicio
    	Real n1, n2, n3, n4, promedio
    	
    	Imprima "Ingrese la primer nota."
    	Lea n1
    	Imprima "Ingrese la segunda nota."
    	Lea n2
    	Imprima "Ingrese la tercer nota."
    	Lea n3
    	Imprima "Ingrese la cuarta nota."
    	Lea n4
    	
    	promedio = (n1 + n2 + n3 + n4) / 4
    	
    	Si (promedio == 5) Entonces
    		Imprima "Excelente."
    	Sino
    		Si ((promedio >= 4) y (promedio < 4.9)) Entonces
    			Imprima "Sobresaliente."
    		Sino
    			Si ((promedio >= 3.5) y (promedio < 4)) Entonces
    				Imprima "Aceptable."
    			Sino
    				Imprima "Insuficiente."
    			Fin Si
    		Fin Si
    	Fin Si
    Fin
    ```

    |  n1  |  n2  |  n3  |  n4  | promedio |    Salida     |
    | :--: | :--: | :--: | :--: | :------: | :-----------: |
    | 2.5  | 3.8  |  4   | 3.6  |   3.47   | Insuficiente  |
    | 3.8  | 4.2  | 4.4  | 3.6  |    4     | Sobresaliente |

5. Leer 3 números e imprimirlos en orden descendente (De mayor a menor).

     ```
 Inicio
        	Real n1, n2, n3
        	
        	Imprima "Ingrese el primer número."
         Lea n1
         Imprima "Ingrese el segundo número."
         Lea n2
         Imprima "Ingerse el tercer número."
         Lea n3
     
         Si ((n1 <> n2) y (n1 <> n3) y (n2 <> n3)) Entonces
             Si ((n1 > n2) y (n2 > n3) Entonces
                 Imprima n1, n2, n3
             Sino
                 Si ((n1 > n3) y (n3 > n2) Entonces
                     Imprima n1, n3, n2
                 Sino
                     Si ((n2 > n1) y (n1 > n3)) Entonces
                         Imprima n2, n1, n3
                     Sino
                         Si ((n2 > n3) y (n3 > n1)) Entonces
                             Imprima n2, n3, n1
                         Sino
                             Si ((n3 > n1) y (n1 > n2)) Entonces
                                 Imprima n3, n1, n2
                             Sino
                                 Imprima n3, n2, n1
                             Fin Si
                         Fin Si
                     Fin Si
                 Fin Si
             FinSi
         Sino
             Imprima "Uno de los números ingresados esta repetido."
         Fin Si
    Fin
    ```
   
   |  n1  |  n2  |  n3  |  Salida   |
| :--: | :--: | :--: | :-------: |
   |  7   |  15  |  3   | 15, 7, 3  |
   |  40  |  8   |  74  | 74, 40, 8 |
   
6. Leer 2 números y calcular:
   
   * Si el primero es mayor al segundo y es múltiplo de 3: la resta.
    * Si son iguales y múltiplos de 4: la suma.
     
     * De lo contrario: la multiplicación.
	
     Imprimir el resultado.
   
     ```
     Inicio
     	Real n1, n2, resta, suma, multiplicacion
     	
     	Imprima "Ingrese el primer número."
     	Lea n1
     	Imprima "Ingrese el segundo número."
     	Lea n2
     	
     	Si ((n1 > n2) y (n1 MOD 3 == 0)) Entonces
     		resta = n1 - n2
     		Imprima "La resta es: ", resta
     	Sino
     		Si ((n1 == n2) y ((n1 MOD 4 == 0) y (n2 MOD 4 == 0))) Entonces
     			suma = n1 + n2
     			Imprima "La suma es: ", suma
     		Sino
     			multiplicacion = n1 * n2
     			Imprima "La multiplicación es: ", multiplicacion
     		Fin Si
     	Fin Si
     Fin
     ```
   
   |  n1  |  n2  | resta | suma | multiplicacion |
   | :--: | :--: | :---: | :--: | :------------: |
   |  12  |  7   |   5   |      |                |
   |  16  |  16  |       |  32  |                |
   |  1   |  5   |       |      |       5        |
   
7. Para las votaciones de un municipio de Antioquia, se tienen registradas 5 mesas de votación. Dependiendo del ultimo digito del documento de identidad será asignada la mesa de votación así:
   
* 0 – 1 Mesa 1
  
     * 2 – 3 Mesa 2
     
     * 4 – 5 Mesa 3
     
     * 6 – 7 Mesa 4
     
     * 8 – 9 Mesa 5
     
     Elaborar un algoritmo que permita imprimir el número de la mesa en la que podrá votar la persona, teniendo en cuenta que debe ser mayor de edad y de nacionalidad colombiana.
     
     ```
     Inicio
     	Entero edad, digito
      	Cadena nacionalidad
      	
      	Imprima "Ingrese su edad."
      	Lea edad
      	Imprima "Ingrese su nacionalidad."
      	Lea nacionalidad
      	
      	Si ((edad >= 18) y (nacionalidad == "Colombiana")) Entonces
      	
      		Imprima "Ingrese el ultimo dígito de su cédula."
      		Lea digito
      		
      		Si ((digito == 0) o (digito == 1)) Entonces
      			Imprima "Le tocó la mesa #1."
      		Sino
      			Si ((digito == 2) o (digito == 3)) Entonces
      				Imprima "Le tocó la mesa #2."
      			Sino
      				Si ((digito == 4) o (digito == 5)) Entonces
      					Imprima "Le tocó la mesa #3."
      				Sino
      					Si ((digito == 6) o (digito == 7)) Entonces
      						Imprima "Le tocó la mesa #4."
      					Sino Si ((digito == 8) o (digito == 9)) Entonces
      						Imprima "Le toco la mesa #5."
      					Fin Si
      				Fin Si
      			Fin Si
      		Fin Si
      	Sino
      		Imprima "Usted no puede participar en la votaciones."
      	Fin Si
     Fin
     ```
     
     | edad | nacionalidad | digito |                   Salida                    |
     | :--: | :----------: | :----: | :-----------------------------------------: |
     |  22  |  Colombiana  |   6    |             Le tocó la mesa #4.             |
     |  17  |  Colombiana  |        | Usted no puede participar en la votaciones. |
     


8. Una empresa estatal requiere clasificar a las personas que se jubilarán en el año 2013. Existen 3 tipos de jubilación: por edad, por antigüedad joven y por antigüedad adulta. Las personas inscritas en la jubilación por edad, deben tener una edad igual o superior de 60 años y una antigüedad en su empleo menor de 25 años. Las personas inscritas en la jubilación por antigüedad joven, deben tener menos de 60 años y una antigüedad para su empleo de 25 años o más. Las personas inscritas en la jubilación por antigüedad adulta deben tener más de 60 años y una antigüedad para su empleo de más de 25 años. Determinar en qué tipo de jubilación quedará inscrita una persona.
   

   ```
   Inicio
   	Entero edad, antiguedad
   	
   	Imprima "¿Cuál es la edad del empleado?"
   	Lea edad
   	Imprima "¿Cuántos años lleva en su empleo?"
   	Lea antiguedad
   	
   	Si ((edad >= 60) y (antiguedad < 25)) Entonces
   		Imprima "Se jubila por edad."
   	Sino
   		Si ((edad < 60) y (antiguedad >= 25)) Entonces
   			Imprima "Se jubila por antigüedad joven."
   		Sino
   			Si ((edad > 60) y (antiguedad > 25)) Entonces
   				Imprima "Se jubila por antigüedad adulta."
   			Sino
   				Imprima "No cumple con los requisitos."
   			Fin Si
   		Fin Si
   	Fin Si
   Fin
   ```

   | edad | antiguedad |              Salida              |
   | :--: | :--------: | :------------------------------: |
   |  62  |     14     |       Se jubila por edad.        |
   |  45  |     28     | Se jubila por antigüedad joven.  |
   |  61  |     35     | Se jubila por antigüedad adulta. |
   |  59  |     21     |  No cumple con los requisitos.   |

9. Un vendedor de televisores, ofrece un descuento del 15% sobre el precio sin IVA, para cualquier aparato cuyo precio supere $1.000.000; además, ofrece un 7% sobre el precio sin IVA, si el aparato es marca LG. Determinar cuánto debe pagar con IVA incluido cualquier comprador.

   ```
Inicio
   	Real precioTV, descuento, total, IVA
   	Cadena marcaTV
   	
   	Imprima "Ingrese el precio del televisor."
   	Lea precioTV
   	Imprima "Ingrese la marca."
   	Lea marcaTV
   	
   	
   	Si (precio > 1000000) Entonces
   		descuento = precioTV * 0.15
   	Sino
   		Si ((precio > 1000000) y (marca == "LG")) Entonces
   			descuento = (precioTV * 0.15) + (precioTV * 0.07)
   		Sino
   			Si (marca == "LG") Entonces
   				descuento = precioTV
   			Fin Si
   		Fin Si
   	Fin Si
   	
   	total = precioTV - descuento
   	totalIVA = precioTV 
   	
   	Imprima "El total a pagar es: ", total
   Fin
   ```
   
   | precioTV  | descuento | IVA  | Total | marca |
| :-------: | :-------: | :--: | :---: | ----- |
   | 2.000.000 |           |      |       | LG    |
   |           |           |      |       |       |
   |           |           |      |       |       |
   
10. Determinar la cantidad de dinero que recibirá un trabajador por concepto de las horas extras trabajadas en una empresa, sabiendo que cuando las horas de trabajo excedan de 40, el resto se considera horas extras y se pagan al doble de una hora normal, cuando no excedan de la 8; si las horas extras exceden de 8, se pagan las primeras 8 al doble de lo que se paga una hora normal y el resto al triple. Del trabajador se conocen los siguientes datos: número de horas trabajadas en la semana y valor recibido por una hora normal de trabajo.

    ```
    Inicio
    	Entero horasTrabajadas
    	Real valorHora, extras, salario
    	
    	Imprima "Ingrese el número de horas trabajadas por el empleado."
    	Lea horasTrabajadas;
    	Imprima "Ingrese el costo por hora laborada."
    	Lea valorHora
    	
    	Si (horasTrabajadas > 40) Entonces
    		extras = horasTrabajadas - 40
    		Si (horasTrabajadas > 8) Entonces
    			salario = ((40 * valorHora) + (8 * (valorHora * 2)) + ((extras - 8) * (valorHora * 3)))
    		SiNo
    			salario = ((40 * valorHora) + (extras * (valorHora * 2)))
    		FinSi
    	SiNo
    		salario = horasTrabajadas * valorHora
    	FinSi
    	
    	Imprima "El salario del empleado es: ", salario
    Fin
    ```

    | horasTrabajadas | valorHora | extras | salario |
    | :-------------: | :-------: | :----: | :-----: |
    |       49        |   2.700   |   9    | 159.300 |
    |       57        |   3.400   |   17   | 282.200 |
    |       36        |   4.000   |        | 144.000 |

11. Una llantera, ofrece descuentos por la cantidad y marca de llantas compradas así:

    | Cantidad  |  Marca   | Descuento |
    | :-------: | :------: | :-------: |
    |   0 - 5   | Goodyear |    5%     |
    |   0 - 5   | Pirelli  |    8%     |
    |  6 - 10   | Goodyear |    10%    |
    |  6 - 10   | Pirelli  |    12%    |
    | Más de 10 | Goodyear |    13%    |
    | Más de 10 | Pirelli  |    15%    |

    Hacer un algoritmo que permita leer esta información e imprima el valor inicial, el valor del descuento y el valor final que deberá pagar un cliente.

    ```
    Inicio
    	Real precio, valorInicial, descuento, valorFinal
    	Entero cantidad
    	Cadena marca
    	
    	Imprima "Ingrese la marca."
    	Lea marca
    	Imprima "Ingrese el precio."
    	Lea precio.
    	Imprima "Ingrese la cantidad."
    	Lea cantidad
    	
    	valorInicial = precio * cantidad
    	
    	Si (((cantidad >= 0) y (<= 5)) y (marca == "Goodyear")) Entonces
    		descuento = valorInicial * 0.05
    	Sino
    		Si (((cantidad >= 0) y (<= 5)) y (marca == "Pirelli")) Entonces
    			descuento = valorInicial * 0.08
    		Sino
    			Si (((cantidad >= 6) y (<= 10)) y (marca == "Goodyear")) Entonces
    				descuento = valorInicial * 0.1
    			Sino
    				Si (((cantidad >= 6) y (<= 10)) y (marca == "Pirelli")) Entonces
    					descuento = valorInicial * 0.12
    				Sino
    					Si ((cantidad > 10) y (marca == "Goodyear")) Entonces
    						descuento = valorInicial * 0.13
    					Sino
    						Si ((cantidad > 10) y (marca == "Pirelli")) Entonces
    							descuento = valorInicial * 0.15
    						Sino
    							descuento = 0
    						Fin Si
    					Fin Si
    				Fin Si
    			Fin Si
    		Fin Si
    	Fin Si
    	
    	valorFinal = valorInicial - descuento
    	
    	Imprima "El valor inicial es: ", valorInicial 
    	Imprima "El valor del descuento es: ", descuento
    	Imprima "El valor final es: ", valorFinal
    Fin
    ```

    |   marca   | precio | cantidad | valorInicial | descuento | valorFinal |
    | :-------: | :----: | :------: | :----------: | :-------: | :--------: |
    | Goodyear  | 7.000  |    12    |    84.000    |  10.920   |   73.080   |
    |  Pirelli  | 2.000  |    8     |    16.000    |   1.920   |   14.080   |
    | Michellin | 4.800  |    16    |    76.800    |     0     |   76.800   |

12. El ministerio de salud requiere un algoritmo que permita determinar qué tipo de vacuna (A, B o C) debe aplicar a una persona, considerando que, si es menor de 10 años, sin importar el sexo, se le aplica la vacuna tipo A. si tiene entre 10 y 59, y es mujer, se le aplica la B, y si es hombre, la A. Si es mayor de 60 años, se le aplica la vacuna tipo C, sin importar el sexo.

    ```
    Inicio
    	Entero edad
    	Cadena sexo
    	
    	Imprima "Ingrese la edad del paciente."
    	Lea edad
    	
    	Si (edad < 10) Entonces
    		Imprima "Al paciente se le debe aplicar la vacuna A."
    	Sino 
    		Si (edad < 60)  Entonces
    			Imprima "Ingrese el sexo del paciente."
    			Lea sexo
    			
    			Si (sexo == "Femenino") Entonces
    				Escribir "Al paciente se le debe aplicar la vacuna B."
     			SiNo
    				Escribir "Al paciente se le debe aplicar la vacuna A."
    			FinSi
    		SiNo
    			Escribir "Al paciente se le debe aplicar la vacuna C."
    		FinSi
    	FinSi	
    Fin
    ```

    | edad |   sexo    |                   Salida                    |
    | :--: | :-------: | :-----------------------------------------: |
    |  25  | Masculino | Al paciente se le debe aplicar la vacuna A. |
    |  8   |           | Al paciente se le debe aplicar la vacuna A. |
    |  63  |           | Al paciente se le debe aplicar la vacuna C. |


# **Estructura Switch (Case)**



Las estructuras de comparación múltiples, es una toma de decisión especializada que permiten evaluar una variable con distintos posibles resultados, ejecutando para cada caso una serie de instrucciones especificas. La forma es la siguiente:

```
Segun Caso (<Selector>)
    Caso 1:
        <Instrucciones>
    Caso 2:
        <Instrucciones>
    Caso <Otros casos>:
        <Instrucciones>
    Por Defecto:
        <Instrucciones>
Fin Caso
```

- **Según Caso** indica el inicio de la instrucción de selección.
- **Caso:** se compara el valor de la variable selector con el indicador del caso y se ejecutan las instrucciones solo si estos valores coinciden.
- **Por defecto: **instrucciones a ejecutar si la variable selector no coincide con ninguno de los indicadores designados.
- **Fin Caso:** indica el fin de la instrucción de selección.

## Aspectos a tener en cuenta

* Al llegar a la estructura CASO, la variable que hace las veces de selector debe tener
  asignado un valor.
* Al entrar a la estructura CASO sólo se ejecuta una de las secuencias: aquélla que coincida
  con el valor del selector.

## Ejercicios propuestos

1. Calcular e imprimir el salario de un empleado, a partir de las horas extras trabajadas en la semana y la clase a la que pertenece:

  * Clase A: Se les paga $13.000 por hora y se hace una retención del 5%.
  * Clase B: Se les paga $9.000 por hora y se hace una retención del 4%.
  * Clase C: Se les paga $7.000 por hora y se hace una retención del 3%.
  * Clase D: Se les paga $4.000 por hora y se hace una retención del 2%.

  ```
  Inicio
      Real horasTrabajadas, salarioBruto, retencion, salarioNeto
      Caracter clase
      
      Imprima "Ingrese la clase a la que pertenece el empleado (A, B, C, D)."
      Lea clase
      Imprima "Ingrese las horas trabajadas en la semana."
      Lea horasTrabajadas
  	
  	Segun Caso (clase)
          Caso 'A':
  			salarioBruto = horasTrabajadas * 13000
  			retencion = salarioBruto * 0.05
          Caso 'B':
  			salarioBruto = horasTrabajadas * 9000
  			retencion = salarioBruto * 0.04
          Caso 'C':
  			salarioBruto = horasTrabajadas * 7000
  			retencion = salarioBruto * 0.03
          Caso 'D':
  			salarioBruto = horasTrabajadas * 4000
  			retencion = salarioBruto * 0.02
          Por Defecto:
          	Imprima "Ingreso una clase incorrecta."
  	Fin Caso
  	
  	salarioNeto = salarioBruto - retencion
  	
  	Imprima "El salario del empleado es: ", salarioNeto
  Fin
  ```

| clase | horasTrabajadas | salarioBruto | retencion | salarioNeto |                               |
| :---: | :-------------: | :----------: | :-------: | :---------: | :---------------------------: |
|   A   |       24        |   312.000    |  15.600   |   296.400   |                               |
|   B   |        2        |    18.000    |    720    |   17.280    |                               |
|   C   |        5        |    35.000    |   1.050   |   33.950    |                               |
|   D   |        8        |    32.000    |    640    |   31.360    |                               |
|   E   |                 |              |           |             | Ingreso una clase incorrecta. |

2. La secretaria de tránsito, tiene clasificadas las diferentes multas que se sancionan así:

  * A: 1 salario mínimo.
  * B: 1 ½ salarios mínimos.
  * C: 2 salarios mínimos.
  * D: 2 ½ salarios mínimos.
  * E: 3 salarios mínimos.

  Hacer un algoritmo que le permita al usuario ingresar el código de la sanción y le muestre el valor total (en pesos) que deberá pagar.

  ```
  Inicio
  	Real total
  	Caracter codigo
  	
  	Imprima "Ingrese el código de la sanción (A, B, C, D, E)."
  	Lea codigo
  	
  	Segun Caso (codigo)
  		Caso 'A':
  			total = 908526 * 1
  		Caso 'B':
  			total = 908526 * 1.5
  		Caso 'C':
  			total = 908526 * 2
  		Caso 'D':
  			total = 908526 * 2.5
  		Caso 'E':
  			total = 908526 * 3
  		Por Defecto:
  			Imprima "Ingreso un código incorrecto."
  	Fin Caso
  	
  	Imprima "El total a pagar es: ", total
  Fin
  ```

| codigo |   total   |                               |
| :----: | :-------: | :---------------------------: |
|   A    |  908.526  |                               |
|   B    | 1.362.789 |                               |
|   C    | 1.817.052 |                               |
|   D    | 2.271.315 |                               |
|   E    | 2.725.578 |                               |
|   F    |           | Ingreso un código incorrecto. |

3. Hacer un algoritmo que permita seleccionar un número de un menú y de acuerdo con este realice.

  * 1: calcular el área de un triángulo.
  * 2: calcular el área de un cuadrado.
  * 3: calcular el área de un rectángulo.
  * 4: calcular el área de un circulo.

  ```
  Inicio
  	Real base, altura, lado, radio, area
  	Entero menu
  	
  	Imprima "Ingrese una opción (1, 2, 3, 4)."
  	Lea menu
  	
  	Segun Caso (menu)
  		Caso 1:
  			Imprima "Ingrese la medida de la base del triángulo."
  			Lea base
  			Imprima "Ingrese la medida de la altura del triángulo."
  			Lea altura
  			area = (base * altura) / 2
  			Imprima "El área del triángulo es: ", area
  		Caso 2:
  			Imprima "Ingrese la medida de uno de los lados del cuadrado."
  			Lea lado
  			area = lado * lado
  			Imprima “El área del cuadrado es: ”, area
  		Caso 3:
  			Imprima "Ingrese la medida de la base del rectángulo."
  			Lea base
  			Imprima "Imprima la medida de la altura del recángulo."
  			Lea altura
  			area = base * altura
  			Imprima "El área del rectángulo es: ", area
  		Caso 4:
  			Imprima "Ingrese la medida del radio del círculo."
  			Lea radio
  			area = radio * radio * 3,14
  			Imprima "El área del circulo es: ", area
  	Fin Caso
  Fin
  ```

| menu | base | altura | lado | radio |  area  |
| :--: | :--: | :----: | :--: | :---: | :----: |
|  1   |  3   |   4    |  -   |   -   |   6    |
|  2   |  -   |   -    |  8   |   -   |   64   |
|  3   |  6   |   4    |  -   |   -   |   24   |
|  4   |  -   |   -    |  -   |  4,5  | 63,585 |

4. Hacer un algoritmo que permita leer un resultado de una evaluación (A, B, C, D, E) y permita imprimir su equivalente en número.

   * A: 5
   * B: 4,5
   * C: 3,5
   * D: 2,5
   * E: 1

   ```
   Inicio
       Caracter resultado
       Imprima "Ingrese el resultado de la evaluación (A, B, C, D, E)."
       Lea resultado
       
       Segun Caso (resultado)
           Caso 'A':
           	Imprima "Su nota es A que equivale a 5."
           Caso 'B':
           	Imprima "Su nota es B que equivale a 4,5."
           Caso 'C':
           	Imprima "Su nota es B que equivale a 3,5."
           Caso 'D':
           	Imprima "Su nota es D que equivale a 2,5."
           Caso 'E':
           	Imprima "Su nota es E que equivale a 1."
           Por Defecto:
           	Imprima "Ingreso una opción incorrecta."
       Fin Caso
   Fin
   ```

   | resultado |                                  |
   | :-------: | :------------------------------: |
   |     A     |  Su nota es A que equivale a 5.  |
   |     B     | Su nota es B que equivale a 4,5. |
   |     C     | Su nota es B que equivale a 3,5. |
   |     D     | Su nota es D que equivale a 2,5. |
   |     E     |  Su nota es E que equivale a 1.  |
   |     F     |  Ingreso una opción incorrecta.  |

# **Estructuras cíclicas**



Se llaman problemas repetitivos o cíclicos a aquellos en cuya solución es necesario utilizar un mismo conjunto de acciones que se puedan ejecutar una cantidad específica de veces. Esta cantidad puede ser fija (previamente determinada por el programador) o puede ser variable (estar en función de algún dato dentro del programa).

# **Ciclo mientras**



Son aquellos en que el numero de iteraciones no se conoce con exactitud, ya que esta dado en función de un dato dentro del programa.

Esta es una estructura que repetirá un proceso durante N veces, donde N puede ser fijo o variable. Para esto, la instrucción se vale de una condición que es la que debe cumplirse para que se siga ejecutando. Cuando la condición ya no se cumple, entonces ya no se ejecuta el proceso. La forma de esta estructura es la siguiente:

```
Mientras (<Condicion>) Haga
	<Instrucciones>
Fin Mientras
```

## Conceptos de contadores y acumuladores

Ya hemos visto que las variables se puede clasificar de acuerdo a su contenido (numéricas, alfanuméricas y lógicas), pero también es posible clasificarlas según su uso:

- **Contadores:** se utilizan para llevar el control del numero de ocasiones en que se realiza una operación o se cumple una condición. Con los incrementos generalmente de uno en uno.

  De esta forma el incremento se hará con el valor que se le indique.

  ```
  contador = contador + <valor de incremento>
  ```

  De la siguiente forma el contador se incrementará de 1 en 1:

  ```
  contador++
  ```

  También es posible disminuir el valor de un contador en caso de ser necesario.

  ```
  contador = contador - <valor de decremento>
  ```

  Una forma abreviada de escribir la expresión anterior es:

  ```
  contador--
  ```

- **Acumuladores:** forma que toma una variable y que sirve para llevar la suma acumulativa de una serie de valores que se van leyendo o calculando progresivamente.

  ```
  acomulador = acomulador + <valor a acomular>
  ```

  Una forma abreviada de escribir la expresión anterior es:

  ```
  acomulador += <valor a acomular>
  ```

  La diferencia con el contador radica en que el incremento o disminución de cada suma es variable en lugar de constante.

* **Bandera:** es una variable cuyo valor es asignado por el programador para indicar si se debe continuar con la ejecución del programada, este también debe indicar cuando cambiar su valor.

  ```
  bandera = "Si"
  ```

  Los valores escogidos para la bandera pueden ser de cualquier tipo de dato.

## Aspectos a tener en cuenta

* El esquema cuantitativo se implementa a través de un contador, la expresión lógica que
  gobierna el ciclo se establece de acuerdo al valor inicial que se le asigne a éste.
* Los contadores y acumuladores deben partir de un valor inicial.
* Una vez que se entra a un ciclo, éste debe ejecutar todo el conjunto de instrucciones que lo
  componen.
* En la implementación de cualquiera de los dos esquemas, las variables que están
  involucradas en la expresión lógica deben tener almacenado un valor.
* Cuando existen cálculos totales, algunos se hacen dentro del ciclo y otros pueden hacerse
  fuera del ciclo.
* El uso de una bandera exige que ésta tenga asignado un valor en el momento de evaluarse.
* Si un ciclo ya cumplió su misión, para que este termine antes de que la condición en forma
  normal sea falsa, es necesario alterar la expresión lógica.

## Ejercicios propuestos

1. Hacer un algoritmo que imprima los primeros 10 números pares.

   ```
   Inicio
       Entero contador, par
       
       par = 2
       contador = 0
       
       Mientras (contador < 10) Haga
       	Imprima par
   		par += 2
   		contador++
       Fin Mientras
   Fin
   ```

   | contador | par  |
   | :------: | :--: |
   |    0     |  2   |
   |    1     |  4   |
   |    2     |  6   |
   |    3     |  8   |
   |    4     |  10  |
   |    5     |  12  |
   |    6     |  14  |
   |    7     |  16  |
   |    8     |  18  |
   |    9     |  20  |
   |    10    |  22  |

2. Hacer un algoritmo que imprima los primeros N números impares.

   ```
   Inicio
   	Entero impar
   	Cadena bandera
   	bandera = "Si"
   	impar = 1
   	Mientras (bandera == "Si") Haga
   		Imprima impar
   		impar += 2
   		Imprima "¿Desea continuar?"
   		Lea bandera
   	Fin mientras
   Fin
   ```

   | impar | bandera |
   | :---: | :-----: |
   |   1   |   Si    |
   |   3   |   Si    |
   |   5   |   Si    |
   |   7   |   Si    |
   |       |   No    |

3. Hacer un algoritmo que imprima la siguiente secuencia (1, 2, 2, 4, 3, 6, 4, 8…) hasta N.

   ```
   Inicio
   	Entero A, B
   	Cadena bandera
   	A = 1
   	B = 2
   	bandera = "Si"
   	Mientras (bandera == "Si") Haga
   		Imprima A
   		A++
   		Imprima B
   		B += 2
   		Imprima "¿Desea continuar?"
   		Lea bandera
   	Fin Mientras
   Fin
   ```

   |  A   |  B   | bandera |
   | :--: | :--: | :-----: |
   |  1   |  2   |   Si    |
   |  2   |  4   |   Si    |
   |  3   |  6   |   Si    |
   |  4   |  8   |   Si    |
   |  5   |  10  |   No    |

4. Hacer un algoritmo que imprima 10 números de la serie Fibonacci (1, 1, 2, 3, 5, 8, 13…).

   ```
   Inicio
       Entero contador, A, B, C
       contador = 0
       A = 0
       B = 1
       Imprima B
       Mientras (contador < 9) Haga
           C = A + B
           Imprima C
           A = B
           B = C
           contador++
       Fin Mientras
   Fin
   ```

   | contador |  A   |  B   |  C   |
   | :------: | :--: | :--: | :--: |
   |    0     |  0   |  1   |  1   |
   |    1     |  1   |  1   |  2   |
   |    2     |  1   |  2   |  3   |
   |    3     |  2   |  3   |  5   |
   |    4     |  3   |  5   |  8   |
   |    5     |  5   |  8   |  13  |
   |    6     |  8   |  13  |  21  |
   |    7     |  13  |  21  |  34  |
   |    8     |  21  |  34  |  55  |
   |    9     |  34  |  55  |      |

5. Hacer un algoritmo que lea un número (entero) e imprima su cuadrado utilizando sumas únicamente.

   ```
   Inicio
   	Entero contador, numero, cuadrado
   	Imprima "Ingrese un número."
   	Lea numero
   	contador = 0
   	cuadrado = 0;
   	Mientras (contador < numero) Haga
   		cuadrado += numero
   		contador++
   	Fin Mientras
   	Imprima "El cuadrado es: ", cuadrado
   Fin
   ```

   | contador | numero | cuadrado |
   | :------: | :----: | :------: |
   |    0     |   3    |    0     |
   |    1     |        |    3     |
   |    2     |        |    6     |
   |    3     |        |    9     |

   | contador | numero | cuadrado |
   | :------: | :----: | :------: |
   |    0     |   5    |    0     |
   |    1     |        |    5     |
   |    2     |        |    10    |
   |    3     |        |    15    |
   |    4     |        |    20    |
   |    5     |        |    25    |

6. Hacer un algoritmo que le N números e imprima la cantidad de pares.

   ```
   Inicio
   	Real numero
   	Entero contador
   	Cadena bandera
   	
   	contador = 0
   	bandera = "Si"
   	
   	Mientras (bandera == "Si") Haga
   		Imprima "Ingrese un número."
   		Lea numero
   		
   		Si (numero MOD 2 == 0) Entonces
   			contador++
   		Fin Si
   		
   		Imprima "¿Desea continuar?"
   		Lea bandera
   	Fin Mientras
   	
   	Imprima "La cantidad de pares es: ", contador
   Fin
   ```

   | numero | contador | bandera |
   | :----: | :------: | :-----: |
   |        |    0     |   Si    |
   |   10   |    1     |   Si    |
   |   8    |    2     |   Si    |
   |   3    |    -     |   Si    |
   |   12   |    3     |   No    |

7. Hacer un algoritmo que imprima la siguiente serie: (10, 13, 19, 28, 40…) hasta N.

   ```
   Inicio
   	Entero A, B
   	Cadena bandera
   	bandera = "Si"
   	A = 10
   	B = 3
   	Mientras (bandera == "Si") Haga
   		Imprima A
   		A += B
   		B += 3
   		Imprima "¿Desea continuar?"
   		Lea bandera
   	Fin Mientras
   Fin
   ```

   | bandera |  A   |  B   |
   | :-----: | :--: | :--: |
   |   Si    |  10  |  3   |
   |   Si    |  13  |  6   |
   |   Si    |  19  |  9   |
   |   Si    |  28  |  12  |
   |   No    |  40  |  15  |

8. Se tienen las donaciones en dinero de un grupo indeterminado de personas. Elabore un algoritmo que permita calcular le promedio de la donación y cuantas personas realizaron la misma.

   ```
   Inicio	
   	Real valorDonacion, promedio, totalRecaudado
   	Entero cantidadDonantes
   	Cadena bandera
   	
   	totalRecaudado = 0
   	cantidadDonantes = 0
   	bandera = "Si"
   	
   	Mientras (bandera == "Si") Haga	
   		Imprima "Ingrese el valor de la donación"
   		Lea valorDonacion
   		
   		cantidadDonantes++
   		totalRecaudado += valorDonacion
   		
   		Imprima "¿Desea agregar otra donación?"
   		Lea bandera
   	Fin Mientras
   	
   	promedio = totalRecaudado / cantidadDonantes
   	
   	Imprima "El promedio de la donación es: ", promedio
   	Imprima "La cantidad de personas que donaron es: ", cantidadDonantes
   Fin
   ```

   | bandera | cantidadDonantes | valorDonacion | promedio | totalRecaudado |
   | :-----: | :--------------: | :-----------: | :------: | :------------: |
   |   Si    |        0         |               |          |       0        |
   |   Si    |        1         |     1.000     |          |     1.000      |
   |   Si    |        2         |     2.000     |          |     3.000      |
   |   No    |        3         |     3.000     |  2.000   |     5.000      |

9. Se tiene N información para cada uno de los N estudiantes de la universidad:

   * Edad
   * Sexo (1: Masculino, 2: Femenino)
   * Carrera (1: Ingeniería, 2: Otra carrera)

   Hacer un algoritmo que obtenga e imprima:

     * Promedio de edad de los estudiantes de ingeniería.
     * Porcentaje de hombres en la universidad.
     * Porcentaje de mujeres que estudian ingeniería.

   ```
   Inicio
   	Entero edad, sexo, carrera, sumaEdades, CHU, CMI, CE, CEI
   	Real PEEI, PHU, PMI
   	Cadena bandera
   	
   	bandera = "Si"
   	
   	sumaEdades = 0
   	CHU = 0
   	CMI = 0
   	CE = 0
   	CEI = 0
   	
   	Mientras (bandera == "Si") Haga
   		Imprima "Ingrese la edad del estudiante: "
   		Lea edad
   		Imprima "Ingrese el sexo del estudiante (1: Masculino, 2: Femenino): "
   		Lea sexo
   		Imprima "Ingrese la carrera que esta cursando (1: Ingeniería, 2: Otra carrera): "
   		Lea carrera
   		
   		CE++
   		
   		Si (carrera = 1) Entonces
   			sumaEdades += edad
   			CEI++
   		FinSi
   		
   		Si (sexo == 1) Entonces
   			CHU++
   		FinSi
   		
   		Si ((sexo = 2) y (carrera = 1)) Entonces
   			CMI++
   		FinSi
   		
   		Imprima "¿Desea agregar otro estudiante?"
   		Lea bandera
   	Fin Mientras
   	
   	PEEI = sumaEdades / CEI
   	PHU = (CHU / CE) * 100
   	PMI = (CMI / CE) * 100
   	
   	Imprima "El promedio de edad de los estudiantes de ingenierí es: ", PEEI
   	Imprima "El porcentaje de hombres en la universidad es: ", PHU
   	Imprima "El porcentaje de mujeres que estudian ingeniería es: ", PMI
   Fin
   ```

   | bandera |  edad  | sexo  | carrera | sumaEdades |  CHU  |  CMI  |  CE   |  CEI  | PEEI | PHU  | PMI  |
   | :-----: | :----: | :---: | :-----: | :--------: | :---: | :---: | :---: | :---: | :--: | :--: | :--: |
   | ~~Si~~  | ~~25~~ | ~~1~~ |  ~~1~~  |   ~~0~~    | ~~0~~ | ~~0~~ | ~~0~~ | ~~0~~ |  28  |  50  |  25  |
   | ~~Si~~  | ~~35~~ | ~~1~~ |  ~~1~~  |   ~~25~~   | ~~1~~ |   1   | ~~1~~ | ~~1~~ |      |      |      |
   | ~~Si~~  | ~~24~~ | ~~2~~ |  ~~1~~  |   ~~60~~   |   2   |       | ~~2~~ | ~~2~~ |      |      |      |
   | ~~Si~~  |   22   |   2   |    2    |     84     |       |       | ~~3~~ |   3   |      |      |      |
   |   No    |        |       |         |            |       |       |   4   |       |      |      |      |

# **Ciclo Para**



Son aquellos en que el número de iteraciones se conoce antes de ejecutarse el ciclo. La forma de esta estructura es la siguiente:

```
Para (<variable> = <expresion1>, <variable> Hasta <expresion2>, Con paso <expresion3>) Haga
	<Instrucciones>
Fin Para
```

* **Variable:** variable numérica entera que sirve de control del ciclo (contador en la estructura mientras).
* **Expresion1:** valor inicial del contador.
* **Expresion2:** valor final del contador o número de repeticiones del ciclo.
* **Expresion3: **expresión entera que indica el valor del incremento o disminución de la variable de control; si el valor es uno se puede omitir o si se omite el paso, significa que la variable aumentará de uno en uno.

## Ejercicios propuestos

1. Hacer un algoritmo que imprima los múltiplos de 7 que hay entre 150 y 200.

   ```
   Inicio
   	Entero x
   	Para (x = 150, x <= 200, 1) Haga
   		Si (x MOD 7 == 0) Entonces
   			Imprima x
   		Fin Si
   	Fin Para
   Fin
   ```

   |    x    |
   | :-----: |
   | ~~150~~ |
   | ~~151~~ |
   |    ⁝    |
   |   154   |
   |    ⁝    |
   |   161   |
   |    ⁝    |
   | ~~200~~ |
   |   201   |

2. Hacer un algoritmo que imprima la secuencia (10, 2, 8, 4, 6, 6, 4, 8, 2, 10). Además de imprimir su suma.

   ```
   Inicio
   	Entero x, A, B, suma
   	A = 10
   	B = 2
   	suma = 0
   	Para (x = 1, x <= 5, 1) Haga
   		Imprima A
   		Imprima B
   		suma = suma + A + B
   		A -= 2
   		B += 2
   	Fin Para
   Fin
   ```

   |  x   |  A   |  B   | suma |
   | :--: | :--: | :--: | :--: |
   |  1   |  10  |  2   |  0   |
   |  2   |  8   |  4   |  12  |
   |  3   |  6   |  6   |  24  |
   |  4   |  4   |  8   |  36  |
   |  5   |  2   |  10  |  48  |
   |  6   |  0   |  12  |  60  |

3. Hacer un algoritmo que permita imprimir 10 números de la serie Fibonacci.

   ```
   Inicio
       Entero x, A, B
       A = 0
       B = 1
       Para (x = 1, x < =10, 1) Haga
           Imprima B
           B = A + B
           A = B - A
       Fin Para
   Fin
   ```

   |  x   |  A   |  B   |
   | :--: | :--: | :--: |
   |  1   |  0   |  1   |
   |  2   |  1   |  1   |
   |  3   |  1   |  2   |
   |  4   |  2   |  3   |
   |  5   |  3   |  5   |
   |  6   |  5   |  8   |
   |  7   |  8   |  13  |
   |  8   |  13  |  21  |
   |  9   |  21  |  34  |
   |  10  |  34  |  55  |
   |  11  |  55  |  89  |

4. Hacer un algoritmo que imprima los números del 100 al 50.

   ```
   Inicio
   	Entero x
   	Para (x = 100, x >= 50, -1) Haga
   		Imprima x
   	Fin Para
   Fin
   ```

   |  x   |
   | :--: |
   | 100  |
   |  99  |
   |  98  |
   |  ⁝   |
   |  51  |
   |  50  |
   |  49  |

5. Hacer un algoritmo que lea un número e imprima su factorial.

   ```
   Inicio
   	Entero x, numero, factorial
   	Imprima "Ingrese un número."
   	Lea numero
   	factorial = 1
   	Para (x = 1, x <= numero, 1) Haga
   		factorial = factorial * x
   	Fin Para
   	Imprima "El factorial del número ingresado es: ", factorial
   Fin
   ```

   | numero |   x   | factorial |
   | :----: | :---: | :-------: |
   |   5    | ~~1~~ |   ~~1~~   |
   |        | ~~2~~ |   ~~1~~   |
   |        | ~~3~~ |   ~~2~~   |
   |        | ~~4~~ |   ~~6~~   |
   |        | ~~5~~ |  ~~24~~   |
   |        |   6   |    120    |

   | numero |   x   | factorial |
   | :----: | :---: | :-------: |
   |   7    | ~~1~~ |   ~~1~~   |
   |        | ~~2~~ |   ~~1~~   |
   |        | ~~3~~ |   ~~2~~   |
   |        | ~~4~~ |   ~~6~~   |
   |        | ~~5~~ |  ~~24~~   |
   |        | ~~6~~ |  ~~120~~  |
   |        | ~~7~~ |  ~~720~~  |
   |        |   8   |   5.040   |

6. Hacer un algoritmo que lea 10 notas de un estudiante y al final imprima:

   * Promedio.
   * Cantidad de notas aprobadas.
   * Cantidad de notas reprobadas.
   * Nota más alta.
   * Nota más baja.

   ```
   Inicio
   	Entero x, cantidadAprobadas, cantidadReprobadas
   	Real nota, sumaNotas, promedio, notaMasAlta, notaMasBaja
   	
   	sumaNotas = 0
   	cantidadAprobadas = 0
   	cantidadReprobadas = 0
   	notaMasAlta = 0
   	notaMasBaja = 5
   	
   	Para (x = 1, x <= 10, 1) Haga
   		Imprima "Ingrese nota."
   		Lea nota
   		
   		sumaNotas += nota
   		
   		Si (nota >= 3.5) Entonces
   			cantidadAprobadas++
   		Sino
   			cantidadReprobadas++
   		Fin Si
   		
   		Si (nota > notaMasAlta) Entonces
   			notaMasAlta = nota
   		Fin Si
   		
   		Si (nota < notaMasBaja) Entonces
   			notaMasBaja = nota
   		Fin Si
   	Fin Para
   	
   	promedio = sumaNotas / 10
   	
   	Imprima "El promedio del estudiante es: ", promedio
   	Imprima "La cantidad de notas aprobadas es: ", cantidadAprobadas
   	Imprima "La cantidad de notas reprobadas es: ", cantidadReprobadas
   	Imprima "La nota más alta es: ", notaMasAlta
   	Imprima "La nota más baja es: ", notaMasBaja
   Fin
   ```

   |   x    |  nota   | sumaNotas | promedio | cantidadAprobadas | cantidadReprobadas | notaMasAlta | notaMasBaja |
   | :----: | :-----: | :-------: | :------: | :---------------: | :----------------: | :---------: | :---------: |
   | ~~1~~  | ~~2.8~~ |   ~~0~~   |   3.51   |       ~~0~~       |       ~~0~~        |    ~~0~~    |    ~~5~~    |
   | ~~2~~  | ~~3.2~~ |  ~~2.8~~  |          |       ~~1~~       |       ~~1~~        |   ~~2.8~~   |   ~~2.8~~   |
   | ~~3~~  | ~~4.6~~ |   ~~6~~   |          |       ~~2~~       |       ~~2~~        |   ~~3.2~~   |     1.6     |
   | ~~4~~  | ~~3.9~~ | ~~10.6~~  |          |       ~~3~~       |       ~~3~~        |   ~~4.6~~   |             |
   | ~~5~~  | ~~1.6~~ | ~~14.5~~  |          |       ~~4~~       |         4          |      5      |             |
   | ~~6~~  | ~~1.9~~ | ~~16.1~~  |          |       ~~5~~       |                    |             |             |
   | ~~7~~  | ~~3.8~~ |  ~~18~~   |          |         6         |                    |             |             |
   | ~~8~~  | ~~4.2~~ | ~~21.8~~  |          |                   |                    |             |             |
   | ~~9~~  | ~~4.1~~ |  ~~26~~   |          |                   |                    |             |             |
   | ~~10~~ |    5    | ~~30.1~~  |          |                   |                    |             |             |
   |   11   |         |   35.1    |          |                   |                    |             |             |

7. Hacer un algoritmo que lea 50 números e imprima:
   * Cantidad de pares.
   * Cantidad de múltiplos de 6.
   * Cantidad de mayores a 40.
   * Suma de los menores a 20.

   ```
   Inicio
   	Entero x, pares, multiplos, mayores, sumaMenores
   	Real numero
   	pares = 0
   	multiplos = 0
   	mayores = 0
   	suma = 0
   	Para (x = 1, x <= 50, 1) Haga
   		Si (numero MOD 2 == 0) Entonces
   			pares++
   		Fin Si
   		
   		Si (numero MOD 6 == 0) Entonces
   			multiplos++
   		Fin Si
   		
   		Si (numero > 40) Entonces
   			mayores++
   		Fin Si
   		
   		Si (numero < 20) Entonces
   			sumaMenores += numero
   		Fin Si
   	Fin Para
   	Imprima "La cantidad de números pares es: ", pares
   	Imprima "La cantidad de números multiplos de 6 es: ", multiplos
   	Imprima "La cantidad de números mayores a 40 es: ", mayores
   	Imprima "La suma de los números menores a 20 es: ", menores"
   Fin
   ```

   |   x   | numero | pares | multiplos | mayores | sumaMenores |
   | :---: | :----: | :---: | :-------: | :-----: | :---------: |
   | ~~1~~ | ~~26~~ | ~~0~~ |     0     |    0    |    ~~0~~    |
   | ~~2~~ | ~~35~~ | ~~1~~ |           |         |   ~~14~~    |
   | ~~3~~ | ~~14~~ | ~~2~~ |           |         |   ~~18~~    |
   | ~~4~~ | ~~4~~  |   3   |           |         |     27      |
   |   5   |   9    |       |           |         |             |

   **Nota:** la prueba de escritorio solo se realizó con 5 números, ya que hacerlo con los 50 es demasiado larga.

# **Ciclos Anidados**

## Ejercicios propuestos

1. En un grupo hay 15 estudiantes y para cada uno se leen 5 notas. Hacer un algoritmo que imprima:
   * Promedio de notas del estudiante.
   * Promedio de notas del grupo.
   * Cantidad de notas aprobadas en el grupo.
   * Cantidad de notas reprobadas en el grupo.
   * Estudiante con el promedio más alto.
   * Estudiante con el promedio más bajo.
   
   ```
   Inicio
   	Entero x, z, notasAprobadas, notasReprobadas
   	Real nota, sumaEstudiante, sumaGrupo, promedioEstudiante, promedioGrupo, promedioMasAlto, 			 promedioMasBajo
   	Cadena nombre, ePromedioMasAlto, ePromedioMasBajo
   	
   	notasAprobadas = 0
   	notasReprobadas = 0
   	sumaGrupo = 0
   	promedioMasAlto = 0
   	promedioMasBajo = 5
   	
   	Para (x = 1, x <= 15, 1) Haga
   		
   		sumaEstudiante = 0
   		
   		Escribir "Ingrese el nombre del estudiante: "
   		Leer nombre
   		
   		Para (x = 1, x <= 5, 1) Haga
   			
   			Escribir "Ingrese la nota del estudiante."
   			Leer nota
   			
   			sumaEstudiante += nota
   			
   			Si (nota >= 3.5) Entonces
   				notasAprobadas++
   			SiNo
   				notasReprobadas++
   			Fin Si
   			
   		Fin Para
   		
   		promedioEstudiante = sumaEstudiante / 5
   		
   		Imprima "El promedio del estudiante es: ", promedioEstudiante
   		
   		sumaGrupo += promedioEstudiante
   		
   		Si (promedioEstudiante > promedioMasAlto) Entonces
   			promedioMasAlto = promedioEstudiante
   			ePromedioMasAlto = nombre
   		Fin Si
   		
   		Si (promedioEstudiante < promedioMasBajo) Entonces
   			promedioMasBajo = promedioEstudiante
   			ePromedioMasBajo = nombre
   		Fin Si
   		
   	Fin Para
   	
   	promedioGrupo = sumaGrupo / 15
   	
   	Imprima "El promedio del grupo es: ", promedioGrupo
   	Imprima "La cantidad de notas aprobadas en el grupo son: ", notasAprobadas
   	Imprima "La cantidad de notas reprobadas en el grupo son: ", notasReprobadas
   	Imprima "El estudiante con el promedio más alto es: ", ePromedioMasAlto
   	Imprima "El estudiante con el promedio más bajo es: ", ePromedioMasBajo
   Fin
   ```
   
   |   x   |   z   | notasAprobadas | notasReprobadas | nota  | sumaEstudiante | sumaGrupo | promedioEstudiante | promedioGrupo | promedioMasAlto | promedioMasBajo |  nombre  | ePromedioMasAlto | ePromedioMasBajo |
   | :---: | :---: | :------------: | :-------------: | :---: | :------------: | :-------: | :----------------: | :-----------: | :-------------: | :-------------: | :------: | :--------------: | :--------------: |
   | ~~1~~ | ~~1~~ |     ~~0~~      |      ~~0~~      | ~~4~~ |     ~~0~~      |   ~~0~~   |        3.6         |               |      ~~0~~      |      ~~5~~      | ~~Jhon~~ |     ~~Jhon~~     |     ~~Jhon~~     |
   | ~~2~~ | ~~2~~ |     ~~1~~      |      ~~1~~      | ~~3~~ |     ~~4~~      |  ~~3.6~~  |                    |               |     ~~3.6~~     |     ~~3.6~~     |          |                  |                  |
   | ~~3~~ | ~~3~~ |     ~~2~~      |                 | ~~4~~ |     ~~7~~      |           |                    |               |                 |                 |          |                  |                  |
   |   4   |   4   |                |                 |       |       11       |           |                    |               |                 |                 |          |                  |                  |
   |       |       |                |                 |       |                |           |                    |               |                 |                 |          |                  |                  |
   | ~~1~~ |       |     ~~3~~      |      ~~2~~      | ~~3~~ |     ~~0~~      |  ~~7.6~~  |         4          |               |        4        |                 | ~~Dani~~ |       Dani       |                  |
   | ~~2~~ |       |       4        |                 | ~~4~~ |     ~~3~~      |           |                    |               |                 |                 |          |                  |                  |
   | ~~3~~ |       |                |                 | ~~5~~ |     ~~7~~      |           |                    |               |                 |                 |          |                  |                  |
   |   4   |       |                |                 |       |       12       |           |                    |               |                 |                 |          |                  |                  |
   |       |       |                |                 |       |                |           |                    |               |                 |                 |          |                  |                  |
   | ~~1~~ |       |                |      ~~3~~      | ~~2~~ |     ~~0~~      |   9.93    |        2.33        |     3.31      |                 |      2.33       |   Caro   |                  |       Caro       |
   | ~~2~~ |       |                |      ~~4~~      | ~~3~~ |     ~~2~~      |           |                    |               |                 |                 |          |                  |                  |
   | ~~3~~ |       |                |        5        |   2   |     ~~5~~      |           |                    |               |                 |                 |          |                  |                  |
   |   4   |       |                |                 |       |       7        |           |                    |               |                 |                 |          |                  |                  |
   
2. Hacer un algoritmo que imprima el factorial de N números.

     ```
     Inicio
     	Entero x, numero, factorial
     	Cadena bandera
     	
     	bandera = "Si"
     	
     	Mientras (bandera == "Si") Haga
     	
     		factorial = 1
     		
     		Imprima "Ingrese un número."
     		Lea numero
     		
     		Para (x = 1, x <= n, 1) Hacer
     			factorial *= x
     		Fin Para
     		
     		Imprima "El factorial del número ingresado es: ", factorial
     		
     		Imprima "¿Desea generar conocer el factorial de otro número?"
     		Lea bandera
     	Fin Mientras
     Fin
     ```

     | bandera |  x   | numero | factorial |
     | :-----: | :--: | :----: | :-------: |
     |   Si    |  1   |   4    |     1     |
     |         |  2   |        |     1     |
     |         |  3   |        |     2     |
     |         |  4   |        |     6     |
     |         |  5   |        | <u>24</u> |
     |         |      |        |           |
     |   Si    |  1   |   3    |     1     |
     |         |  2   |        |     1     |
     |         |  3   |        |     2     |
     |         |  4   |        | <u>6</u>  |
     |         |      |        |           |
     |   No    |      |        |           |

3. Hacer un algoritmo que imprima la sumatoria de N números.

     ```
     Inicio
     	Entero x, numero, sumatoria
     	Cadena bandera
     	
     	bandera = "Si"
     	
     	Mientras (bandera == "Si") Haga
     		
     		Imprima "Ingrese un número."
     		Lea numero
     		
     		sumatoria = 0
     		
     		Para (x = 1, x <= numero, 1) Haga
     			sumatoria += x
     		Fin Para
     		
     		Imprima "La sumatoria del número ingresado es: ", sumatoria
     		
     		Imprima "¿Desea generar conocer la sumatoria de otro número?"
     		Lea bandera
     	Fin Mientras
     Fin
     ```

     | bandera |  x   | numero | sumatoria |
     | :-----: | :--: | :----: | :-------: |
     |   Si    |  1   |   5    |     0     |
     |         |  2   |        |     1     |
     |         |  3   |        |     3     |
     |         |  4   |        |     6     |
     |         |  5   |        |    10     |
     |         |  6   |        |    15     |
     |         |      |        |           |
     |   Si    |  1   |   3    |     0     |
     |         |  2   |        |     1     |
     |         |  3   |        |     3     |
     |         |  4   |        |     6     |
     |         |      |        |           |
     |   No    |      |        |           |

4. Elaborar un algoritmo que genere los primeros N números de la serie: (17, 15, 18, 16, 19, 17, 20, 18, 21, 19…).

     ```
     Inicio
     	Entero x, limite, serie
     	serie = 17
     	Imprima "¿Cuántos números desea generar?"
     	Lea limite
     	Para (x = 1, x <= limite, 1) Haga
     		Imprima serie
     		Si (x MOD 2 == 0) Entonces
     			serie += 3
     		Sino
     			serie -= 2
     		Fin Si
     	Fin Para
     Fin
     ```

     | limite |  x   | serie |
     | :----: | :--: | :---: |
     |   5    |  1   |  17   |
     |        |  2   |  15   |
     |        |  3   |  18   |
     |        |  4   |  16   |
     |        |  5   |  19   |
     |        |  6   |  17   |

5. Para las elecciones municipales donde solo hay 5 opciones de resultados (3 candidatos, voto en blanco y voto nulo), se tienen N cantidad de puestos de votación y cada uno de estos tiene N cantidad de mesas. Al finalizar la jornada se requiere un algoritmo que permita determinar lo siguiente:

     * Cantidad de votos por cada opción en cada mesa.
     * Cantidad de votos por cada opción en cada puesto de votación.
     * Cantidad total de votos por cada opción.
     * Cantidad de votos en cada mesa.
     * Cantidad de votos en cada puesto de votación.
     * Cantidad total de votos.
     * Porcentaje total de votos por cada opción.

     ```
     
     ```

     |      |      |      |
     | :--- | ---- | ---- |
     |      |      |      |
     |      |      |      |
     |      |      |      |

6. Un almacén tiene 4 departamentos numerados consecutivamente del 1 al 4, los cuales venden artículos de diferente naturaleza. Por cada artículo se tiene la siguiente información:

   * Código del artículo
   * Código del departamento
   * Cantidad vendida
   * Precio de venta unitario
   * Precio de costo unitario
   * Indicativo que dice si el producto es importado o colombiano (1: colombiano, 2: importado)

   Hacer un algoritmo que determine, por cada departamento por cuántos y por cuáles productos importados se obtuvo una utilidad superior a $1.000.000 y la utilidad total por departamento.

   ```
   Inicio
   	Definir x, CA, CD, CV, indicativo Como Entero
   	Definir PVU, PCU, GI, GN, GTPD Como Real
   	Definir bandera Como Caracter
   	
   	Para (x = 1, x <= 4, 1) Haga
   		
   		bandera = "Si"
   		GTPD = 0
   		
   		Mientras (bandera == "Si") Haga
   			
   			GI = 0
   			GN = 0
   			
   			Imprima "Ingrese el código del artículo: "
   			Lea CA
   			Imprima "Ingrese el código del departamento: "
   			Lea CD
   			Imprima "Ingrese la cantidad vendida: "
   			Lea CV
   			Imprima "Ingrese el precio de venta unitario: "
   			Lea PVU
   			Imprima "Ingrese el precio de costo unitario: "
   			Lea PCU
   			Imprima "Ingrese el indicativo (1: colombiano, 2: importado): "
   			Lea indicativo
   			
   			Si (indicativo == 2) Entonces
   				
   				GI = PVU - PCU
   				
   				Si (GI > 1000000) Entonces
   					Imprima "La cantidad de productos por lo que se obtuvo una utilidad de mas                                  $1'000.000 es: ", CV
   					Imprima "El código del articulo es: ", CA
   				Fin Si
   			SiNo
   				GN = PVU - PCU
   			FinSi
   			
   			GTPD += (GI + GN)
   			
   			Imprima "¿Desea agregar otro producto?"
   			Lea bandera
   		Fin Mientras
   		
   		Imprima "La utilidad total del departamento es: ", GTPD
   		
   	Fin Para
   FinProceso
   ```

   |      |      |      |
   | ---- | ---- | ---- |
   |      |      |      |
   |      |      |      |
   |      |      |      |

8. En una EPS, se atienden diariamente N cantidad de pacientes y cada uno asiste por un concepto diferente. Los conceptos son:

   * Cita médica
   * Cita odontológica
   * Cita con especialista
   * Cita prioritaria
   * Vacunación

   Por cada concepto, el paciente deberá cancelar un copago que depende del nivel salarial:

     * Si el nivel salarial es 1: $2.900
     * Si el nivel salarial es 2: $9.600
     * Si el nivel salarial es 3: $17.000
     * Si el nivel salarial es 4: $26.000

   Elaborar un algoritmo que permita imprimir al finalizar el día:

     * Cantidad de pacientes atendidos en el día.
     * Cantidad de pacientes atendidos por cada concepto.
     * Valor recaudado por cada concepto.
     * Valor recaudado en el día.
     * Porcentaje correspondiente a cada concepto.

# **Arreglos de una dimensión o vectores**



## Ejercicios propuestos

1. Llenar un vector de 10 posiciones e imprimirlo.

   **Solución usando el ciclo Para**:

   ```
   Inicio
   	Entero x, y, vector [10]
   	
   	Para (x = 1, x <= 10, 1) Haga
   		Imprima "Ingrese un número."
   		Lea vector[x]
   	Fin Para
   	
   	Para (y = 1, y <= 10, 1) Haga
   		Imprima vector[y]
   	Fin Para
   Fin
   ```

   |  x   |  y   | vector[10] |
   | :--: | :--: | :--------: |
   |  1   |  1   |     1      |
   |  2   |  2   |     3      |
   |  3   |  3   |     5      |
   |  4   |  4   |     9      |
   |  5   |  5   |     13     |
   |  6   |  6   |     8      |
   |  7   |  7   |     12     |
   |  8   |  8   |     20     |
   |  9   |  9   |     2      |
   |  10  |  10  |     7      |
   |  11  |  11  |            |

   **Solución usando el ciclo Mientras:**

   ```
   Inicio
   	Entero x, y, vector[10]
   	
   	x = 1
   	y = 1
   	
   	Mientras (x <= 10) Haga
   		Imprima "Ingrese un número."
   		Lea vector[x]
   		x++
   	Fin Mientras
   	
   	Mientras (y <= 10) Haga
   		Imprima vector[y]
   		y++
   	Fin mientras
   Fin
   ```

   |  x   |  y   | vector[10] |
   | :--: | :--: | :--------: |
   |  1   |  1   |     1      |
   |  2   |  2   |     3      |
   |  3   |  3   |     5      |
   |  4   |  4   |     9      |
   |  5   |  5   |     13     |
   |  6   |  6   |     8      |
   |  7   |  7   |     12     |
   |  8   |  8   |     20     |
   |  9   |  9   |     2      |
   |  10  |  10  |     7      |
   |  11  |  11  |            |

2. Llenar un vector de 5 posiciones con números enteros e imprimir su suma.

   ```
   Inicio
   	Entero x, vector[5], suma
   	
   	suma = 0
   	
   	Para (x = 1, x <= 5, 1) Haga
   		Imprima "Ingrese un número."
   		Lea vector[x]
   		suma += vector[x]
   	FinPara
   	
   	Imprima "La suma de los elementos en el vector es: ", suma
   Fin
   ```

   |  x   | vector[5] |   suma    |
   | :--: | :-------: | :-------: |
   |  1   |     6     |     0     |
   |  2   |     7     |     6     |
   |  3   |     2     |    13     |
   |  4   |     5     |    15     |
   |  5   |     3     |    20     |
   |  6   |           | <u>23</u> |

3. Hacer un algoritmo que permita llenar un vector de 7 posiciones con números, calcula el promedio e imprima:

    * Cantidad de valores mayores al promedio.
    * Cantidad de valores menores al promedio.
    * Cantidad de valores iguales al promedio.

    ```
    Inicio
    	Real vector[7], promedio, suma
    	Entero x, y, mayores, menores, iguales
    	
    	suma = 0
    	mayores = 0
    	menores = 0
    	iguales = 0
    	
    	Para (x = 1, x <= 7, 1) Haga
    		Imprima "Ingrese un número."
    		Lea vector[x]
    		suma += vector[x]
    	Fin Para
    	
    	promedio = suma / 7
    	
    	Para (y = 1, y <= 7, 1) Haga
    		Si (vector[y] > promedio) Entonces
    			mayores++
    		Sino Si (vector[y] < promedio) Entonces
    				menores++
    			Sino
    				iguales++
    			Fin Si
    		Fin Si
    	Fin Para
    	
    	Imprima "La cantidad de valores mayores al promedio son: ", mayores
    	Imprima "La cantidad de valores menores al promedio son: ", menores
    	Imprima "La cantidad de valores iguales al promedio son: ", iguales
    Fin
    ```

    |   x   |   y   | vector[ 7 ] |  suma  | promedio | mayores | menores | iguales |
    | :---: | :---: | :---------: | :----: | :------: | :-----: | :-----: | :-----: |
    | ~~1~~ | ~~1~~ |      2      | ~~0~~  |   3.42   |  ~~0~~  |  ~~0~~  |    0    |
    | ~~2~~ | ~~2~~ |    ~~4~~    | ~~2~~  |          |  ~~1~~  |  ~~1~~  |         |
    | ~~3~~ | ~~3~~ |      3      | ~~6~~  |          |  ~~2~~  |  ~~2~~  |         |
    | ~~4~~ | ~~4~~ |      7      | ~~9~~  |          |    3    |  ~~3~~  |         |
    | ~~5~~ | ~~5~~ |      2      | ~~16~~ |          |         |  ~~4~~  |         |
    | ~~6~~ | ~~6~~ |      1      | ~~18~~ |          |         |         |         |
    | ~~7~~ | ~~7~~ |      5      | ~~19~~ |          |         |         |         |
    |   8   |   8   |             |   24   |          |         |         |         |

4. Hacer un algoritmo que permita llenar un vector de 10 posiciones con números enteros e imprima:

    * Número mayor y posición en la que se encuentra.
    * Número menor y posición en la que se encuentra.

    ```
    Inicio
    	entero x, y, vector[10], nmayor, nmenor, pmayor, pmenor
    	
    	Para (x = 0, x < 10, 1) Haga
    		Imprima "Ingrese un número entero."
    		Lea vector[x]
    	Fin Para
    	
    	nmayor = vector[0]
    	nmenor = vector[0]
    	
    	Para (y = 0, y < 10, 1) Haga
    		Si (vector[y] > nmayor) Entonces
    			nmayor = vector[y]
    			pmayor = y
    		Fin Si
    		
    		Si (vector[y] < nmenor) Entonces
    			nmenor = vector[y]
    			pmenor = y
    		Fin Si
    	Fin Para
    	
    	Imprima "El número mayor en el vector es: ", nmayor
    	Imprima "La posición en la que se encuentra el número mayor es: ", pmayor
    	Imprima "El número menor en el vector es: ", nmenor
    	Imprima "La posición en la que se encentra el número menor es: ", pmenor	
    Fin
    ```

    |   x   |   y   | vector[10] | nmayor | nmenor | pmayor | pmenor |
    | :---: | :---: | :--------: | :----: | :----: | :----: | :----: |
    | ~~0~~ | ~~0~~ |     7      | ~~7~~  | ~~7~~  | ~~0~~  | ~~0~~  |
    | ~~1~~ | ~~1~~ |     4      | ~~9~~  | ~~4~~  | ~~4~~  | ~~1~~  |
    | ~~2~~ | ~~2~~ |     2      |   13   | ~~2~~  |   5    | ~~2~~  |
    | ~~3~~ | ~~3~~ |     1      |        | ~~1~~  |        | ~~3~~  |
    | ~~4~~ | ~~4~~ |     9      |        |   0    |        |   8    |
    | ~~5~~ | ~~5~~ |     13     |        |        |        |        |
    | ~~6~~ | ~~6~~ |     6      |        |        |        |        |
    | ~~7~~ | ~~7~~ |     8      |        |        |        |        |
    | ~~8~~ | ~~8~~ |     0      |        |        |        |        |
    | ~~9~~ | ~~9~~ |     4      |        |        |        |        |
    |  10   |  10   |            |        |        |        |        |

5. Hacer un algoritmo que permita llenar un vector de 8 posiciones y cree un segundo vector con los cuadrados del primero.

    ```
    Inicio	
    	Entero x, vector[8], cuadrado[8]
    	
    	Para (x = 0, x < 9, 1) Haga
    		Imprima "Ingrese un número entero."
    		Lea vector[x]
    		cuadrado[x] = vector[x] * vector[x]
    	Fin Para
    Fin
    ```

    |   x   | vector[8] | cuadrado[8] |
    | :---: | :-------: | :---------: |
    | ~~0~~ |     2     |      4      |
    | ~~1~~ |     4     |     16      |
    | ~~2~~ |     6     |     36      |
    | ~~3~~ |     8     |     64      |
    | ~~4~~ |    10     |     100     |
    | ~~5~~ |     5     |     25      |
    | ~~6~~ |     3     |      9      |
    | ~~7~~ |     7     |     49      |
    |   8   |           |             |

6. Hacer un algoritmo que permita llenar un vector A un vector B de 9 posiciones cada uno y cree un tercer vector con la suma de los 2 primeros.

    ```
    Inicio
    	Entero A[9], B[9], C[9]
    	
    	Para (x = 0, x < 9, 1) Haga
    		Imprima "Ingrese un número entero."
    		Lea A[x]
    		Imprima "Ingrese un número entero."
    		Lea B[x]
    		C[x] = A[x] + B[x]
    	Fin Para
    Fin
    ```

    |   x   | A[9] | B[9] | C[9] |
    | :---: | :--: | :--: | :--: |
    | ~~0~~ |  2   |  8   |  10  |
    | ~~1~~ |  3   |  2   |  5   |
    | ~~2~~ |  10  |  4   |  14  |
    | ~~3~~ |  8   |  3   |  11  |
    | ~~4~~ |  5   |  5   |  10  |
    | ~~5~~ |  1   |  9   |  10  |
    | ~~6~~ |  4   |  7   |  11  |
    | ~~7~~ |  2   |  6   |  8   |
    | ~~8~~ |  7   |  1   |  8   |
    |   9   |      |      |      |

7. Hacer un algoritmo que permita llenar 2 vectores A y B de 5 posiciones cada uno y cree un vector C con la unión de los 2 primeros.

    ```
    Inicio	
    	Entero x, A[5], B[5],C[10]
    	
    	Para (x = 0, x < 5, 1) Haga
    		Imprima "Ingrese un número."
    		Lea A[x]
    		Imprima "Ingrese un número."
    		Lea B[x]
    		C[x] = A[x]
    		C[x + 5] = B[x]
    	Fin Para
    Fin
    ```

    |   x   | A[5] | B[5] | C[10] |
    | :---: | :--: | :--: | :---: |
    | ~~0~~ |  1   |  8   |   1   |
    | ~~1~~ |  3   |  4   |   3   |
    | ~~2~~ |  5   |  7   |   5   |
    | ~~3~~ |  6   |  2   |   6   |
    | ~~4~~ |  10  |  20  |  10   |
    | ~~5~~ |      |      |   8   |
    | ~~6~~ |      |      |   4   |
    | ~~7~~ |      |      |   7   |
    | ~~8~~ |      |      |   2   |
    |   9   |      |      |  20   |
    
8. Hacer un algoritmo que permita llenar un vector de 10 posiciones, así:

   |  0   |  0   |  4   |  5   |  8   |  10  |  12  |  15  |  16  |  20  |
   | :--: | :--: | :--: | :--: | :--: | :--: | :--: | :--: | :--: | :--: |
   |  0   |  1   |  2   |  3   |  4   |  5   |  6   |  7   |  8   |  9   |

   ```
   Inicio
   	Entero x, A, B, vector[10]
   	
   	A = 0
   	B = 0
   	
   	Para (x = 0, x < 10, 1) Haga
   		Si (x MOD 2 == 0) Entonces
   			vector[x] = A
   			A += 4
   		Sino
   			vector[x] = B
   			B += 5
   		Fin Si
   	Fin Para
   Fin
   ```

   |   x   |   A    |   B    | vector[10] |
   | :---: | :----: | :----: | :--------: |
   | ~~0~~ | ~~0~~  | ~~0~~  |     0      |
   | ~~1~~ | ~~4~~  | ~~5~~  |     0      |
   | ~~2~~ | ~~8~~  | ~~10~~ |     4      |
   | ~~3~~ | ~~12~~ | ~~15~~ |     5      |
   | ~~4~~ | ~~16~~ |   20   |     8      |
   | ~~5~~ | ~~20~~ |        |     10     |
   | ~~6~~ |   24   |        |     12     |
   | ~~7~~ |        |        |     15     |
   | ~~8~~ |        |        |     16     |
   | ~~9~~ |        |        |     20     |
   |  10   |        |        |            |

   Otra solución:

   ```
   Inicio
   	Entero x, vector[10]
   	Para (x = 0, x <= 4, 1) Haga
   		vector [2 * x] = x * 4
   		vector [2 * x + 1] = x * 5
   	Fin Para
   Fin
   ```

   |   x   | vector[10] |
   | :---: | :--------: |
   | ~~0~~ |     0      |
   | ~~1~~ |     0      |
   | ~~2~~ |     4      |
   | ~~3~~ |     5      |
   | ~~4~~ |     8      |
   |   5   |     10     |
   |       |     12     |
   |       |     15     |
   |       |     16     |
   |       |     20     |

9. Hacer un algoritmo que permita llenar un vector de 8 posiciones y permita crear otro con los factoriales.

    ```
    Inicio
    	Entero x, y, A[8], B[8], factorial
    	
    	Para (x = 0, x < 8, 1) Haga
    		Imprima "Ingrese un número."
    		Lea A[x]
    		
    		factorial = 1
    		
    		Para (y = 1, x <= A[x], 1) Haga
    			factorial = factorial * y
    		Fin Para
    		
    		B[x] = factorial
    	Fin Para
    Fin
    ```

    **Nota:** la prueba de escritorio se realizó solo con un valor ya que hacerla completa seria demasiado extensa.

    |   x   |   y   | factorial | A[8] | B[8] |
    | :---: | :---: | :-------: | :--: | :--: |
    | ~~0~~ | ~~1~~ |   ~~1~~   |  4   |  24  |
    |   1   | ~~2~~ |   ~~1~~   |      |      |
    |       | ~~3~~ |   ~~2~~   |      |      |
    |       | ~~4~~ |   ~~6~~   |      |      |
    |       |   5   |    24     |      |      |
    |       |       |           |      |      |
    |       |       |           |      |      |
    |       |       |           |      |      |
    |       |       |           |      |      |

    

# **Arreglos multidimensionales o matrices**

## Ejercicios propuestos

1. Llenar una matriz de 4x4 por filas.
2. Hacer un algoritmo que permita llenar una matriz de 3x4 por columnas e imprima la suma de los valores ingresados.
3. Hacer un algoritmo que permita llenar por filas una matriz de 3x3, calcule el promedio e imprima:
   * Cantidad de valores iguales al promedio.
   * Cantidad de valores menores al promedio.
   * Cantidad de valores menores al promedio.

4. Hacer un algoritmo que permita llenar una matriz de 4x4 e imprima:
   * Los valores que se encuentran en la diagonal principal.
   * Los valores que se encuentran en la diagonal secundaria.
   * Los valores que se encuentran encima de la diagonal principal.
   * Los valores que se encuentran debajo de la diagonal principal.
   * Los valores que se encuentran encima de la diagonal secundaria.
   * Los valores que se encuentran debajo de la diagonal secundaria.

5. Hacer un algoritmo que permita llenar una matriz de 3x4 por columnas, solo con números enteros e imprima:
   * Suma de cada columna.
   * Suma de cada fila.
6. Hacer un algoritmo que permita llenar una matriz de 4x4 con números enteros y permita crear un vector con los valores que se encuentran debajo de la diagonal secundaria.
7. Hacer un algoritmo que permita llenar una matriz de 5x5 con números enteros y permita crear un vector con el factorial de cada número que se encuentra en la diagonal secundaria.
