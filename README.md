</head>
<body>
  <div class="container">
    <img src="img/Evolución computadoras.JPG" alt="Evolución computadoras">
    <p>Evolución computadoras</p>
  </div>
</body>
</html>


## Objetivos de Aprendizaje
- Comprender los principios básicos de la Ciencia de la Computación.

# Introducción al pensamiento computacional
## Introducción al cómputo

La historia del cómputo se remonta a tiempos antiguos. Los **antiguos griegos** crearon posiblemente la primera computadora, que tenía el propósito de calcular las posiciones del *Sol*, la *Luna* y otros *cuerpos celestes*. Posteriormente, en la **época más moderna**, se desarrollaron tecnologías como el *telar de Jacquard*, un dispositivo mecánico que utilizaba tarjetas perforadas para tejer patrones complejos en la tela.

El avance de la tecnología llevó a la creación del *motor analítico de Charles Babbage*, una máquina diseñada para realizar cálculos. Luego, las máquinas tabuladoras revolucionaron el procesamiento de datos para realizar censos con mayor precisión y velocidad.

En el **siglo XX**, las ideas de *Alan Turing* y *Alonzo Church* sentaron las bases del pensamiento computacional, al demostrar que todos los algoritmos podían ser reducidos a una máquina abstracta con una cinta infinita para manipular símbolos. Esto llevó al desarrollo de la primera computadora electrónica, el *ENIAC*.

*John von Neumann* propuso una arquitectura que permitía almacenar programas en la memoria junto con los datos, lo que se conoció como la *arquitectura de von Neumann*. Con la evolución de los microchips, la computación moderna dio paso a la tecnología que conocemos hoy en día.

## Computer Science (Ciencia de la Computación)

Computer Science (CS) es el estudio de procesos algorítmicos, sistemas computacionales y las computadoras per se. A continuación se darán a conocer las tres principales áreas de estudio.

### Teoria Computacional

La Ciencia de la Computación (Computer Science) es el estudio de procesos algorítmicos, sistemas computacionales y las computadoras en sí. Tiene tres áreas principales de estudio:

Teoría Computacional: Se enfoca en el aprendizaje y análisis de algoritmos, que son secuencias de pasos ordenados que resuelven problemas específicos. Además, abarca conceptos como la complejidad algorítmica, la teoría de grafos, la criptografía, el hardware y las estructuras de datos.

Aplicaciones: Se centra en áreas de la informática como la inteligencia artificial, la robótica, el aprendizaje automático (machine learning), la satisfacibilidad booleana, el procesamiento de imágenes, el procesamiento de lenguaje natural, la realidad aumentada, el análisis de big data y el hacking ético.

Ingeniería Computacional: Se ocupa de la ingeniería del software y el desarrollo de programas y aplicaciones. Incluye el conocimiento y desarrollo de diversos lenguajes de programación, la arquitectura de computadoras, los compiladores y otros aspectos relacionados.

## Circuitos Eléctricos y Conectores Lógicos

Antes de comprender el funcionamiento de una computadora, es importante entender los circuitos eléctricos. Un circuito eléctrico es una interconexión de componentes eléctricos que permite el flujo de corriente eléctrica en una trayectoria cerrada.

Para entender los conceptos lógicos en computación, podemos asociar interruptores a valores lógicos: un interruptor abierto representa el valor lógico 0 (falso) y un interruptor cerrado representa el valor lógico 1 (verdadero).

- El conectivo AND se representa con interruptores en serie. Para que una lámpara se encienda (valor 1), ambos interruptores deben estar cerrados (valor 1).

- El conectivo OR se representa con interruptores en paralelo. Si al menos uno de los interruptores está cerrado (valor 1), la lámpara se enciende (valor 1).

- El conectivo XOR (OR exclusiva) se representa con interruptores en paralelo, pero no ambos interruptores pueden estar cerrados al mismo tiempo. Solo uno de ellos debe estar cerrado para que la lámpara se encienda (valor 1).

- El conectivo NOT (negación) es simplemente el opuesto de un interruptor. Si un interruptor está abierto (valor 0), al agregar una negación, se cierra (valor 1).

Estos conectores lógicos son fundamentales para la construcción de circuitos y la realización de operaciones lógicas en una computadora. La combinación de diferentes conectores lógicos permite realizar tareas más complejas y desarrollar programas y algoritmos eficientes.

**Tablas de verdad**

A | B | AND
--| --| --
1 | 1 |  1
1 | 0 |  0
0 | 0 |  0
0 | 1 |  0

A | B | OR
--| --| --
1 | 1 |  1
1 | 0 |  1
0 | 0 |  0
0 | 1 |  1

A | B | XOR
--| --| --
1 | 1 |  0
1 | 0 |  1
0 | 0 |  0
0 | 1 |  1

