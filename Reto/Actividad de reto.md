# RETOS

### Se requiere obtener la distancia entre dos puntos en el plano cartesiano, tal y como se muestra en la figura 1. Realice un diagrama de flujo y pseudocódigo que representen el algoritmo para obtener la distancia entre esos puntos.


 ## Analisis

### Variables de entrada
x1, x2, y1, y2

### Variables de salida
D

### Constantes
No hay

### Otras Variables 
No hay

### Ecuaciones

D = x1-x2



Diagrama de flujo

![alt text](<Diagrama de flujo Tarea 1.png>)


pseudocodigo

Inicio
Leer x1,x2,y1,y2
D = x
D = y
Fin

### 2. Una modista, para realizar sus prendas de vestir, encarga las telas al extranjero Para cada pedido, tiene que proporcionar las medidas de la tela en pulgadas, pero ella generalmente las tiene en metros. Realice un algoritmo para ayudar a resolver el problema, determinando cuántas pulgadas debe pedir con base en los metros que requiere. Represéntelo mediante un diagrama de flujo y pseudocódigo (1 pulgada = 0.0254 m).

## Analisis

### Variables de entrada
tela_metros
### Variable de salida
Tela_Pulgadas
### Constantes
Pulgada = 0.0254
### Otras variables
medidas_conv = 
### Ecuaciones
Tela_pulgadas = 
## Diagrama de flujo


## Pseudocodigo
Inicio

Fin


## 3.  Se requiere determinar la hipotenusa de un triángulo rectángulo. ¿Cómo sería el diagrama de flujo y el pseudocódigo que representen el algoritmo para obtenerla? Recuerde que por Pitágoras se tiene que: $C^2 = A^2 + B^2$.

## Analisis

### Varibale de entrada 
A,B,C
### Variable de salida
Hipotenusa_del_triangulo
### Constantes
A = cateto_o ^ 2
b = cateto_a ^ 2
C = Hipotenusa
### Otras variables


### Ecuaciones
C^2 = A^2 + B^2

### Diagrama de flujo



## Pseudocodigo

Inicio

Fin


## 4. Se requiere determinar la edad actual de una persona basándose en su fecha de nacimiento. Además, es necesario establecer si la persona ya ha cumplido años en el año en curso, si aún no lo ha hecho, o si hoy es su cumpleaños, para celebrarlo. La fecha de nacimiento y la fecha actual estarán representadas mediante tres variables: día, mes y año. 


## Analisis

### Varibale de entrada 
dia_nacimiento, mes_nacimiento, año_nacimeinto
### Variable de salida
edad
### Constantes
No hay constantes
### Otras variables
Fecha_actual, edad actual
### Ecuaciones
Año_actual - año_nacimiento

edad - 1
### Diagrama de flujo



## Pseudocodigo
Inicio
Leer dia_nacimiento, mes_nacimiento , año_nacimiento, edad
dia_actual, mes_actual, año_actual
edad = año_actual - año_nacimiento
     si mes_nacimiento < mes_actual
        edad = edad - 1
     si no mes_nacimiento = mes_actual
           imprimir edad
Fin si
     dia_actual = dia_nacimiento
         imprimir Felicitaciones
Fin
## 5. Realice un algoritmo que permita determinar el sueldo semanal de un trabajador con base en las horas trabajadas y el pago por hora, considerando que a partir de la hora número 41 y hasta la 45, cada hora se le paga el doble, de la hora 46 a la 50, el triple, y que trabajar más de 50 horas no está permitido. Represente el algoritmo mediante pseudocódigo.

## Analisis

### Varibale de entrada 
pago_hora
### Variable de salida
Sueldo_semanal
### Constantes
No hay
### Otras variables
No hay
### Ecuaciones

### Diagrama de flujo

### pseudocodigo

Inicio

Fin

## 6. Se requiere un algoritmo para determinar, de N cantidades, cuántas son cero, cuántas son menores a cero, y cuántas son mayores a cero. Realice el pseudocódigo para representarlo, utilizando el ciclo apropiado.

## Analisis

### Varibale de entrada 
cantidad_0, cantidad_menor, cantidad_mayor
### Variable de salida
cantidad_N
### constante
No Hay
### Ecuaciones

### Diagrama de flujo

### pseudocodigo

Inicio
Leer Cantidades_0, Cantidades_mayores, Cantidades_menores


Fin

## 7. Se requiere un algoritmo para determinar cuánto ahorrará en pesos una persona diariamente, y en un año, si ahorra 3¢ el primero de enero, 9¢ el dos de enero, 27¢ el 3 de enero y así sucesivamente todo el año. Represente la solución mediante pseudocódigo.

## Analisis

### Varibale de entrada 

### Variable de salida
Ahorro_anual
### Constantes

### Ecuaciones

### Diagrama de flujo

### pseudocodigo

Inicio

Fin

## 8. Realice el algoritmo para determinar cuánto pagará una persona que adquiere N artículos, los cuales están de promoción. Considere que si su precio es mayor o igual a $200 se le aplica un descuento de 15%, y si su precio es mayor a $100, pero menor a $200, el descuento es de 12%; de lo contrario, solo se le aplica 10%. Se debe saber cuál es el costo y el descuento que tendrá cada uno de los artículos y finalmente cuánto se pagará por todos los artículos obtenidos. Represente la solución mediante pseudocódigo.

## Analisis

### Varibale de entrada 
Articulos_N
### Variable de salida
Precio_final
### Constantes
15%, 12%, 10%
### Ecuaciones

### pseudocodigo.

Inicio
Leer Articulos_N
Desd


Fin


## 9. Realice un algoritmo y represéntelo mediante pseudocódigo para obtener una función exponencial, la cual está dada por:  $𝑒^𝑥 = 1+\frac x {1!} + \frac {x^2}{2!}+ \frac {x^3}{3!}+ …$

## Analisis

### Varibale de entrada 

### Variable de salida

### Constantes

### Ecuaciones

### Diagrama de flujo

### pseudocodigo.

Inicio

Fin

## 10. Realice un algoritmo para obtener el seno de un ángulo y represéntelo mediante pseudocódigo. Utilice la siguiente ecuación: $Sen x = x - \frac{x^3}{3!} + \frac{x^5}{5!} - \frac{x^7}{7!} + ...$

## Analisis

### Varibale de entrada 

### Variable de salida

### Constantes

### Ecuaciones

### Diagrama de flujo

### pseudocodigo.

Inicio

Fin





## solicitar al usuario 2 numero enteros. Imprimir en pantalla los numero pares comprendidos entre ellos

### pseudocodigo

Inicio

Leer numero_1, numero_2    

    si numero_1 > numero_2 
    mayor = numero_1
    menor = numero_2
    si no 
        mayor = numero_2
        menor = numero_1
Fin si
mientras menor < mayor
         si residuo(menor, 2) = 0 //si menor es para
         Escribir menor
         Fin si
         menor = menor +1
    Fin mientras
    Fin

     numero_1 = int(input( "Ingrese el primer numero: "))
    numero_2 = int(input(" Ingrese el segundo numero:"))

if numero_1 > numero_2:
    mayor = numero_1
    menor = numero_2
    
else:
    mayor = numero_2
    menor = numero_1
while menor <= mayor:
    if (menor % 2) == 0:
       print(menor)

Serie de fiboraci
¿ Cuantos numeros de la serie desea imprimir?

Inicio
Leer N
Escribir N0, N1
N0 = 0
N1 = 1

Mientras n >0
 Resultado = No + N1
 Escribir resultado
 n0 = N1
 n1 = resultado
 N = N - 1

Fin mientras
Fin
SI N