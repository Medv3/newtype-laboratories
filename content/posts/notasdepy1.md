---
title: "Título del Ensayo"
date: 2026-11-05T05:16:24-05:00
draft: false
dropcap: true
toc: false
series: []
tags: []
---
# Notas de Python

## Intro a la programación

### ¿Qué es una computadora?

Una _computadora_ es una máquina programable diseñada para procesar información mediante la ejecución de instrucciones formalmente definidas para llevar a cabo operaciones sobre datos, tales como operaciones aritméticas, lógicas, de comparación, transformación, almacenamiento y transferencia.

Las computadoras solo pueden ejecutar operaciones extremadamente simples por sí mismas, como sumar o dividir, pero pueden hacerlo muy rápido y repetir estas acciones casi infinitamente.

Para que una computadora ejecute tareas complejas, es necesario darle instrucciones detalladas para descomponer estas tareas en secuencias de operaciones simples.

### ¿Qué es la programación?

_Programar_ es dar instrucciones formalmente definidas a un computador para que ejecute una tarea. Un conjunto ordenado o serie de estas instrucciones destinadas a la ejecución de una o un conjunto de tareas es un _programa_.

Estas instrucciones deben ser traducidas a un _lenguaje_ que la computadora pueda entender. Esto es, a un _lenguaje de programacion_.

### ¿Qué es el lenguaje?

«Un lenguaje es un medio (y una herramienta) para expresar y registrar pensamientos.» Esta es una definicion contenciosa, pero suficientemente funcional para nuestros propósitos. Un lenguaje, por lo general consta de los siguientes elementos:

- Un alfabeto: un conjunto de símbolos que se pueden combinar para formar palabras de un determinado lenguaje.
- Un léxico: un diccionario o conjunto de palabras que el lenguaje ofrece a sus usuarios. Se trata de la lista de combinaciones aceptables y comprensibles de los símbolos que componen el alfabeto.
- Una sintaxis: un conjunto de reglas (formales o informales) utilizadas para precisar si una determinada cadena de palabras forma una oración válida.
- Una semántica: un conjunto de reglas que determinan si una frase tiene sentido o no en un determinado lenguaje.

Solemos asociar los lenguajes con el habla y la escritura, pero no todos los lenguajes requieren estas prácticas o acciones. Por ejemplo el lenguaje corporal no requiere a ninguna de las dos.

Hay muchos lenguajes a nuestro alrededor, varios de ellos los utilizamos en nuestra vida cotidiana. Los lenguajes generados de manera espontánea entre grupos de hablantes con el propósito de comunicarse se conocen como lenguajes naturales, pero también existe una amplia variedad de lenguajes construidos, lenguas artificiales diseñadas a partir del estudio de lenguajes naturales.

Por lo general se reservan estos rótulos (lenguaje natural y lenguaje artificial o construido) para los idiomas, las lenguas utilizadas por los grupos humanos para comunicarse entre sí. Los lenguajes destinados específicamente al uso en las matemáticas o la informática, no a la comunicación directa de pensamientos entre seres humanos, se distiguen y se categorizan por aparte, como lenguajes formales. Este es el caso de los conjuntos de símbolos y fórmulas bien formadas de la lógica, el conjunto de los símbolos de la matemática, casos más específicos como la numeración de Gödel y también el conjunto de todos los lenguajes de programación.

### Lenguajes de programación

Un lenguaje de programación es un lenguaje formal destinado a proporcionar a una programadora la capacidad de escribir programas, secuencias de instrucciones en forma de algoritmos para controlar el comportamiento de un computador o de un sistema informático.

### Lenguajes de programación bajo y alto nivel

El lenguaje de programación más básico que comprende un computador es el _lenguaje máquina_, un sistema de códigos interpretable directamente por los circuitos microprogramables de un computador. El lenguaje máquina sólo puede ser representado por unos y ceros, los caracteres del sistema binario de numberación. El computador entiende e interpreta estor patrones de bits (dígitos binarios) como representación, cada uno, de un estado electrónico. Esto resulta en instrucciones para ejecutar una operación simple como tomar un número, dividirlo por otro y guardar el resultado, por ejemplo.

