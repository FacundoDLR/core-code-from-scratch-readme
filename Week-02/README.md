# Pseudocode - Week 2
## (Monday) 💻

## 1. Logic problem
### Description
The teacher asks his 5 students if they studied mathematics yesterday.

- Alice: "Nobody studied math yesterday".
- Bob: "1 person studied math yesterday".
- Charlie: "2 people studied math yesterday".
- Dan: "3 people studied mathematics yesterday".
- Eva: "4 people studied mathematics yesterday".

The teacher knows that only those who studied would be telling the truth and those who didn't would be lying. Who is telling the truth?

### Expected output
Identify which student is telling the truth

### Solution 😎

The problem is to determine which of the five students is telling the truth. If we assume that one person is telling the truth, then we must analyze each statement to see if it is possible for that person to be the only one telling the truth.

- Alice states that nobody studied math yesterday, but this is not possible because it contradicts the statements of Bob, Charlie, Dan, and Eva.

- Bob says that one person studied math yesterday. If we accept that Bob is telling the truth, then he is the only person who studied math yesterday.

- Charlie states that two people studied math yesterday, but this contradicts Bob's statement. Therefore, if we accept that Bob is telling the truth, then Charlie is lying.

- Dan says that three people studied math yesterday, but this also contradicts Bob's statement. Therefore, if we accept that Bob is telling the truth, then Dan is also lying.

- Eva states that four people studied math yesterday. If we accept that Bob is telling the truth, then we must also accept that Eva is telling the truth, which means that four people studied math yesterday.

Therefore, the only possibility that remains is that Bob and three other people studied math yesterday, and the only person who is telling the truth is **Eva**.

## 2. Which comes first, cereal or milk?

### Description
Create an algorithm to prepare a bowl of cereal with milk. Represent the result in pseudocode and in a flowchart.

### Expected output
Two ways to represent your algorithm previously created

### Solution 😎

1. Get a bowl
2. Add cereal to the bowl
3. Get milk from the refrigerator
4. Pour milk into the bowl of cereal
5. Enjoy!

Here is the flowchart representation of the algorithm:

<p><img src="https://raw.githubusercontent.com/FacundoDLR/core-code-from-scratch-readme/main/assets/CerealMilk.jpg" alt="facundodlr" /></p>

## (Tuesday) 💻

## 1. Print my name & age
### Description
This challenge is similar to the previous guided challenge, but now you will try alone. For this challenge, you will need to create an algorithm in Pseudocode using PSeInt that prints your name and your age in separate lines, remeber that your name should be a string and your age a number

### Solution 😎
```PSeInt
Algoritmo myNameAndAge
	escribir 'Facundo Andres de los Rios'
	escribir '26'
FinAlgoritmo
```

## (Wednesday) 💻

## 1. Algorithm game

### Description
This will be a fun challenge, you will be playing a game base on simple commands, and the idea is for you to help the squirrel to take the pine cone. For this challenge try to pass the first 15 levels. We wish you all the luck and happy gaming.

P.S. If you like, you can try to do all 27 levels, but following level 15 we will need more programming concepts, maybe you can go back to this challenge later 😉

### Solution 😎

<p align="center">
  <img src="https://raw.githubusercontent.com/FacundoDLR/core-code-from-scratch-readme/main/assets/GameComplete27.png" alt="Code Game: Help the Lynx collect pine cones!">
  <img src="https://raw.githubusercontent.com/FacundoDLR/core-code-from-scratch-readme/main/assets/SolutionGame27.png" alt="Code Game: Help the Lynx collect pine cones!">
</p>

## 2. Mod

### Description. Mod in PSeInt Challenge
The challenge for you now is to create a PSeInt program that will receive a number from the user and add the mod operator using the even/odd case ( X % 2 ) where X is the user input

### Solution 😎
```PSeInt
Algoritmo ModuloParImpar
    // Solicitamos un número al usuario
    Escribir "Ingrese un número:"
    Leer num

    // Calculamos el módulo 2 del número ingresado
    resto = num % 2

    // Verificamos si el número es par o impar
    Si resto == 0 Entonces
        Escribir "El número ingresado es par."
    SiNo
        Escribir "El número ingresado es impar."
    FinSi

FinAlgoritmo
```

## 3. Register form

### Description
You are given the task to create a registration form for new users, this form should ask the user for the following information:

First name
Last name
Age
Email
Address
At the end of the program, you should print all the information added from the user in a friendly way

