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

### Solution 😎



### Solution 😎



## (Thursday) 💻

### Solution 😎



### Solution 😎
