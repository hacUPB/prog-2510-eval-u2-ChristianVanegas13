# Ejercicio 1

![alt text](image.png)


- Unas variables binarias pueden representar dos posibles estados cada una. Cuando tienes varias variables binarias, el número de posibles estados aumenta exponencialmente.

Para 
𝑁 variables binarias, el número total de posibles estados se da por: 2𝑁


## Ejemplo:

- 1 variable binaria: 2^1 = 2 estados

- 2 variables binarias: 2^2 = 4 estados

- 3 variables binarias: 2^3 = 8 estados

- Así que para cualquier número 𝑁 de variables binarias, solo necesitas elevar 2 a la potencia de 𝑁.


# Bitacora

### 1. Escribe un párrafo explicando, en tus propias palabras, cómo se representan los datos en una computadora. Por ejemplo, ¿cómo se ingresan números, letras, imágenes a una computadora?

- Las computadoras usan el sistema binario (0 y 1) para representar datos. Cuando ingresamos información como números, letras o imágenes, la computadora convierte todo en una secuencia de estos bits. Los números se transforman en binario, las letras en códigos como ASCII o Unicode y las imágenes en píxeles con valores binarios. Así, la computadora puede entender, procesar y almacenar la información eficientemente.


### 2. Luego de realizar el ejercicio 1, escribe tus conclusiones acerca de la pregunta planteada en la Figura 2. ¿Cuántos estados diferentes pueden ser representados por N variables binarias?

- Si tienes 𝑁 variables binarias, puedes representar 2 𝑁 diferentes estados. Esto significa que cada variable binaria puede ser 0 o 1, y al combinar 𝑁
  variables, el total de combinaciones posibles es 2 𝑁. Entonces, para cualquier número de variables binarias, puedes encontrar el número de estados diferentes usando esta fórmula.

### 3. ¿Cuáles son las unidades de almacenamiento de datos que se utilizan en computación? Crea una tabla donde muestres estas unidades con sus prefijos. En este caso me refiero a KiloByte, MegaByte, etc


| Unidad        | Abreviatura | Tamaño en Bytes                                            |
|---------------|-------------|----------------------------------------------------------- |
| Byte          | B           | 1 Byte                                                     |
| KiloByte      | KB          | 1,024 Bytes                                                |
| MegaByte      | MB          | 1,024 KiloBytes (1,048,576 Bytes)                          |
| GigaByte      | GB          | 1,024 MegaBytes (1,073,741,824 Bytes)                      |
| TeraByte      | TB          | 1,024 GigaBytes (1,099,511,627,776 Bytes)                  |
| PetaByte      | PB          | 1,024 TeraBytes (1,125,899,906,842,624 Bytes)              |
| ExaByte       | EB          | 1,024 PetaBytes (1,152,921,504,606,846,976 Bytes)          |
| ZettaByte     | ZB          | 1,024 ExaBytes (1,180,591,620,717,411,303,424 Bytes)       |
| YottaByte     | YB          | 1,024 ZettaBytes (1,208,925,819,614,629,174,706,176 Bytes) |

- Fuente: https://edu.gcfglobal.org/es/cultura-tecnologica/medidas-de-almacenamiento-de-informacion/1/


### 4. Incluye un pequeño resumen, de un par de renglones, donde menciones la importancia del trabajo de George Bool en este tópico.

- George Boole fue un matemático y lógico que creó el álgebra booleana, una forma de lógica basada en valores binarios (0 y 1). Su trabajo es fundamental para las computadoras modernas, ya que permite representar y procesar datos utilizando el sistema binario. Gracias a Boole, podemos almacenar y manejar información de manera eficiente en dispositivos electrónicos.



# Ejercicio 2.

## como pasar de numero binario a decimales paso a paso.

#### paso 1.

- Crear una tabla donde vas a elevar el # 2 de atras así alante.

### Ejemplo

#### Convertir $10100101_2$


|2^8  |2^7 |2^6|2^5|2^4|2^2|2^1|2^0|
------------------------------------
| 128 | 64 | 32| 16| 8 | 4 | 2 | 1 |
------------------------------------
- Ahora al poner el numero binario en la tabla, vas ponerlo como te lo dieron pero empezando de atras hacia alante en la tabla.

### Ejemplo

