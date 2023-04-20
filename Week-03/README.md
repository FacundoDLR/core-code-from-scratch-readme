# Pseudocode - Week 03
## (Monday) 💻

## 1. Simple calculator
### Description
For this challenge you will be performing a simple calculator, this calculator can perform the following operations:

1. Sum (+)
2. Subtract (-)
3. Multiplication (*)
4. Division (/)

The calculator must ask the user for two numbers, after asking for the two numbers, you must ask for the operation to be performed, keep in mind that you must show the user the options available (+, -, \*, /). The first thing that must be done is to validate that the operation that the user entered is valid, if it is not a valid option, the user must be shown an error message, for example: `⚠️ La operación no es valida` and terminate the program. If the operation is valid, show the message: `Procesando: <OPERACIÓN A REALIZAR>` For, example: if the user has entered the numbers 10 and 15 as well as the operation \*, the message should read: `Procesando: 10 * 15`. After this message the result of the operation must be displayed, following the previous example, the result of operating 10 \* 15 is 150, so the program should return: `Resultado: 150`. Remember to use conditionals to identify which operations you should execute.

### Solution 😎

```PSeInt
Algoritmo  calcular_operacion

    Escribir "Ingrese el primer número:"
    Leer num1
	
    Escribir "Ingrese el segundo número:"
    Leer num2
	
    Escribir "Ingrese la operación a realizar (+, -, *, /):"
    Leer operacion
	
	signoValido = Falso // Bandera
	
    Si operacion == "+" Entonces
		Escribir "Procesando: " , num1 , " + " , num2
        result = num1 + num2
		signoValido = Verdadero
	FinSi
	
	Si operacion == "-" Entonces
		Escribir "Procesando: " , num1 , " - " , num2
        result = num1 - num2
		signoValido = Verdadero
	FinSi
	
	Si operacion == "*" Entonces
		Escribir "Procesando: " , num1 , " * " , num2
        result = num1 * num2
		signoValido = Verdadero
	FinSi
	
	Si operacion == "/" Entonces
        Si num2 = 0 Entonces
            Escribir "No se puede dividir entre cero"
        Sino
            result = num1 / num2
            Escribir "Procesando: " , num1 , " / " , num2
			signoValido = Verdadero
        FinSi
    FinSi
	
	Si signoValido Entonces
		Escribir  result
	SiNo
		Escribir  "Operacion No valida"
	FinSi
FinProceso
```

## 2. Special number
### Description
You must create the code that follows the following logic, if the given number is 100, take this number as special and show the following message: "This is a special number!", but if the number is less than 1000, multiple of 10 and different from 100, you must show the following message: "This number is almost special". if none of the given conditions are met show the following message: "Just a regular number". Another developer was trying to program the logic, but apparently couldn't, you need to fix the code to work properly

This was the code from the developer

```PSeInt
Algoritmo specialNumber
	Leer n
	Si n == 100 Entonces
		Imprimir 'This is a special number'
	FinSi
	Si n < 1000 Entonces
		Imprimir ''
	SiNo
		Imprimir 'Just a regular number'
	FinSi
	Si n % 10 == 0 Entonces
		Imprimir 'This number is multiple of 10'
	FinSi
FinAlgoritmo
```

### Solution 😎

```PSeInt
Algoritmo numeroEspecial
    Leer n
    Si n == 100 Entonces
        Imprimir '¡Este es un número especial!'
	SiNo
		Si n < 1000 & n % 10 == 0 Entonces
			Imprimir 'Este número es casi especial'
		SiNo
			Imprimir 'Solo un número regular'
		FinSi
    FinSi
FinAlgoritmo
```

## (Tuesday) 💻

## 1. Simple calculator
### Description
For this challenge you will be performing a simple calculator using Switch (Segun), this calculator can perform the following operations:

1. Sum (+)
2. Subtract (-)
3. Multiplication (*)
4. Division (/)

The calculator must ask the user for two numbers, after asking for the two numbers, you must ask for the operation to be performed, keep in mind that you must show the user the options available (+, -, *, /). The first thing that must be done is to validate that the operation that the user entered is valid, if it is not a valid option, the user must be shown an error message, for example: `⚠️ La operación no es valida and terminate the program`. If the operation is valid, show the message: `Procesando: <OPERACIÓN A REALIZAR>` For, example: if the user has entered the numbers 10 and 15 as well as the operation *, the message should read: `Procesando: 10 * 15`. After this message the result of the operation must be displayed, following the previous example, the result of operating 10 * 15 is 150, so the program should return: `Resultado: 150`. Remember to use Switch (Segun) to identify which operations you should execute.

