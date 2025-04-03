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
Pulgada = 0.0254m
### Otras variables
medidas_conv = Tela_Pulgada / 0.0254
### Ecuaciones
Tela_pulgadas = Tela_metros * Medidas_Conv
## Diagrama de flujo


## Pseudocodigo

Inicio
```
    Leer Tela_Metros

    Escribir "Ingrese los metros de tela necesarios: "
   
    Si 1 pulgada = 0.0254 metros
      Entonces Medidas_Conv = Tela_Pulgada / 0.0254
    
    Si Tela_Pulgada => 0
      Entonces Tela_Pulgadas = Tela_metros * Medidas_Conv

    Fin si
     Ecribir "Se necesitan " + pulgadas + " Tela_Pulgada."

Fin
```

## 3.  Se requiere determinar la hipotenusa de un triángulo rectángulo. ¿Cómo sería el diagrama de flujo y el pseudocódigo que representen el algoritmo para obtenerla? Recuerde que por Pitágoras se tiene que: $C^2 = A^2 + B^2$.

## Analisis

### Varibale de entrada 
A,B,C
### Variable de salida
Hipotenusa_del_triangulo
### Constantes
A = cateto_O ^ 2  
b = cateto_A ^ 2  
C = Hipotenusa
### Otras variables


### Ecuaciones
C^2 = RC(A^2 + B^2)

### Diagrama de flujo



## Pseudocodigo
```
Inicio

    Leer A,B,C
    
    A = Cateto_A
    B = Cateto_O
    C = Hipotenusa

    Si Cateto_o^2
    Entonces
        Escribir "Ingrese el valor de A: "
   
    Si Cateto_A^2
    Entonces 
      Escribir "Ingrese el valor de b: "
   
    Fin si
       c = RC(a^2 + b^2)
    
    Entonces 
    Escribir "La hipotenusa es: ", c

Fin
```

## 4. Se requiere determinar la edad actual de una persona basándose en su fecha de nacimiento. Además, es necesario establecer si la persona ya ha cumplido años en el año en curso, si aún no lo ha hecho, o si hoy es su cumpleaños, para celebrarlo. La fecha de nacimiento y la fecha actual estarán representadas mediante tres variables: día, mes y año. 


## Analisis

### Varibale de entrada 
dia_nacimiento, mes_nacimiento, año_nacimeinto, edad, anio_actual, mes_actual, dia_actual 
### Variable de salida
edad
### Constantes
No hay constantes
### Otras variables
No hay
### Ecuaciones
Anio_actual - anio_nacimiento

edad - 1
### Diagrama de flujo



## Pseudocodigo

```
Inicio
   
    LEER dia_nacimiento, mes_nacimiento , anio_nacimiento, edad
    dia_actual, mes_actual, anio_actual
    
    Escribir "Ingrese el día de nacimiento: ", dia_nacimiento
    
    Escribir "Ingrese el mes de nacimiento: ", mes_nacimiento
   
    Escribir "Ingrese el año de nacimiento: ", anio_nacimiento
    
    Escribir "Ingrese el día actual: ", dia_actual

    Escribir "Ingrese el mes actual: ", mes_actual
    
    Escribir "Ingrese el año actual: ", anio_actual
    
     edad = anio_actual - anio_nacimiento

    Si mes_actual < mes_nacimiento 
       Entonces
           edad = edad - 1
             cumplido = Aun no
    Si No 
        Si mes_actual >= mes_nacimiento Y dia_actual < dia_nacimiento 
          Entonces
           edad = edad - 1
             cumplido = Aun no
    Si No
        cumplido = Ya Cumpliste
    Fin Si
      Escribir "La edad es: ", edad
    
    Si mes_actual => mes_nacimiento Y dia_actual => dia_nacimiento 
      Entonces
        Escribir "!Happy Birthday!"

    Si No 
        Si cumplido 
          Entonces
             Escribir "Ya ha cumplido años este año."
    Si No
        Escribir "Todavía no ha cumplido años este año."
    Fin Si
Fin    
``` 

## 5. Realice un algoritmo que permita determinar el sueldo semanal de un trabajador con base en las horas trabajadas y el pago por hora, considerando que a partir de la hora número 41 y hasta la 45, cada hora se le paga el doble, de la hora 46 a la 50, el triple, y que trabajar más de 50 horas no está permitido. Represente el algoritmo mediante pseudocódigo.

## Analisis