El conjunto de operaciones básicas que un procesador puede entender y ejecutar directamente mediante lenguaje máquina se conoce como _Instruction Set_ o _conjunto de instrucciones_. El conjunto puede variar según la arquitectura del procesador, diseñado al igual que el lenguaje de máquina, por los seres humanos.

El alfabeto del lenguaje máquina son unos y ceros. Este lenguaje está muy lejos de un lenguaje natural. Esto motivó, por facilidad y eficiencia, a la búsqueda de puentes entre estos lenguajes.

Se comenzaron a crear distintos lenguajes de programación que representaban las instrucciones que se daban a los computadores con el lenguaje máquina, o conjuntos de ellas, con símbolos y reglas de combinación orientados a complejizar las instrucciones que se le dan a las máquinas a la vez que se hacían más cercanos a los lenguajes naturales, sobre todo al inglés, en alfabeto, léxico, sintáxis y semántica.

Se trata de lenguajes formales más simples que un lenguaje natural pero suficientemente potentes para comandar al computador a realizar tareas complejas de manera un poco más fácil de comprender para un ser humano familiarizado con el lenguaje natural en el que se basa el lenguaje de programación.

Estos lenguajes de proramación se denominan lenguajes de programación de alto nivel, en contraposición a los lenguajes de bajo nivel como el lenguaje de máquina y los lenguajes muy cercanos a este que buscaron simplificar un poco el léxico y la sintáxis manteniéndose siempre muy cerca de las instrucciones directas al hardware, como el _lenguaje emsamblador_ (_assembly_).

Un programa escrito en un lenguaje de programación de alto nivel se denomina _código fuente_ (_source code_), a diferencia del código máquina o de un lenguaje de bajo nivel que es una forma de escribir las instrucciones del lenguaje máquina usando mnemotecnia y abreviaturas. El archivo que contiene el código fuente se denomina _archivo fuente_ (_source_).

### Compilación e interpretación

«La programación informática es el acto de componer los elementos del lenguaje de programación seleccionado en el orden que provocará el efecto deseado». Esta composición debe ser correcta alfabética, léxica, sintáctica y semánticamente. Esto significa que un programa debe estar escrito en un alfabeto reconocible, cuyos caracteres deben combinarse de acuerdo con reglas gramaticales claras y estas combinaciones a su vez deben formar combinaciones mayores siguiendo las reglas sintácticas definidas. Finalmente, el programa debe tener sentido.

Una vez tenemos un programa escrito correctamente en un lenguaje de programación, debemos convertirlo en lenguaje de máquina para que el computador pueda entender y ejecutar nuestras instrucciones. ¿Cómo? La misma computadora puede traducirlo de dos maneras:

- Compilación: El código fuente se traduce una vez obteniendo un archivo que contiene el código máquina. El programa que realiza esta traducción se llama _compilador_ o _traductor_. La compilación nos deja con un archivo ejecutable que podemos distribuir de inmediato. El problema es que cada vez que modifiquemos el código fuente, debemos volver a compilar y obtener un nuevo archivo (por ejemplo .exe o .bin).

- Interpretación: El código se traduce línea por línea dentro de un intérprete cada que se ejecuta. El programa que realiza esta traducción se llama _intérprete_, pues interpreta el código cada vez que lo va a ejecutar, línea por línea. Acá uno puede ir actualizando el código fuente sin tener que compilar cada versión, pero el usuario final necesita contar con el intérprete para poder ejecutar el programa. Aún cuando se congela un programa de Python, por ejemplo, lo que se hace es empaquetar el código fuente junto con el intérprete para que se ejecute e interprete el código cada vez que se ejecute el achivo ejecutable.