### Solution 😎

```PSeInt
Algoritmo  calcular_operacion
	
    Escribir "Ingrese el primer número:"
    Leer num1
	
    Escribir "Ingrese el segundo número:"
    Leer num2
	
    Escribir "Ingrese la operación a realizar (+, -, *, /):"
    Leer operacion
	
	signoValido = Falso // Bandera
	
	Segun operacion Hacer
		"+":
			Escribir "Procesando: " , num1 , " + " , num2
			result = num1 + num2
			signoValido = Verdadero
		"-":
			Escribir "Procesando: " , num1 , " - " , num2
			result = num1 - num2
			signoValido = Verdadero
		"*":
			Escribir "Procesando: " , num1 , " * " , num2
			result = num1 * num2
			signoValido = Verdadero
		"/":
			Si num2 = 0 Entonces
				Escribir "No se puede dividir entre cero"
			Sino
				result = num1 / num2
				Escribir "Procesando: " , num1 , " / " , num2
				signoValido = Verdadero
			FinSi
	Fin Segun
	
	Si signoValido Entonces
		Escribir  result
	SiNo
		Escribir  "Operacion No valida"
	FinSi
FinProceso
```

## 2. Multi Option Program
### Description
For this challenge you will create a program with multiple options using Switch (Segun), the options available are the following:

1. Sum two numbers
2. Print the day of the week given the day number
3. Print the length of a given text

This program must have a start menu where the user must select one of the previously described options. When the user selects each of the options, the program will perform the following:

1. Sum. The user enters two numbers and the result of the sum of both is printed
2. Print day of the week. The user enters a day of the week using numbers and the name of the day must be printed. For example, if the number 1 is entered, the program prints the text Lunes.
3. Calculate text length. The user enters a text and the length of the text should be printed. I was able to use the Pseint Longitud function to get the length.

When the user enters an incorrect option, a message should be printed saying that the option is not available.

### Solution 😎

```PSeInt
Algoritmo programaOpciones
	
    Escribir "Bienvenido al programa de opciones"
    Escribir "Por favor, seleccione una opción:"
    Escribir "1. Sumar dos números"
    Escribir "2. Imprimir el día de la semana dado el número del día"
    Escribir "3. Imprimir la longitud de un texto"
    Leer opcion
	
    Segun opcion Hacer
        1:
            Escribir "Por favor, ingrese dos números a sumar:"
            Leer num1, num2
            Escribir "El resultado de la suma es:", num1 + num2
        2:
            Escribir "Por favor, ingrese un número del 1 al 7 para imprimir el día de la semana:"
            Leer dia
            Segun dia Hacer
                1: Escribir "Lunes"
                2: Escribir "Martes"
                3: Escribir "Miércoles"
                4: Escribir "Jueves"
                5: Escribir "Viernes"
                6: Escribir "Sábado"
                7: Escribir "Domingo"
                De Otro Modo: Escribir "Opción no disponible"
            FinSegun
        3:
            Escribir "Por favor, ingrese un texto:"
            Leer texto
            Escribir "La longitud del texto es:", Longitud(texto)
        De Otro Modo:
            Escribir "Opción no disponible"
    FinSegun
	
FinAlgoritmo
```

## (Wednesday) 💻

## 1. Multiplication Tables
### Description
For this challenge you will create a program to calculate the multiplication tables for a given number using While (Mientras). The user must enter a number and then the multiplication table for the number must be printed.

### Solution 😎

```PSeInt
Algoritmo MultiplicationTable
	Imprimir '======= Multiplication Tables ======='
	// Declaring variables
	Definir num, i, result Como Entero
	
	// Getting user input
	Escribir "Ingrese un numero para imprimir su tabla de multiplicar: "
	Leer num
	
	// Initializing loop counter
	i = 1
	
	// Printing multiplication table
	Mientras (i <= 10) Hacer
		result = num * i
		Escribir num, " x ", i, " = ", result
		i = i + 1
	Fin Mientras
	
FinAlgoritmo
```

## 2. Simple calculator with Do While
### Description
For this challenge we are going to use the simple calculator that we made in the challenge 02 but now adding the functionality to perform a calculation again without finishing the program. The program should ask us if we want to use another operation and if the user answers yes then we can perform a new operation. To solve this challenge remember to use Do while (Repetir Hasta Que).