### Varibale de entrada 
pago_hora, Horas_trabajada, Extra_Doble, Extra_Triple
### Variable de salida
Sueldo_semanal
### Constantes
No hay
### Otras variables
No hay
### Ecuaciones

### Diagrama de flujo

### pseudocodigo

```
Inicio

    
    Leer Pago_hora, Horas_Trabajadas
    
    Escribir "Ingrese las horas trabajadas en la semana: ", 
    Horas_trabajadas

    Escribir "Ingrese el pago por hora: ", pago_hora

    Si Horas_Trabajada > 50 
       Entonces
         Escribir "No está permitido trabajar más de 50 horas."
    Si No
      Si Horas_Trabajadas <= 40 Entonces
            Sueldo_Semanal = Horas_Trabajadas * pago_hora
        Si No
            Sueldo_Semanal = 40 * pago_hora
            
    Si Horas_Trabajadas > 40 Y Horas_Trabajadas <= 45 
      Entonces
         Extra_Doble = Horas_Trabajadas - 40
         
         Sueldo_Semanal = Sueldo_Semanal + (Extra_Doble * pago_hora * 2)
      
      Si No Si Horas_Trabajada > 45 
      Entonces
         Extra_Doble = 45 - 40
            
         Sueldo_Semanal = Sueldo_Semanal + (ExtraDoble * pago_Hora * 2)
                
       
        Extra_Triple = Horas_Trabajadas - 45
        Sueldo_Semanal = Sueldo_Semanal + (Extra_Triple * pago_Hora * 3)
      
      Fin Si
        Escribir "El sueldo semanal es: $", Sueldo_Semanal
    
    Fin Si

FIN
```

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

```
Inicio

    // Declaración de variables
    ahorroDiario = 0.03 // Inicialmente ahorra 3¢ el primer día
    ahorroAnual = 0 // Total ahorrado en un año
    diasEnUnAño = 365

    // Ciclo para calcular el ahorro diario y anual
    PARA i = 1 HASTA diasEnUnAño HACER
        // Calcular el ahorro diario
        ahorroDiario = 0.03 * (3^(i-1))
        
        // Sumar al ahorro anual
        ahorroAnual = ahorroAnual + ahorroDiario
        
        // Mostrar el ahorro diario
        ESCRIBIR "El ahorro del día " + i + " es: $" + ahorroDiario
    FIN PARA

    // Mostrar el ahorro anual
    ESCRIBIR "El ahorro total en un año es: $" + ahorroAnual

FIN
```

## 7. Se requiere un algoritmo para determinar cuánto ahorrará en pesos una persona diariamente, y en un año, si ahorra 3¢ el primero de enero, 9¢ el dos de enero, 27¢ el 3 de enero y así sucesivamente todo el año. Represente la solución mediante pseudocódigo.

## Analisis

### Varibale de entrada 
Ahorro_Diario, Dias_Anual
### Variable de salida
Ahorro_anual
### Constantes
Ahorro_Diaro = 0.03

Dias_Anual = 365

### Ecuaciones

### Diagrama de flujo

### pseudocodigo
```
INICIO

    Leer Ahorro_Diario, Dias_Anual

    Dias_Anual =365

    Para i = 1 
    
      Hasta Dias_Anual 
        Hacer
        Ahorro_Diario = 0.03 * (3^(i-1))
        Hacer
          Ahorro_Anual = Ahorro_Anual + Ahorro_Diario
            Entonces
              Escribir "El ahorro del día " + i + " es: $" + ahorroDiario
    Fin Para

    Escribir "El ahorro total en un año es: $",  Ahorro_Anual

Fin
```


## 8. Realice el algoritmo para determinar cuánto pagará una persona que adquiere N artículos, los cuales están de promoción. Considere que si su precio es mayor o igual a $200 se le aplica un descuento de 15%, y si su precio es mayor a $100, pero menor a $200, el descuento es de 12%; de lo contrario, solo se le aplica 10%. Se debe saber cuál es el costo y el descuento que tendrá cada uno de los artículos y finalmente cuánto se pagará por todos los artículos obtenidos. Represente la solución mediante pseudocódigo.

## Analisis

### Varibale de entrada 
Precio_Articulo
### Variable de salida
Precio_Total
### Constantes
15%, 12%, 10%

### Otras VARIABLES
Descuento_Total, Descuento_Articulo

### Ecuaciones


### pseudocodigo.

