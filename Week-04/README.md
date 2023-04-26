# Pseudocode - Week 04
## (Monday) 💻

## 1. Average sales and commission
### Description

Make a program that asks how many sales the seller had, Once the number of sales is entered, ask for the value of each sale until all are entered, then return as a result the average value of sales, and the commission that the seller will take, If the seller had more than 5 sales, his commission will be 15% of the total value of the sales, if he sold 5 or less, his commission will be only 10%.

### Solution 😎

```PSeInt
Algoritmo ComisionVendedor
	
    Escribir "Ingrese el número de ventas realizadas:"
    Leer numVentas
	
    totalVentas <- 0
	
    Para i <- 1 Hasta numVentas Con Paso 1 Hacer
        Escribir "Ingrese el valor de la venta número ", i, ":"
        Leer valorVenta
        totalVentas <- totalVentas + valorVenta
    FinPara
	
    promedioVentas <- totalVentas / numVentas
	
    Si numVentas <= 5 Entonces
        comision <- totalVentas * 0.1
    SiNo
        comision <- totalVentas * 0.15
    FinSi
	
    Escribir "El promedio de ventas es: $", promedioVentas
    Escribir "La comisión del vendedor es: $", comision
	
FinAlgoritmo
```

## 2. Even or odd
### Description

Request a number from 1 to 50, if the number is not between those values, report the error and request it again until you get a valid number, then it shows on the screen all the numbers from 1 to that number, if the number is even it only shows the even numbers, if it is odd it only shows the odd ones.

### Solution 😎

```PSeInt
Algoritmo NumerosParesImpares

    Repetir
        Escribir "Ingrese un número del 1 al 50:"
        Leer num
        Si num < 1 | num > 50 Entonces
            Escribir "Error: número inválido"
        FinSi
    Hasta Que num >= 1 & num <= 50
	
    Si num % 2 = 0 Entonces
        Escribir "Los números pares del 1 al ", num, " son:"
        Para i <- 1 Hasta num Con Paso 1 Hacer
            Si i % 2 = 0 Entonces
                Escribir i
            FinSi
        FinPara
    SiNo
        Escribir "Los números impares del 1 al ", num, " son:"
        Para i <- 1 Hasta num Con Paso 1 Hacer
            Si i % 2 <> 0 Entonces
                Escribir i
            FinSi
        FinPara
    FinSi
FinAlgoritmo
```

## (Tuesday) 💻

## 1. Full name
### Description

Make a program that takes a first name and a last name, then returns a string with both values ​​with the first letter uppercase and the rest lowercase.

### Solution 😎

```PSeInt
Algoritmo NombresMayuscula
    
    Escribir "Ingrese su primer nombre:"
    Leer nombre
    Escribir "Ingrese su apellido:"
    Leer apellido
	
    nombre = Mayusculas(Subcadena(nombre, 0, 0)) + Minusculas(Subcadena(nombre, 1, Longitud(nombre)-1))
    apellido = Mayusculas(Subcadena(apellido, 0, 0)) + Minusculas(Subcadena(apellido, 1, Longitud(apellido)-1))
	
    Escribir "Su nombre completo en mayúscula es:", nombre, " ", apellido
FinAlgoritmo
```

## 2. Throw dice
### Description

make a program that simulates the roll of 2 dice 10 times, and display for each roll the values ​​of the two dice separated by a space, in case the 2 dice throw the same value in addition to the result, add a string to the ending that says "the dice are the same".

### Solution 😎

```PSeInt
Algoritmo TirarDados
	
    Para i <- 1 Hasta 10 Con Paso 1 Hacer
        dado1 <- Aleatorio(1, 6)
        dado2 <- Aleatorio(1, 6)
		
        Si dado1 = dado2 Entonces
            Escribir dado1, " ", dado2, " Los dados son iguales."
        Sino
            Escribir dado1, " ", dado2
        FinSi
    FinPara
	
FinAlgoritmo
```

## (Wednesday) 💻

## 1. Distance to zero
### Description

Make a program that asks for 5 values ​​and also allows us to know which one is furthest from zero, once obtained it returns that number (the numbers can be negative), showing only the integer part of the number.

### Solution 😎

### Description
### Solution 😎

### Description
### Solution 😎

## (Thursday) 💻

### Description
### Solution 😎

### Description
### Solution 😎

### Description
### Solution 😎