|2^8  |2^7 |2^6|2^5|2^4|2^2|2^1|2^0|
------------------------------------
| 128 |  64| 32| 16|  8| 4 | 2 | 1 |
------------------------------------
|    1|   0|  1|  0|  0| 1 | 0 | 1 |


- Ahora los numeros que esten encima del digito 1 en la tabla 3, se sumaran y los que tengan el digito 0 encima se ignoraran.

### Ejemplo

El 1 tiene digito 1 por debajo?
si, entonces se tomara ese numero para sumar.

El 2 tiene el digito 1 por debajo?
No, pues en ese caso no se suma el 2.

Así susesivamente con cada numero que haya tocado.

### La respuesta seria entonces:

1+ 4+ 32+ 128 = $165_{10}$

## Ejercicios 2.

- 1. $1010101010_2$
- 2. $11111_2$
- 3. $10000000_2$
- 4. $100100100_2$
- 5. $111000_2$

- 1. $1010101010_2$

|2^10|2^9|2^8  |2^7 |2^6|2^5|2^4|2^2|2^1|2^0|
---------------------------------------------
| 512|256| 128 |  64| 32| 16|  8| 4 | 2 | 1 |
---------------------------------------------
|   0|  1|    0|   1|  0|  1|  0| 1 | 0 | 1 |

- 1+4+16+64+256 = $341{10}$
 
- 2. $11111_2$

|2^5|2^4|2^2|2^1|2^0|
---------------------
| 16|  8| 4 | 2 | 1 |
---------------------
|  1|  1|  1|  1|  1|

- 1+2+4+8+16 = $31{10}$

- 3. $10000000_2$

|2^8  |2^7 |2^6|2^5|2^4|2^2|2^1|2^0|
------------------------------------
| 128 |  64| 32| 16|  8| 4 | 2 | 1 |
------------------------------------
|    0|   0|  0|  0|  0| 0 | 0 | 1 |

- La respuesta es $1{10}$

- 4. $100100100_2$

|2^9|2^8  |2^7 |2^6|2^5|2^4|2^2|2^1|2^0|
----------------------------------------
|256| 128 |  64| 32| 16|  8| 4 | 2 | 1 |
----------------------------------------
|  0|    0|   1|  0|  0|  1| 0 | 0 | 1 |

- 1+8+64 = $73{10}$

- 5. $111000_2$

|2^6|2^5|2^4|2^2|2^1|2^0|
-------------------------
| 32| 16|  8| 4 | 2 | 1 |
-------------------------
|  0|  0| 0 | 1 | 1 | 1 |


- 1+2+4 = $7{10}$

## Convertir ahora de Decimal a Binario.

### Hay varias formas para hacerlo. Solo enseñare dos.

## Ejemplo 1.

- Convertir $156{10}$

- Cogemos la misma tabla

|2^9|2^8  |2^7 |2^6|2^5|2^4|2^2|2^1|2^0|
---------------------------------------------
|256| 128 |  64| 32| 16|  8| 4 | 2 | 1 |
---------------------------------------------
|  0|    1|   0|  0|  1|  1| 1 | 0 | 0 |

#### Ahora lo que vas a hacer es localizar el puesto mas alto que el 156 en la tabla, en este caso el 256, ya que el 128 esta mas bajo que el 156.

- Como el 256 es mayor pues colocamos un 0 debajo.

- Pues bien ya que es 0 lo ignoramos.

- Ahora bien el 128 es menor o igual que el 156?

- Si entonces lo que vas a hacer es restarle 128 al 156 y debajo del 128 ponemos un 1.

- 156 - 128 = 28

- Pues bien ahora 64 es <= que 28?

- No entonces ponemos un 0 debajo del 64.

- Seguimos, 32 es <= que 28?

- No, entonces se pone un 0 debajo de 32 en la tabla.

- Seguimos, 16 es <= 28?

- Si, entonces se pone un 1 debajo del 16 en la tabla y le restamos 16 al 28.

- 28 - 16 = 12

- Ahora el 8 es <= 12?

- si, entonces se pone un 1 debajo del 8.

- 12 - 8 = 4.

- Entonces el 4 <= 4?

- si, entonces ponemos un 1 debajo del 4 y le volvemos a restar 4 al 4.