### Solution 😎

```PSeInt
Algoritmo calculadora
	
	Leer num1, num2, result
	Leer operacion, respuesta
	
	Repetir
		Escribir "Ingrese el primer número:"
		Leer num1
		
		Escribir "Ingrese el segundo número:"
		Leer num2
		
		Escribir "Ingrese la operación a realizar (+, -, *, /):"
		Leer operacion
		
		Segun operacion Hacer
			"+":
				Escribir "Procesando: " , num1 , " + " , num2
				result = num1 + num2
				signoValido = Verdadero
			"-":
				Escribir "Procesando: " , num1 , " - " , num2
				result = num1 - num2
				signoValido = Verdadero
			"*":
				Escribir "Procesando: " , num1 , " * " , num2
				result = num1 * num2
				signoValido = Verdadero
			"/":
				Si num2 = 0 Entonces
					Escribir "No se puede dividir entre cero"
				Sino
					result = num1 / num2
					Escribir "Procesando: " , num1 , " / " , num2
					signoValido = Verdadero
				FinSi
		Fin Segun
		
		Si signoValido Entonces
			Escribir  result
		SiNo
			Escribir  "Operacion No valida"
		FinSi
			
		Escribir "¿Desea realizar otra operación? (S/N)"
		Leer respuesta
	Mientras Que  respuesta = "S" | respuesta = "s"

FinAlgoritmo
```

## (Thursday) 💻

## 1. Multiplication Tables with For
### Description
For this challenge you will create a program to calculate the multiplication tables for a given number using the For(Para) loop. The user must enter a number and then the multiplication table for the number must be printed.

### Solution 😎

```PSeInt
Algoritmo tabla_multiplicar
	
	Escribir "Ingrese un número:"
	Leer numero
	
	Para i = 1 Hasta 10 Con Paso 1 Hacer
		resultado <- numero * i
		Escribir numero, " x ", i, " = ", resultado
	FinPara
	
FinAlgoritmo
```
## 2. Ascending and Descending Numbers
### Description
For this challenge we are going to print numbers in ascending or descending order. The user must enter a number, then he must enter if he wants to print the numbers in ascending or descending order. If the user chooses ascending, the numbers will be printed from the number 0 to the number entered, otherwise the numbers will be printed descending from the number entered to the number 0.To solve this challenge remember to use the For(Para) loop.

### Solution 😎

```PSeInt
Algoritmo UpaAndDwnNum
	
	Escribir "======= Ascending and Descending Numbers ======="
	Escribir "¡Deseas realizar operacion de Ascenso o Descenso? (A/D)"
	Leer  respuesta
	Escribir "Ingresa un numero"
	Leer num
	Si respuesta == "A" | respuesta == "a" Entonces
		Para i = 0 Hasta num Con Paso 1 Hacer
			Escribir i
		Fin Para
	SiNo
		Para i=num Hasta 0 Con Paso -1 Hacer
			Escribir i
		Fin Para
	Fin Si
FinAlgoritmo
```

## 3. Greetings
## Description
For this challenge, you need to create a program that prints a greeting based on an hour entered. The program should do the following:

- Print Buenos dias! if the hour is from 0 to 12
- Print Buenas tardes! if the hour is from 13 to 18
- Print Buenas noches! if the hour is from 19 to 23
- Ask the user if he wants to perform another greeting. If the answer is Si, the program must start again.
- At the end of the program, print out the number of times the program has greeted.

### Solution 😎
```PSeInt
Algoritmo Cheers
	
	Escribir "===== Cheers ====="
	contador = 0
	
	Repetir
		Escribir "Ingrese la hora actual (0 - 23):"
		Leer hora
		
		Si hora >= 0 & hora <= 12 Entonces
			saludo = "Buenos dias!"
		SiNo
			Si hora >= 13 & hora <= 18 Entonces
				saludo = "Buenas tardes!"
			SiNo
				Si hora >= 19 & hora <= 23 Entonces
					saludo = "Buenas noches!"
				SiNo
					Escribir "Hora invalida. Ingrese un numero entre 0 y 23."
				FinSi
			FinSi
		FinSi
		
		contador = contador +1
		Escribir saludo
		
		Escribir "¿Quiere realizar otro saludo? (S/N)"
		Leer respuesta
		
	Mientras Que respuesta = "S" | respuesta = "s"
	Escribir "Saludos realizados: ",contador

FinAlgoritmo
```
