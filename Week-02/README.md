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