- 4 - 4 = 0

- Entonces el 2 <= al 0?

- No, entonces ponemos otro 0 debjao del 2.

- El 0 <= 1

- No, pues se pone un 0 debajo del 1.

- Ignorando siempre el numero de la tabla mayor al numero decimal, entonces seria el restuado de esta manera.

- En este caso empezando desde el numero debajo del 128 hasta el

- $156{10}$ =  $10011100_2$

## Ejemplo 2.

- Convirtiendo el mismo decimal $156{10}$ a binario.

- Usamos la misma tabla otra vez.

|2^9|2^8  |2^7 |2^6|2^5|2^4|2^2|2^1|2^0|
----------------------------------------
|256| 128 |  64| 32| 16|  8| 4 | 2 | 1 |
----------------------------------------
|  0|    1|   0|  0|  1|  1| 1 | 0 | 0 |


- localizamos de nuevo el numero mas alto en la tabla que el decimal dado, en este caso es el decimal es 156. Entonces cogemos el 256 en la tabla.

- Debajo del 56 volvemos a poner el digito 0 debajo del 256 en la tabla porque 256 es > 156.

- Bueno el numero que sigue en la tabla es el 128.

- Ahora el 128 <= 156?

- si pues se pone un 1 debajo del 128.

-  Nada diferente al anterior verdad?

- No, pues ahora cambia todo, ahora lo que tienes que hacer es sumarle al 128 el numero que sigue en la tabla, que en este caso es 64.

- 128 + 64 = 192

- 192 es <= 156?

- No, pues en este caso se pone un 0 debajo del 64 y no lo sumamos mas.

- El siguiente numero en la tabla es 32, entonces lo sumamos.

- 128 + 32 = 160

- 160 es <= 156?

- No, entonces se pone un 0 debajo del 32 y no se suma mas.

- Sigue el numero 16 entonces lo sumamos.

- 128 + 16 = 144

- 144 es <= 156?

- Si, entonces ponemos un 1 debajo del 16 en la tabla y lo sumamos.

- 128 + 16 + 8 = 152

- Es 152 <= 156?

- Si, entonces se pone un 1 debajo del 8 en la tabla y lo sumamos.

- 128+16+8+4=156

- Es 156 <= 156?

- Si es igual, entonces se pone un 1 debajo del 4 en la tabla y se suma.

- 128+16+8+4+2=158

- Es 158 <= 156?

- No, entonces no se suma y se debe poner un 0 debajo del 2 en la tabla.

- Sigue el numero 2 en la tabla lo sumamos.

- 128+16+8+4+1=157

- Es 157 <=156?

- No, entonces no se suma y se pone un 0 debajo del 1 en la tabla.

- En este caso se vuelve a coger el numero debajo del 128 hasta el 1 ignirando el numero mayor a 156 en la tabla.

- $156{10}$ = $10011100_2$

## Ejercicios de convertir de numero decimal a numero Binario.


- 1. $127_{10}$
- 2. $246_{10}$
- 3. $1025_{10}$
- 4. $354_{10}$

- 1. $127_{10}$

|2^8  |2^7 |2^6|2^5|2^4|2^2|2^1|2^0|
----------------------------------------
| 128 |  64| 32| 16|  8| 4 | 2 | 1 |
----------------------------------------
|    0|   1|  1|  1|  1| 1 | 1 | 1 |


64+32=96
64+32+16=112
64+32+16+8=120
64+32+16+8+4=124
64+32+16+8+4+2=126
64+32+16+8+4+2+1=127

- $127_{10}$ = $1111111_2$

- 2. $246_{10}$

|2^9|2^8  |2^7 |2^6|2^5|2^4|2^2|2^1|2^0|
----------------------------------------
|256| 128 |  64| 32| 16|  8| 4 | 2 | 1 |
----------------------------------------
|  0|    1|   1|  1|  1|  0| 1 | 1 | 0 |

246-128=118
118-64=54
54-32=22
22-16=6
6-4=2
2-2=0

- $246_{10}$ = $11110110_2$

- 3. $1025_{10}$

