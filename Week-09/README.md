# Javascript - Week 08
## Week challenges (Monday) 💻

## 1. "this" is a problem
### Description
https://www.codewars.com/kata/547c71fdc5b2b38db1000098

### Solution 😎
```Javascript
function NameMe(first, last) {
    this.firstName = first;
    this.lastName = last;
    this.name = this.firstName + ' ' + this.lastName;
  return this.name;
}
```
## 2. Thinkful - List and Loop Drills: Lists of lists
### Description
https://www.codewars.com/kata/586e1d458cb711f0a800033b

### Solution 😎
```Javascript
function processData(data){
  
  let product = 1;
  
  for (let i = 0; i < data.length; i++) {
    let sublist = data[i];
    let difference = sublist[0] - sublist[1];
    product *= difference;
  }
  
  return product;
}
```
## 3. Stop gninnipS My sdroW!
### Description
https://www.codewars.com/kata/5264d2b162488dc400000001/

### Solution 😎
```Javascript
function spinWords(string){
  //TODO Have fun :)
    // Split the string into an array of words
  let words = string.split(' ');

  // Iterate over each word in the array
  for (let i = 0; i < words.length; i++) {
    // Check if the word has five or more letters
    if (words[i].length >= 5) {
      // Reverse the word using a helper function
      words[i] = reverseWord(words[i]);
    }
  }

  // Join the array of words back into a string
  let result = words.join(' ');

  // Return the resulting string
  return result;
}

// Helper function to reverse a word
function reverseWord(word) {
  return word.split('').reverse().join('');
}
```
## Week challenges (Tuesday) 💻

## 1. "this" is an other problem
### Description
https://www.codewars.com/kata/547f1a8d4a437abdf800055c

### Solution 😎
```Javascript
function NamedOne(first, last) {
// -- SHOULD be changed --
    this.firstName = first;
    this.lastName = last;
  
    Object.defineProperty(this, 'fullName', {
    get: function() {
      return this.firstName + ' ' + this.lastName;
    },
    set: function(value) {
      let names = value.split(' ');
      if (names.length === 2) {
        this.firstName = names[0];
        this.lastName = names[1];
      }
    }
  });
}

```
## 2. Who likes it?
### Description
https://www.codewars.com/kata/5266876b8f4bf2da9b000362

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
## 3. Convert string to camel case
### Description
https://www.codewars.com/kata/517abf86da9663f1d2000003

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
## Week challenges (Wednesday) 💻

## 1. Easy mathematical callback
### Description
https://www.codewars.com/kata/54b7c8d2cd7f51a839000ebf

### Solution 😎
```Javascript
function processArray(arr, callback) {
    // TODO
  var result = [];

  for (var i = 0; i < arr.length; i++) {
    result.push(callback(arr[i]));
  }

  return result;
}
```
## 2. Moving Zeros To The End
### Description
https://www.codewars.com/kata/52597aa56021e91c93000cb0

### Solution 😎
```Javascript
function moveZeros(arr) {
  let result = [];
  let zeros = [];
  
  for (let i = 0; i < arr.length; i++) {
    if (arr[i] === 0){
      zeros.push(arr[i]);
    }else{
      result.push(arr[i]);
    }
  }
  return result.concat(zeros)
}
```
## 3. Valid Parentheses
### Description
https://www.codewars.com/kata/52774a314c2333f0a7000688

### Solution 😎
```Javascript
function validParentheses(parens){
  var stack = [],
    i;
  
  for (i = 0; i < parens.length; i++) {
    if (parens[i] === '(') {
      stack.push(parens[i]);
    }
    else if('(' !== stack.pop()) {
      return false;
    }
  }
  
  return stack.length === 0;
}
```
## Week challenges (Thursday) 💻

## 1. The Hashtag Generator
### Description
https://www.codewars.com/kata/52449b062fb80683ec000024

### Solution 😎
```Javascript
function generateHashtag (str) {
    if (str.trim() === '') {
    return false;
  }

  const words = str.trim().split(' ');
  const capitalizedWords = words.map(word => word.charAt(0).toUpperCase() + word.slice(1));
  const hashtag = '#' + capitalizedWords.join('');

  if (hashtag.length > 140) {
    return false;
  }

  return hashtag;
}
```
## 2. String incrementer
### Description
https://www.codewars.com/kata/54a91a4883a7de5d7800009c

### Solution 😎
```Javascript
function incrementString (str) {
    const regex = /(.*?)(\d*)$/;
  const match = str.match(regex);
  const base = match[1];
  let number = match[2] || '';

  if (number === '') {
    return str + '1';
  }

  const digits = number.length;
  const incrementedNumber = (parseInt(number) + 1).toString().padStart(digits, '0');

  return base + incrementedNumber;
}
```