### Solution 😎

```PSeInt
Algoritmo RegistroDeUsuarios
    // Solicitamos al usuario que ingrese su información
    Escribir "Bienvenido al formulario de registro de usuarios"
    Escribir "Por favor ingrese su información personal:"
    Escribir " "
	
    Escribir "Nombre:"
    Leer nombre
	
    Escribir "Apellido:"
    Leer apellido
	
    Escribir "Edad:"
    Leer edad
	
    Escribir "Email:"
    Leer email
	
    Escribir "Dirección:"
    Leer direccion
	
    // Imprimimos la información ingresada por el usuario
    Escribir " "
    Escribir "Gracias por registrarse! Aquí está su información personal:"
    Escribir "Nombre completo: " + nombre + " " + apellido
    Escribir "Edad: " + edad
    Escribir "Email: " + email
    Escribir "Dirección: " + direccion
	
FinAlgoritmo
```

## (Thursday) 💻

## 1. Truth tables
### Description
You are going to learn about three main logical operations used in programming, these operations are called AND, OR, and NOT. Each of the operations uses booleans as operands, and when applying the operations a result is generated, which is also a boolean, this is easier to check using the Truth Tables for each of the operations, now your task is for you to learn, and add the Truth Tables for each of the operations add them to your README and check if the following operations are correct by answering ✅ or ❌ at the end of each operation

Operations:

Remember that AND can be represented by &

Remember that OR can be represented by |

Remember that NOT can be represented by ~

- T & T = T
- T & F = F
- F & T = T
- F & F = F
- T | T = T
- T | F = F
- F | T = T
- F | F = F
- ~T = T
- ~F = T
- (T & F) | (~F) = T
- (T | F ) & (F | F) = T
- ~((T | F ) & (F | F)) & F = T
- ~((T | F ) & (F | F)) & T = F

### Solution 😎

- T & T = T ✅
- T & F = F ✅
- F & T = T ❌
- F & F = F ✅
- T | T = T ✅
- T | F = F ❌
- +F | T = T ✅
- F | F = F ✅
- ~T = T ❌
- ~F = T ✅
- (T & F) | (~F) = T ✅
- (T | F ) & (F | F) = T ❌
- ~((T | F ) & (F | F)) & F = T ❌
- ~((T | F ) & (F | F)) & T = F ❌

## 2. Boolean results
### Description
You have been assigned to verify and explain a code created by one of your colleagues, the idea is that you can describe the value that each variable has within the code as well as what was done for each line. What is expected of you is that you add comments below each line showing the value that the variable would have and a short explanation of how that value is reached.

This is the code:

```PSeInt
Algoritmo boolean
	a <- 5 == 3
	b <- 4 <> 3
	c <- 7 > 7
	d <- 4 < 4
	e <- 100 <= 90
	f <- 40 >= 40
FinAlgoritmo
```

### Solution 😎

```PSeInt
Algoritmo boolean
	a <- 5 == 3 
	// a is assigned the result of the equality comparison between 5 and 3, which is *false*
	b <- 4 <> 3 
	// b is assigned the result of the inequality comparison between 4 and 3, which is true
	c <- 7 > 7 
	// c is assigned the result of the greater-than comparison between 7 and 7, which is false
	d <- 4 < 4 
	// d is assigned the result of the less-than comparison between 4 and 4, which is false
	e <- 100 <= 90 
	// e is assigned the result of the less-than-or-equal-to comparison between 100 and 90, which is false
	f <- 40 >= 40 
	// f is assigned the result of the greater-than-or-equal-to comparison between 40 and 40, which is true
FinAlgoritmo
```

## 3. Identify odd and even numbers
### Description
Remember the last challenge about the Mod operator? well, today your task will be to create a program that will be able to detect based on the user input if the number is odd or even. The process should be the following:

The user enters a number
Your algorithm detects if the number is odd or even (remember to use conditional statements Si...Entonces)
Print ‘Número: x es par’ if the number is even (x is the number the user enters)
Print ‘Número: x es impar’ if the number is odd (x is the number the user enters)

### Solution 😎

```PSeInt
Algoritmo ParImpar
	Escribir "Ingrese un número para verficar"
	Leer num
	Si num%2 == 0
		Escribir "Número: ", num, " es par"
	SiNo                       
		Escribir "Número: ", num, " es impar"
	FinSi
FinAlgoritmo
```