| 2^12| 2^11|2^10|2^9|2^8  |2^7 |2^6|2^5|2^4|2^2|2^1|2^0|
---------------------------------------------------------
|2.048|1.024| 512|256| 128 |  64| 32| 16|  8| 4 | 2 | 1 |
---------------------------------------------------------
|    0|    1|   0|  0|    0|   0|  0| 0 | 0 |  0|  0|  1| 

1.025-1.024=1 

- $1025_{10}$ = $10000000001_2$


- 4. $354_{10}$

|2^10|2^9|2^8  |2^7 |2^6|2^5|2^4|2^2|2^1|2^0|
---------------------------------------------
| 512|256| 128 |  64| 32| 16|  8| 4 | 2 | 1 |
---------------------------------------------
|   0|  1|    0|   1|  1|  0|  0| 0 | 1 | 0 |

256+128= 384
256+64= 320
256+64+32=352
256+64+32+16=368
256+64+32+8=360
256+64+32+4=356
256+64+32+2=354
256+64+32+2+1=355

- $354_{10}$ = $101100010_2$


# 1.Introducción

En una computadora digital, toda la información del mundo real (texto, números, imágenes, sonidos) se convierte en secuencias de bits (0 y 1). Estos bits permiten a la máquina procesar y almacenar datos de manera eficiente y confiable, lo que nos permite modelar datos complejos a partir de una representación binaria simple.😊

# 2. Pregunta para reflexionar.

Las computadoras usan representación binaria (0 y 1) porque es más fácil y confiable. Los componentes electrónicos pueden distinguir entre dos estados, lo que reduce errores. También, las operaciones con 0 y 1 son rápidas y eficientes. Es un estándar universal que hace que diferentes dispositivos se comuniquen bien entre sí. Además, diseñar y fabricar componentes electrónicos es más simple y económico usando solo dos estados.

En resumen, el sistema binario es sencillo, eficiente y práctico para las computadoras.

# 3. Investiga los diferentes tipos de datos que se utilizan en varios lenguajes de programación (por ejemplo, C, Java, Python). Ten en cuenta cómo cada lenguaje define los números enteros, los decimales (o flotantes), las letras del alfabeto, las cadenas de texto, valores booleanos, entre otros. Investiga qué nombres se asignan y qué abreviaciones se utilizan en cada lenguaje.

## C

### Números enteros:

- int: enteros

- short int: enteros cortos

- long int: enteros largos

- unsigned int: enteros sin signo

- Decimales (flotantes):

- float: números de punto flotante

- double: números de punto flotante de doble precisión

- long double: números de punto flotante de precisión extendida

- Letras del alfabeto:

- char: un solo carácter

- Cadenas de texto:

- char[]: arreglo de caracteres

- Valores booleanos:

- bool (en stdbool.h): valores booleanos (true o false)

## Java

### Números enteros:

- byte: enteros de 8 bits

- short: enteros de 16 bits

- int: enteros de 32 bits

- long: enteros de 64 bits

- Decimales (flotantes):

- float: números de punto flotante de 32 bits

- double: números de punto flotante de 64 bits

- Letras del alfabeto:

- char: un solo carácter (16 bits, compatible con Unicode)

- Cadenas de texto:

- String: cadena de texto

- Valores booleanos:

- boolean: valores booleanos (true o false)

## Python

### Números enteros:

- int: enteros (de tamaño arbitrario en Python 3)

- Decimales (flotantes):

- float: números de punto flotante (equivalente a double en otros lenguajes)

- Letras del alfabeto:

- str: un solo carácter se representa como una cadena de longitud 1

#### Cadenas de texto:

- str: cadena de texto

#### Valores booleanos:

- bool: valores booleanos (True o False)

https://www.hostinger.com/mx/tutoriales/java-vs-python?form=MG0AV3

https://j2logo.com/python/tutorial/tipos-de-datos-basicos-de-python/?form=MG0AV3


# 4. Con la información recolectada, organiza los datos en una tabla que incluya:

- **Nombre de la variable**
- **Abreviación (si existe)**
- **Características principales** (rango, tipo de valor, etc.)



#   | Nombre de la Variable | Abreviación (si existe) | Características Principales              | Lenguaje  |
    |-----------------------|-------------------------|------------------------------------------|-----------|
