# Pseudocode & Javascript - Week 05
## Week challenges (Monday) 💻

## 1. Time Converter
### Description
Create a function called timeConverter that receives a positive number of seconds and returns a string based on the number. "Days: 1, Hours: 5, Minutes: 40 and seconds: 5"

4000 --> "days: 0, hours: 1, minutes: 6, and seconds: 4"

40000 --> "days: 0, hours: 11, minutes: 6, and seconds: 4"

150000 --> "days: 1, hours: 17, minutes: 40, and seconds: 0"
### Expected output
```PSeInt
Algoritmo exampleTimeConverter
	Imprimir timeConverter(4000)
FinAlgoritmo
```
### Solution 😎



## 2. Compare distances
### Description
Create a function called compareDistances that asks for 5 numbers, these can be positive or negative, add the positives with positives and negatives with negatives, the function should return true if there is more distance to 0 with positives or false if the distance is greater with negatives .

4, 12 , 100, 8, -60 --> true

40, 120 , 10, -80, -91 --> false
### Expected output
```PSeInt
Algoritmo exampleCompareDistances
	Imprimir CompareDistances()
FinAlgoritmo
```
### Solution 😎
```PSeInt
Funcion result <- compareDistances()
	sumPositives <- 0
	sumNegatives <- 0
	Para count = 1 Hasta 5 Con Paso 1 Hacer
		leer num
		si num > 0 Entonces
			sumPositives = sumPositives + num;
		SiNo
			sumNegatives = sumNegatives + num;
		FinSi
	FinPara
	result = sumPositives > Abs(sumNegatives)
Fin Funcion

Algoritmo compareDistancess
	Imprimir "Ingrese 5 números:"
	resultado <- compareDistances()
	Si resultado Entonces
		Imprimir resultado ," - La suma de los números positivos está más lejos de 0."
	Sino
		Imprimir resultado ," - La suma de los números negativos está más lejos de 0."
	FinSi
FinAlgoritmo
```
## Week challenges (Tuesday) 💻

## 1. Sum of pairs
### Description
write a function called sumOfPairs that asks for a number from 1 to 100 indefinitely, if a negative number or greater than 100 is entered, it stops asking for more numbers and returns the sum of all the even numbers entered.

4, 12 , 100, 11, -60 --> 116

40, 121 --> 40

### Expected output
```PSeInt
Algoritmo exampleSumOfPairs
	Imprimir sumOfPairs()
FinAlgoritmo
```
### Solution 😎

## 2. Mid point
### Description
write a function called midpoint that given 2 values ​​(can be negative) does not return the value of the midpoint between them

-50,50 --> 0

40, 80 --> 60

### Expected output
```PSeInt
Algoritmo exampleMidpPoint
	Imprimir midPoint(40,80)
FinAlgoritmo
```
### Solution 😎
```PSeInt
Funcion result <- midPoint (valor1, valor2)
	// Calculate the midpoint between the two values
	result = (valor1 + valor2) / 2
	
	// Return the midpoint
	escribir result
FinFuncion

Algoritmo exampleMidPoint
// Call the midPoint function with the values 40 and 80
Imprimir midPoint(40, 80)

FinAlgoritmo
```

## Week challenges (Wednesday) 💻

## 1. Cashier
### Description
create a function called "cashier" that pretends to be a panel of a bank should display the text: "select an option: a. to deposit. b. withdraw. c. go out." and have a value called balance that will return when finished and will print it on the screen, its initial value will be 1000. You must repeat the menu until you select the option 'c'

if we select 'a' it invokes another function called 'deposit' that will display a text on the screen that will say 'how much do you want to deposit:' it will add that value to the balance and end the function.

if we select 'b' it invokes another function called 'withdraw' that will display a text on the screen that will say 'how much do you want to withdraw:' it will subtract that value from the balance and end the function.

"select an option: a. to deposit. b. withdraw. c. go out."

a -->

"how much do you want to deposit:"

500 -->

"select an option: a. to deposit. b. withdraw. c. go out."

b -->

"how much do you want to withdraw:"

1400 -->

"select an option: a. to deposit. b. withdraw. c. go out."

c -->

100

### Expected output
```PSeInt
Algoritmo exampleCashier
	Imprimir cashier()
FinAlgoritmo
```
### Solution 😎

## 2. Weather average
### Description
write an algorithm that loops indefinitely until 'x' is entered which will calculate an average of the weather, note that for each value entered it should ask if it is fahrenheit or celsius, then ask for the value. add everything up and divide by the number of values ​​entered. The result must be returned in celsius, have a function that, in case fahrenheit is entered, transforms it to celsius in order to add them.

Expected output
```PSeInt
Algoritmo exampleWeatherAverage

FinAlgoritmo
```
### Solution 😎


## Week challenges (Thursday) 💻

## 1. 'IF' statement in JavaScript
### Description
Create an if statement with the JavaScript syntax

### Expected output
A piece of code with an if written in JavaScript
### Solution 😎
```js
let x = 10;

if (x > 5) {
  console.log("x is greater than 5");
}
```
## 2. 'WHILE' loop in JavaScript
### Description
Create a while loop statement with the JavaScript syntax

### Expected output
A piece of code with a while using the JavaScript syntax
### Solution 😎
```js
let i = 0;

while (i < 5) {
  console.log("The value of i is: " + i);
  i++;
}
```
## 3. 'FOR' loop in JavaScript
### Description
Create a for loop with the JavaScript syntax

### Expected output
A piece of code with a for loop statement written in the JavaScript syntax
### Solution 😎
```js
for (let i = 0; i < 5; i++) {
  console.log("The value of i is: " + i);
}
```