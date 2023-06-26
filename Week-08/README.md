# Javascript - Week 08
## Week challenges (Monday) 💻

## 1. Training JS #7: if..else and ternary operator
### Description
https://www.codewars.com/kata/57202aefe8d6c514300001fd/train/javascript

### Solution 😎
```Javascript
function saleHotdogs(n){
  let price;
  
  if( n < 5)  {
    price = 100
  }else if (n >= 5 && n < 10) {
    price = 95;
  }else{
    price = 90;
  }
  
  let totalPrice = price * n;
  return totalPrice;
}
```
## 2. Training JS #8: Conditional statement--switch
### Description
https://www.codewars.com/kata/572059afc2f4612825000d8a/train/javascript

### Solution 😎
```Javascript
function howManydays(month){
  switch (month) {
    case 2:
      return 28;
    case 4:
    case 6:
    case 9:
    case 11:
      return 30;
    default:
      return 31;
  }
}
```
## 3. Basic Calculator
### Description
https://www.codewars.com/kata/5296455e4fe0cdf2e000059f/train/javascript

### Solution 😎
```Javascript
function calculate(num1, operation, num2) {
   switch (operation) {
    case "+":
      return num1 + num2;
    case "-":
      return num1 - num2;
    case "*":
      return num1 * num2;
    case "/":
      if (num2 !== 0) {
        return num1 / num2;
      } else {
        return null;
      }
    default:
      return null;
  }
}
```

## Week challenges (Tuesday) 💻
## 1. Even or Odd
### Description
https://www.codewars.com/kata/53da3dbb4a5168369a0000fe/train/javascript

### Solution 😎
```Javascript
function evenOrOdd(number) {
    if (number % 2 === 0) {
    return "Even";
  } else {
    return "Odd";
  }
}
```
## 2. A wolf in sheep's clothing
### Description
https://www.codewars.com/kata/5c8bfa44b9d1192e1ebd3d15/train/javascript

### Solution 😎
```Javascript
function warnTheSheep(queue) {
  const wolfIndex = queue.findIndex((animal) => animal === "wolf");
  const sheepNumber = queue.length - wolfIndex - 1;

  if (wolfIndex === queue.length - 1) {
    return "Pls go away and stop eating my sheep";
  } else {
    return `Oi! Sheep number ${sheepNumber}! You are about to be eaten by a wolf!`;
  }
}
```
## 3. Decode the Morse code
### Description
https://www.codewars.com/kata/54b724efac3d5402db00065e/train/javascript

### Solution 😎
```Javascript
decodeMorse = function(morseCode){
    const words = morseCode.trim().split("   ");
  const decodedMessage = words
    .map((word) => {
      const letters = word.split(" ");
      const decodedWord = letters
        .map((letter) => MORSE_CODE[letter])
        .join("");
      return decodedWord;
    })
    .join(" ");

  return decodedMessage;
}
```

## Week challenges (Wednesday) 💻
## 1. Who likes it?
### Description
https://www.codewars.com/kata/5266876b8f4bf2da9b000362/train/javascript

### Solution 😎
```Javascript
function likes(names) {
  // TODO
  let count = names.length;
  
  if (count === 0) {
    return "no one likes this";
  } else if (count === 1) {
    return names[0] + " likes this";
  } else if (count === 2) {
    return names[0] + " and " + names[1] + " like this";
  } else if (count === 3) {
    return names[0] + ", " + names[1] + " and " + names[2] + " like this";
  } else {
    return names[0] + ", " + names[1] + " and " + (count - 2) + " others like this";
  }
}
```
## 2. Bit Counting
### Description
https://www.codewars.com/kata/526571aae218b8ee490006f4/train/javascript

### Solution 😎
```Javascript
var countBits = function(n) {
    let count = 0;
  let binaryString = n.toString(2); // Convert number to binary string

  for (let i = 0; i < binaryString.length; i++) {
    if (binaryString[i] === "1") {
      count++;
    }
  }

  return count;
};
```
## 3. Your order, please
### Description
https://www.codewars.com/kata/55c45be3b2079eccff00010f/train/javascript

### Solution 😎
```Javascript
function order(string){
    if (string === "") {
    return "";
  }

  const words = string.split(" ");
  const sortedWords = [];

  for (let i = 1; i <= 9; i++) {
    const filteredWords = words.filter((word) => word.includes(i.toString()));
    sortedWords.push(...filteredWords);
  }

  return sortedWords.join(" ");
}
```

## Week challenges (Thursday) 💻
## 1. Counting Duplicates
### Description
https://www.codewars.com/kata/54bf1c2cd5b56cc47f0007a1/train/javascript

### Solution 😎
```Javascript
function duplicateCount(input){
    const charCount = {};
  const lowerCaseInput = input.toLowerCase();
  let count = 0;

  for (let i = 0; i < lowerCaseInput.length; i++) {
    const char = lowerCaseInput[i];

    if (/[a-z0-9]/.test(char)) {
      charCount[char] = (charCount[char] || 0) + 1;

      if (charCount[char] === 2) {
        count++;
      }
    }
  }

  return count;
```
## 2. Encrypt this!
### Description
https://www.codewars.com/kata/5848565e273af816fb000449/train/javascript

### Solution 😎
```Javascript
var encryptThis = function(message) {
    const words = message.split(" ");
  const encryptedWords = [];

  for (let i = 0; i < words.length; i++) {
    const word = words[i];

    if (word === "") {
      encryptedWords.push("");
    } else {
      const firstLetterAscii = word.charCodeAt(0);
      const switchedLetters = switchLetters(word);
      encryptedWords.push(`${firstLetterAscii}${switchedLetters}`);
    }
  }

  return encryptedWords.join(" ");
}

function switchLetters(word) {
  if (word.length <= 2) {
    return word.slice(1);
  } else {
    const secondLetter = word[1];
    const lastLetter = word[word.length - 1];
    const middleLetters = word.slice(2, word.length - 1);
    return lastLetter + middleLetters + secondLetter;
  }
}
```
## 3. Valid Parentheses
### Description
https://www.codewars.com/kata/52774a314c2333f0a7000688/train/javascript

### Solution 😎
```Javascript
function validParentheses(parens) {
  // your code here ..
  let stack = [];

  for (let i = 0; i < parens.length; i++) {
    let char = parens.charAt(i);

    if (char === "(") {
      stack.push(char);
    } else if (char === ")") {
      if (stack.length === 0 || stack.pop() !== "(") {
        return false;
      }
    }
  }

  return stack.length === 0;
}
```
## 4. Convert string to camel case
### Description
https://www.codewars.com/kata/517abf86da9663f1d2000003/train/javascript

### Solution 😎
```Javascript
function toCamelCase(str){
  let words = str.split(/[-_]/);
  let result = words[0];

  for (let i = 1; i < words.length; i++) {
    let capitalizedWord = words[i].charAt(0).toUpperCase() + words[i].slice(1);
    result += capitalizedWord;
  }

  return result;
}
```