##  | `int`                 | `int`                   | Enteros, tamaño depende del sistema      | C         |
##  | `short int`           | `short`                 | Enteros cortos, generalmente 16 bits     | C         |
##  | `long int`            | `long`                  | Enteros largos, generalmente 32 o 64 bits| C         |
##  | `unsigned int`        | `unsigned`              | Enteros sin signo                        | C         |
##  | `float`               | `float`                 | Flotantes, precisión simple              | C         |
##  | `double`              | `double`                | Flotantes, precisión doble               | C         |
##  | `long double`         | `long double`           | Flotantes, precisión extendida           | C         |
##  | `char`                | `char`                  | Carácter único                           | C         |
##  | `char[]`              | `char[]`                | Cadena de caracteres                     | C         |
##  | `bool`                | `bool`                  | Booleanos (`true` o `false`)             | C         |
##  | `byte`                | `byte`                  | Enteros de 8 bits                        | Java      |
##  | `short`               | `short`                 | Enteros de 16 bits                       | Java      |
##  | `int`                 | `int`                   | Enteros de 32 bits                       | Java      |
##  | `long`                | `long`                  | Enteros de 64 bits                       | Java      |
##  | `float`               | `float`                 | Flotantes de 32 bits                     | Java      |
##  | `double`              | `double`                | Flotantes de 64 bits                     | Java      |
##  | `char`                | `char`                  | Carácter único (16 bits, Unicode)        | Java      |
##  | `String`              | `String`                | Cadena de texto                          | Java      |
##  | `boolean`             | `boolean`               | Booleanos (`true` o `false`)             | Java      |
##  | `int`                 | `int`                   | Enteros (tamaño arbitrario)              | Python    |
##  | `float`               | `float`                 | Flotantes (equivalente a `double`)       | Python    |
##  | `str`                 | `str`                   | Carácter único o cadena de texto         | Python    |
##  | `bool`                | `bool`                  | Booleanos (`True` o `False`)             | Python    |



# 5. Imagina que necesitas almacenar la siguiente información en un programa:

- Un identificador numérico (número entero)
- Una temperatura (valor de punto flotante)
- Un valor lógico (dato booleano)
- Un texto con 10 caracteres.

#### Se almacena la información cada 10 segundos durante 24 horas. Calcula cuánto espacio total se requiere en memoria para almacenar estos datos. Describe el procedimiento y muestra el resultado final.

### 1. Identificador numérico (entero): Asumimos que se usa un entero de 4 bytes (32 bits).

### 2. Temperatura (valor de punto flotante): Asumimos que se usa un float de 4 bytes (32 bits).

### 3. Valor lógico (booleano): Asumimos que se usa un booleano de 1 byte (8 bits).

### 4. Texto con 10 caracteres: Asumimos que cada carácter usa 1 byte (8 bits), por lo tanto, 10 caracteres = 10 bytes.

## Sumemos el tamaño de cada dato:

- Identificador numérico: 4 bytes

- Temperatura: 4 bytes

- Valor lógico: 1 byte

- Texto (10 caracteres): 10 bytes

- Total por cada registro: 4 +4 + 1+ 10 = 19 bytes.

- Ahora, calculamos la cantidad de registros que se almacenan en 24 horas: Hay 86,400 segundos en un día (24 horas * 60 minutos * 60 segundos).

- Se almacena la información cada 10 segundos.

- Total de registros en 24 horas: 86,400 ÷ 10 = 8,640 registros.

- Finalmente, calculamos el espacio total requerido:

- Espacio total requerido = Número de registros * Tamaño de cada registro Espacio total requerido =  8,640  registros ∗19   bytes = 164,160   bytes.

- Convertimos a Kilobytes (KB) para una mejor visualización: 164,160  bytes ÷ 1,024 = 160.31 KB

- Por lo tanto, se requieren aproximadamente 160.31 KB de memoria para almacenar estos datos durante 24 horas.


# 6. Finalmente, explica con tus propias palabras el resultado de esta actividad y qué aprendiste acerca de la representación de datos en las computadoras.

- En resumen, aprendí cómo se representa y almacena la información en las computadoras usando el sistema binario y cómo calcular el espacio de memoria necesario para almacenar datos. Además, aprendí a convertir números binarios a decimales y viceversa, y cómo implementar estas conversiones en diferentes lenguajes de programación. Todo esto es fundamental para comprender el funcionamiento de las computadoras y la programación.