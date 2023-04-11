# Algorithms - Week 1

## (Wednesday) 💻

## 1. Pizza Recipe 🍕

### Description

Design an algorithm to prepare a pizza from scratch. Define the ingredients, what will be the flavor and the preparation.

### Solution 😎

1. Preheat your oven to 450°F (230°C).
2. Roll out your pizza dough on a floured surface and transfer it to a baking sheet.
3. Spread tomato sauce over the dough, leaving a 1-inch (2.5 cm) border around the edges.
4. Sprinkle shredded mozzarella cheese over the sauce.
5. Add your desired toppings, such as sliced mushrooms, bell peppers, onions, and pepperoni.
6. Bake the pizza in the preheated oven for 10-12 minutes or until the crust is golden brown and the cheese is melted and bubbly.
7. Remove the pizza from the oven and let it cool for a few minutes before slicing and serving.

## 2. Hot N Cold 🤒 🧊 🔥

### Description
Define an algorithm that is able to convert temperatures from Celsius to Fahrenheit and vice versa.

### Solution 😎
To convert Celsius to Fahrenheit:

1. Take the Celsius temperature as input.
2. Multiply the Celsius temperature by 1.8.
3. Add 32 to the result of step 2.
4. The resulting value is the Fahrenheit temperature.
---
To convert Fahrenheit to Celsius:

1. Take the Fahrenheit temperature as input.
2. Subtract 32 from the Fahrenheit temperature.
3. Divide the result of step 2 by 1.8.
4. The resulting value is the Celsius temperature.

## 3. Some geometry 📐
### Description
Design an algorithm to calculate the volume of a pyramid, a cube and a sphere.

### Solution 😎

To calculate the volume of a pyramid:

1. Take the base length, base width, and height of the pyramid as inputs.
2. Multiply the base length by the base width to get the area of the base.
3. Multiply the area of the base by the height of the pyramid.
4. Divide the result of step 3 by 3.
5. The resulting value is the volume of the pyramid.
---

To calculate the volume of a cube:

1. Take the length of one side of the cube as input.
2. Cube the length of one side.
3. The resulting value is the volume of the cube.
---

To calculate the volume of a sphere:

1. Take the radius of the sphere as input.
2. Cube the radius.
3. Multiply the result of step 2 by 4/3 and by pi (3.14159).
4. The resulting value is the volume of the sphere.

## (Thursday) 💻

## 1. Numbers 📈
### Description
Design an algorithm to check if a number is even or odd. If it is even, write that it is even, otherwise write that it is odd. Represent the algorithm in a flowchart.

### Expected output
A graph showing the steps to verify if a number is even or odd

### Solution 😎
1. Start
2. Read the input number
3. Divide the number by 2
4. Check if the remainder is equal to 0
5. If the remainder is 0, then the number is even. Output "The number is even."
6. If the remainder is not equal to 0, then the number is odd. Output "The number is odd."
7. Stop

Here is the flowchart representation of the algorithm:

<p><img src="https://raw.githubusercontent.com/FacundoDLR/core-code-from-scratch-readme/main/assets/evenVsOdds.jpg" alt="facundodlr" /></p>

## 2. How old are you 👴
### Description
Write pseudocode for an algorithm that calculates the age of a person based on date of birth

### Expected output
A sequence that tells you how old is someone based on DOB

### Solution 😎
1. Start
2. Read the person's date of birth (dob)
3. Calculate the current date (current_date)
4. Calculate the person's age by subtracting the year of birth from the current year
5. Output the person's age
6. End

## Find the treasure 👑

### Description
We are in a room with three chests. We know that at least one has a treasure in it. Each chest has a message, but all the messages are lies.

- Left chest: The middle chest has a treasure
- Middle chest: All these chests have treasures in them
- Right chest: Only one of these chests has treasures.

### Expected output
Identify which chests have treasures

### Solution 😎
We are in a room with three chests. We know that at least one has a treasure in it. Each chest has a message, but all the messages are lies.

Since each chest has a message and all the messages are lies, we need to remove the illogical options or contradictions.

- The message on the left chest says that the middle chest has a treasure, but we know that all the messages are lies. Therefore, the middle chest does not have a treasure and the left chest's message is false.

- The message on the middle chest says that all the chests have treasures, but we already know that not all the chests have treasures, but some might. Therefore, the message on the middle chest is also false.

- The message on the right chest says that only one of the chests has treasure. Since we know that at least one chest has a treasure, this message must be false. It is not possible for only one of the chest to have treasure.

Since we know that at least one has treasure, as we read in the instructions, the only possible is 'left and right have treasures'.

So the answer is chest A and chest C.