A | NOT
--| --
1 |  0
0 |  1

## Half Adder

Un Half Adder (medio sumador) es un circuito lógico utilizado en computación para sumar dos bits individuales (un bit es un 0 o un 1) y producir dos resultados: la suma y el acarreo (carry).

En un sistema binario, la suma de dos bits puede ser 0, 1 o 10 (que se representa como 2 en decimal). El Half Adder resuelve esta operación y proporciona los resultados correctos.

Por ejemplo, consideremos la suma de los números binarios 10011 y 11000. Utilizaremos el Half Adder para realizar la suma bit a bit:

1 | 0   | 0     | 1   | 1
--|-----|-------|-----|---
1 | 1   | 0     | 0   | 0


Comenzamos de derecha a izquierda. Para el primer bit, 1 AND 0 = 0 (sin acarreo), y 1 XOR 0 = 1. Luego, continuamos con el segundo bit, 0 AND 0 = 0 (sin acarreo), y 1 XOR 0 = 1. Procedemos con el tercer bit, 0 AND 0 = 0 (sin acarreo), y 1 XOR 0 = 1. En el cuarto bit, 1 AND 0 = 0 (sin acarreo), y 1 XOR 0 = 1. Finalmente, en el quinto bit, 1 AND 1 = 1 (hay acarreo), y 1 XOR 1 = 0.

Completamos con ceros a la izquierda para tener la misma longitud en ambos números:

  1 | 1   | 0   | 0     | 1   | 1
--|-----|-----|-------|-----|---
0 | 1   | 1   | 0     | 0   | 0

La suma binaria resultante es 101011, que es el equivalente al número decimal 43.

## Sistemas de Numeración
Los sistemas de numeración son formas de representar cantidades mediante símbolos y reglas específicas. Existen varios sistemas, algunos de los cuales son:

### Sistema Unario
Es el más simple, donde se utiliza un único símbolo repetido para representar cada cantidad. Por ejemplo, el número 3 se representaría como "III". Sin embargo, este sistema no es práctico para representar cantidades grandes.

### Números Romanos
Este sistema utiliza siete símbolos diferentes para representar los números, y se basa en reglas aditivas y sustractivas. Por ejemplo, el número 117 se representa como "CXVII", que se lee como cien + diez + cinco + uno + uno.

### Sistemas Posicionales
En estos sistemas, cada dígito tiene un valor que depende de su posición en la cifra y de la base del sistema numérico. Los sistemas decimales y binarios son ejemplos de sistemas posicionales. En el sistema decimal, la base es 10 y los dígitos van desde 0 hasta 9. En el sistema binario, la base es 2 y solo hay dos dígitos: 0 y 1.

### Conversión entre Binario y Decimal
Para convertir un número binario a decimal, se multiplican los dígitos individuales por las potencias de 2 (según su posición) y luego se suman los resultados. Por ejemplo, para el número binario 10101:

1x2^4 + 0x2^3 + 1x2^2 + 0x2^1 + 1x2^0 = 16 + 0 + 4 + 0 + 1 = 21


## Lenguaje de Máquina
Cuando interactuamos con las computadoras, no escribimos directamente en lenguaje binario (1's y 0's) porque sería extremadamente tedioso y propenso a errores. En cambio, utilizamos lenguajes de programación de alto nivel, como Python, Java, C++, entre otros, que nos permiten expresar nuestras instrucciones en un formato más cercano al lenguaje humano y con una mayor abstracción.

Estos lenguajes de alto nivel son más fáciles de entender para nosotros, los humanos, ya que utilizan palabras clave, estructuras de control y funciones que hacen que la escritura y lectura del código sea más intuitiva y legible. Por ejemplo, podemos escribir un programa para sumar dos números en Python de la siguiente manera:

**def suma(a, b):**
    **return a + b**

**resultado = suma(5, 7)**
**print(resultado)**

Este código en Python es mucho más claro y sencillo de entender que su equivalente en lenguaje de máquina, que consistiría en una secuencia de 1's y 0's que indican al procesador cómo realizar la suma.

Una vez que hemos escrito nuestro código en un lenguaje de alto nivel, este debe ser traducido o compilado a lenguaje de máquina, para que la computadora pueda ejecutarlo. El proceso de compilación es realizado por un compilador, que toma el código en lenguaje de alto nivel y lo transforma en instrucciones en lenguaje de máquina que la computadora pueda entender y ejecutar.

De esta manera, gracias a los lenguajes de programación de alto nivel y al proceso de compilación, podemos desarrollar aplicaciones y programas de manera más eficiente y menos propensa a errores, haciendo que la programación sea accesible y poderosa para una amplia gama de personas.