Por lo general, los lenguajes de programación se diseñan ya pensando en cómose van a implementar los programas, compilándolos o interpretándolos. Casi todos los lenguajes, a muy grandes rasgos, se pueden categorizar como lenguajes compilados e interpretados, si bien existen casos híbridos como C# y en general en todos los casos las fronteras son borrosas: un intérprete de Python, por ejemplo, compila el texto del código fuente para traducirlo a bytecode y ahí sí interpreta.

Un intérprete lee el texto plano del código fuente, verifica que sea correcto en los cuatro aspectos señalados anteriormente para los lenguajes, y comienzas a leer y ejecutar cada línea, verificando que funcione en un bucle de leer, ejecutar e imprimir un resultado si aplica (un _Read, Execute, Print Loop o REPL_).

¿Y qué método de traducción a instrucciones para el hardware es mejor?

|             | Compilación                                                                                                                                                                                                                                                                                                                                                                                               | Interpretación                                                                                                                                                                                                                                                                                                                        |
| ----------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Ventajas    | - La ejecución de un programa compilado suele ser más rápida, solo el programador necesita el compilador porque el usuario final puede ejecutar el programa sin él.<br><br>- El código compilado se almacena usando lenguaje de máquina dando cierta seguridad y privacidad mayor al código                                                                                                               | - El código se puede ejecutar tan pronto como se termine de escribir o actualizar sin ninguna fase o proceso adicional de parte del programador.<br><br>- Este código fuente se mantiene almacenado en el lenguaje de programación en el que se escribió, haciéndolo portable para otras máquinas que tengna otro lenguaje de máquina |
| Desventajas | - La compilación puede tomar mucho tiempo, y hay que ir compilando cada que se modifique el código para ver cómo se ejecuta la nueva versión.<br><br>- Cada plataforma de hardware puede tener instrucciones distintas, hablar un lenguaje de máquina distinto, por lo que la compilación debe hacerse para cada plataforma en particular o de forma que intente abarcar varias, complejizando el proceso | - La interpretación suele ser más lenta a la hora de ejecutar el programa.<br><br>- El usuario final necesita tener un intérprete                                                                                                                                                                                                     |

Python es un lenguaje interpretado. Para programar en Python, se necesita, entonces, el intérprete de Python. Sin el intérprete no podremos ejecutar nuestro código. Por suerte, salvo casos muy específicos (como Mathlab o SAS), el intérprete, como el uso del lenguaje de programación, los compiladores en los lenguajes compilados, etc. son gratuitos y de libre distribución.

Como dato final, por razones históricas, los lenguajes diseñados para ser interpretados suelen denominarse _lenguajes de scripting_ (como bash) y sus programas son llamados _scripts_. Sin embargo este término se mantiene más para lenguajes especializados, con esturcturas más limitadas y sintaxis más simple. Python, por su parte, como Java o C++ es un lenguaje de programación multipropósito y multiparadigma.

## Intro a Python

### ¿ Qué es Python?

«Python es un lenguaje de programación de alto nivel, interpretado, orientado a objetos y de uso generalizado con semántica dinámica, que se utilzia para la programación de propósito general.»

El nombre del lenguaje de programación Python, contrario a lo que suelen creer muchas personas, no proviene de la serpiente constrictora, sino de _Monty Python's Flying Circus_, una serie británica de comedia transmitida por la BBC entre 1969 y 1974. El creador de Python era fan del programa y nombró su lenguaje de programación en honor al show.

A diferencia de la mayoría de los grandes lenguajes de programación, desarrollados y publicados por grandes compañías, Python fue creado por una sola persona, Guido van Rossum (1956 - ), un programador neerlandés. Con el tiempo, sin embargo, Pythons e extendió por todo el mundo y las versiones modernas son el producto del trabajo continuo de miles y miles de programadores, tsters, usuarios y entusiastas.

Guido van Rossum desarrolló Python en 1989 como un proyecto para mantenerse ocupado en Navidad. En 1991 publicó la versión 0.9.0, la primera versión pública del lenguaje. El primer gran lanzamiento, Python 1.0, apareció en enero de 1994.

