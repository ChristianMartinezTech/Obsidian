
***Profesor***: Ivan Dario Maldonado - Ing. Electrónico

***Programación semanal***:
- Semana 1: **Test Tema 1
	- **Test Tema 2
- Semana 2: **Test Tema 3
- Semana 3: **Test Tema 4
	- **Actividad: Laboratorio. Implementación del método de eliminación guassiana por el método del pivotaje parcial escalado
		- Fecha Limite: Lunes, 11 de septiembre de 2023, 23:59
- Semana 4: **Test Tema 5
- Semana 5: **Test Tema 6
	- **Actividad: Creación y resolución de un problema de programación lineal
		- Lunes, 25 de septiembre de 2023, 23:59
.

## TEMA 1: MÉTODOS DE PRUEBA

En el estudio de las matemáticas, existen dos temas fundamentales que se deben tener presentes en todo momento;

1. Cuando un argumento que se plantea es correcto.
2. Cuáles son los métodos o técnicas que podemos usar para comprobarlo.

Para ello, usamos la lógica de primer orden para analizar lenguajes de primer orden (Lenguajes formales con predicados, conectores y afirmaciones con las que se construyen los teoremas).

Los métodos de demostración son importantes, por que nos sirven para demostrar teoremas matemáticos, pero también para la *demostración de algoritmos*, la *verificación de la seguridad de un sistema operativo* o para *comprobar que un determinado programa funciona de forma correcta*.
.
#### 1.2 Variables y cuantificadores

- Predicado: p(x) expresión que puede conectarse con otras expresiones para formar una proposición.

- Proposición: afirmación de la cual se puede decir sin ambigüedad que es verdadera V o falsa F. Suelen representarse mediante p, q, o r. Se denomina proposición **atómica** a aquellas que no incluyen conectores (las mas simples), y proposiciones **moleculares o compuestas** a aquellas que están compuestas por dos o mas proposiciones atómicas unidas mediante conectores.

Para crear una proposición, debemos definir la variable el valor de x, para lo cual, podemos asignar una valor a la variable. Cuando la variable no tiene restricciones se llama **variable libre**, si restringimos el valor de la variable se llama **variable cuantificada**.

Ex: Jupiter es mas grande que Marte
		- Jupiter: Variable cuantificada
		- Marte: Variable Libre
		- es mas grande que : Predicado
		- Todo completo es una proposición

- Cuantificador: expresión que afirma que una condición se cumple para un cierto número de individuos. Los dos cuantificadores más estudiados son el cuantificador **universal** y el **existencial**.
	- Cuantificador Universal (∀): afirma que una condición se cumple para **todos** los individuos de los que se está hablando. Usando la sintaxis ∀x p(x) se lee “para todo valor de x, la propiedad p es cierta”.
	- Cuantificador Universal (∃): afirma que la condición se cumple para **al menos uno** de los valores de la variable. Usando la sintaxis ∃x : p(x) se lee “existe algún valor de x tal que p es cierta”.

- Conectores Lógicos:
	- Negación “no” (¬)
	- Conjunción “y” (∧)
	- Disyunción “o ” (∨)
	- Condicional “si . . .” entonces “. . .” (−→
	- Bicondicional “sí y solo sí” (←→)
.

#### 1.3 Tablas de verdad

Una tabla de verdad es una matriz que contiene los valores de verdad de una proposición en función de los valores de verdad de las proposiciones atómicas que la componen.

![[Pasted image 20230822215640.png]]

Una proposición compuesta que siempre es cierta para cualquiera de los valores de sus proposiciones atómicas recibe el nombre de tautología. La negación de una tautología, es decir, Álgebra y Matemática discreta Tema 1. Ideas clave 9 una proposición compuesta que siempre es falsa, recibe el nombre de contradicción. Si unas veces es falsa y otras cierta, recibe el nombre de contingencia.

![[tablas de verdad-ad4270f9-ae00-4dbd-85ca-880071ee5066.webp]]
.
#### 1.4 Métodos de prueba

Los métodos de prueba permiten demostrar que un teorema es verdadero mediante una secuencia de sentencias que llamamos **demostración**.

Para ello se utilizan las reglas de inferencia, que enlazan cada uno de los pasos que forman la demostración. Las reglas de inferencia constituyen cada uno de los pasos lógicos que nos llevan de p a q para demostrar una sentencia condicional (p → q). A la primera parte de la sentencia condicional se la llama premisa o hipótesis y a la segunda, conclusión o consecuencia.

- Técnicas de demostración directa e indirecta
- Demostración por reducción al absurdo
.

## TEMA 2: INDUCCIÓN Y RECURSIÓN

Ambos son dos conceptos similares que se emplean para demostrar proposiciones sobre conjuntos de números naturales y con los que seguramente te has topado en tu formación matemática, e incluso tal vez antes.

- El principio de inducción es una propiedad que de los números naturales y nos permite demostrar que todos los naturales satisfacen una determinada proposición, es decir, es un método de demostración.
- El principio de recursión, es un resultado que permite dar una definición para todos los números naturales, basándonos en una proposición que cumple su antecesor, es decir, es una definición recursiva.

#### 2.2 Inducción Matemática

La inducción matemática es un método de demostración que se utiliza cuando se trata de establecer la veracidad de una lista infinita de proposiciones

Se trata de un método de demostración de 3 pasos:
		1. Base = Hacer al menos 1 Ejemplo.
		2. Hipótesis = Suponer que se va a cumplir para un cierto valor.
		3. Tesis = Agregarle el siguiente elemento, simplificarlo, y confirmar que el resultado tenga la misma estructura de la proposición original.

.

#### 2.3 Recursión

.

.