```
INICIO


    Leer Precio_Articulo
     
    N = Numero_Articulos
    N = 0
    
    Escribir "Ingrese el número de artículos: ", N

    Para I = 1 Hasta N
       Hacer
        Escribir "Ingrese el Precio_Artículo " + I + ": ", Precio_Articulo

    Si Precio_Articulo >=200    Entonces
         Descuento_Articulo = Precio_Articulo * 0.15
    Si No 
       Si Precio_Articulo > 100 Y Precio-Articulo < 200 ENTONCES
            Descuento_Articulo = Precio_Articulo * 0.12

        De lo contario
            Descuento_Articulo = Precio_Articulo * 0.10
        Fin Si
        Precio_Descuento = Precio_Articulo - Descuento_Articulo

        Precio_Total = Precio_Total + Descuento_Articulo
        Descuento_Total = Descuento_Total + Descuento_Articulo

        Escribir "El costo del artículo " + I + " con descuento es: $" , Descuento_Total
        ESCRIBIR "El descuento aplicado es: $" + descuento
    Fin Para

    Escribir "El total a pagar por todos los artículos es: $", Precio_Total
    Escribir "El descuento total aplicado es: $", Descuento_Total

Fin
```

## 9. Realice un algoritmo y represéntelo mediante pseudocódigo para obtener una función exponencial, la cual está dada por:  $𝑒^𝑥 = 1+\frac x {1!} + \frac {x^2}{2!}+ \frac {x^3}{3!}+ …$

## Analisis

### Varibale de entrada 
x, n
### Variable de salida
Resultado
### Constantes

### Ecuaciones

### Diagrama de flujo

### pseudocodigo.

INICIO

    // Declaración de variables
    x = 0 // Valor de x para calcular e^x
    n = 0 // Número de términos en la serie
    maxIteraciones = 100 // Máximo número de iteraciones
    tolerancia = 0.000001 // Tolerancia para detener la serie
    resultado = 1 // Resultado inicial (1 + 0)
    factorial = 1 // Factorial inicial (0!)
    terminoActual = 1 // Término actual de la serie

    // Entrada de datos
    ESCRIBIR "Ingrese el valor de x: ",  x

    // Establecer el número de iteraciones
    n = 1

    // Ciclo para calcular la serie de Taylor
    MIENTRAS n <= maxIteraciones Y abs(terminoActual) > tolerancia HACER
        // Calcular el término actual de la serie
        factorial = factorial * n
        terminoActual = (x**n) / factorial
        
        // Sumar el término actual al resultado
        resultado = resultado + terminoActual
        
        // Incrementar el número de iteraciones
        n = n + 1
    FIN MIENTRAS

    // Mostrar el resultado
    ESCRIBIR "El valor de e^x es: ", resultado

FIN


Fin

## 10. Realice un algoritmo para obtener el seno de un ángulo y represéntelo mediante pseudocódigo. Utilice la siguiente ecuación: $Sen x = x - \frac{x^3}{3!} + \frac{x^5}{5!} - \frac{x^7}{7!} + ...$

## Analisis

### Varibale de entrada 

### Variable de salida

### Constantes

### Ecuaciones

### Diagrama de flujo

### pseudocodigo.

IINICIO

    // Declaración de variables
    x = 0 // Valor del ángulo en radianes
    n = 0 // Número de términos en la serie
    maxIteraciones = 100 // Máximo número de iteraciones
    tolerancia = 0.000001 // Tolerancia para detener la serie
    resultado = 0 // Resultado inicial
    signo = 1 // Signo del término actual (alterna entre 1 y -1)
    factorial = 1 // Factorial inicial (0!)
    terminoActual = 0 // Término actual de la serie

    // Entrada de datos
    ESCRIBIR "Ingrese el valor del ángulo en radianes: "
    LEER x

    // Establecer el número de iteraciones
    n = 1

    // Ciclo para calcular la serie de Taylor
    MIENTRAS n <= maxIteraciones * 2 Y abs(terminoActual) > tolerancia HACER
        // Calcular el término actual de la serie
        factorial = factorial * (n) * (n + 1)
        terminoActual = signo * (x**(n)) / factorial
        
        // Sumar el término actual al resultado
        resultado = resultado + terminoActual
        
        // Alternar el signo para el siguiente término
        signo = -signo
        
        // Incrementar el número de iteraciones
        n = n + 2
    FIN MIENTRAS

    // Mostrar el resultado
    ESCRIBIR "El seno del ángulo es: ", resultado

FIN


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