En 1999, Guido van Rossum definió los objetivos que tenía para Python:

- que fuera fácil e intuitivo pero tan poderoso como sus principales competidores
- que fuera de código abierto para que cualquier persona pueda contribuir a su desarrollo
- que el código fuese tan comprensible como el inglés
- que fuera adecuado para tareas cotidianas, permitiendo tiempos de desarrollo cortos

Estos objetivos se han cumplido, y hoy Python es probablemente el lenguaje de programación más popular del mundo. Con casi 40 años de desarrollo, Python es ya un lenguaje maduro, bien desarrollado y confiable.

### ¿Por qué Python?

La popularidad de Python se explica por varias razones, principalmente porque:

- es fácil de aprender comparado con otros lenguajes de programación, haciéndolo una buena opción para comenzar a programar.
- es fácil de enseñar, lo que permite que un profesor se enfoque más en las técnicas de programación que en la estructura misma del lenguaje.
- es fácil de utilizar para escribir software, lo cual hace que también sea rápido escribir programas.
- es fácil de entender, lo que lo hace más fácil y rápido de leer y evaluar.
- es fácil de obtener, instalar y ejecutar por ser gratuito, abierto y multiplataforma.

### ¿Por qué no Python?

A pesar de la popularidad de Python, existen todavía áreas en las que se usa poco:

- Programación de bajo nivel: Python no es el lenguaje de programación más efectivo y no siempre es útil si se quiere implementar un driver o un motor gráfico.
- Desarrollo de aplicaciones móviles: Aunque ya existen proyectos orientados a usar Python en esta área, sigue siendo dominada por otros lenguajes de programación.

### Lenguajes rivales de Python

Python tiene dos competidores directos y comparables en propiedades y predisposiciones:

- Perl: lenguaje de scripting escrito originalmente por Larry Wall.
- Ruby: lenguaje de scripting escrito originalmente por Yukihiro Matsumoto.

Perl es más tradicional y consevador que Python, con rasgos similares a lenguajes más antiguos derivados de C. Ruby es más innovador.

### ¿Dónde se utiliza Python?

Python se utiliza en casi todo en la actualidad: servicios de internet como motores de búsqueda, almacenamiento en la nube, redes sociales, herramientas de desarrollo, aplicaciones d euso diario, procesamiento de datos, testeo de proyectos de IT, desarrollo de modelos de IA y un largo, largo etcétera.

### Python 2 v. Python 3

Existen, hoy en día, dos grandes versiones de Python: Python 2 y Python 3.

Python 2 es una versión anterior cuyo desarrollo se dejó atrás para pasar a enfocarse en la versión 3. Sin embargo, aún salen actualizaciones para Python 2 aunque ya vienen orientadas a arreglar errores y parchar posibles vulnerabilidades, sin modificar el lenguaje de forma significativa. Python 2, sin embargo, sigue muy vivo.

Python 3 es la versión más nueva (y la actual) del lenguaje. Sigue evolucionando y se sigue actualizando y desarrollando.

Python 2 y Python 3 no son compatibles. Los comandos de Python 2 no se ejecutarán en un entorno de Python 3 y viceversa. Hay grandes partes del código iguales, pero hay muchas incompatibilidades que casi siempre obligan a que el código sea reescrito para cada versión, lo que suele resultar más barato y seguro que intentar migrar la aplicación de Python 2 a un nuevo entorno.

Python 3 es prácticamente un lenguaje completamente nuevo, si bien muy similar a Python 2, en vez de solo una versión actualizada o mejorada. Sin embargo, la gran cantidad de aplicaciones escritas en Python 2 impiden que este se descarte o se deje completamente atrás.

Hoy en día, sin embargo, la más usada es la versión actual: Python 3. Las versiones de Python 3 sí son compatibles entre sí (3.4, 3.6, 3.7, etc.)

### Implementaciones de Python

CPython, Jython, pypy, MicroPython.
