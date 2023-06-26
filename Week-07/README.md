# Javascript - Week 07
## Week challenges (Monday) 💻

## 1. String: substr()
### Description
https://www.jshero.net/en/koans/stringsubstr.html

### Solution 😎
```Javascript
function firstWord (sentence) {return sentence.substring(0, sentence.indexOf(" "))}
```
## 2. String: replace()
### Description
https://www.jshero.net/en/koans/replace.html

### Solution 😎
```Javascript
function normalize (sentence) {
    const regex = /-/ig;
    return sentence.replaceAll(regex, "/")
};
```
## 3. Increment
### Description
https://www.jshero.net/en/koans/increment.html

### Solution 😎
```Javascript
7
```
## 4. Fahrenheit
### Description
https://www.jshero.net/en/koans/fahrenheit.html

### Solution 😎
```Javascript
function toFahrenheit(celsius) {
  const fahrenheit = (celsius * 9 / 5) + 32;
  return fahrenheit;
}
```
## 5. Boolean
### Description
https://www.jshero.net/en/koans/bool.html

### Solution 😎
```Javascript
function nand(a, b) {
    return a && b ? false : true;
}
```

## Week challenges (Tuesday) 💻
## 1. Objects
### Description
https://www.codewars.com/kata/571f1eb77e8954a812000837/train/javascript

### Solution 😎
```Javascript
function animal(obj){
   return "This " + obj.color + " " + obj.name + " has " + obj.legs + " legs.";
}
```
## 2. Return to Sanity
### Description
https://www.codewars.com/kata/514a7ac1a33775cbb500001e/train/javascript

### Solution 😎
```Javascript
function mystery() {
  var results =
    {sanity: 'Hello'};
  return
    results;
}
```
## 3. Grasshopper - Object syntax debug
### Description
https://www.codewars.com/kata/56d8ae9237123036d3001b54/train/javascript

### Solution 😎
```Javascript
var rooms = {
  first: {
    description: 'This is the first room'
    items: {
      chair: 'The old chair looks comfortable',
      lamp: 'This lamp looks ancient'
  },
  second: {
    description: 'This is the second room'
    items: {
      couch: 'This couch looks like it would hurt your back,
      table: 'On the table there is an unopened bottle of water'
    }
  }
}
```

## Week challenges (Wednesday) 💻
## 1. Count strings in objects
### Description
https://www.codewars.com/kata/565b3542af398bfb50000003/train/javascript

### Solution 😎
```Javascript
function strCount(obj){
// Your code here
  let count = 0;

  function countStrings(obj) {
    for (let key in obj) {
      if (typeof obj[key] === 'string') {
        count++;
      } else if (typeof obj[key] === 'object') {
        countStrings(obj[key]);
      }
    }
  }

  countStrings(obj);
  return count;
}
```
## 2. Extending JavaScript Objects: Get First & Last Array Element
### Description
https://www.codewars.com/kata/581351c40d8f13bc450008b8/train/javascript

### Solution 😎
```Javascript
Array.prototype.first = function () {
  return this[0];
};
Array.prototype.last = function () {
  return this[this.length -1];
};
```
## 3. OOP: Object Oriented Piracy
### Description
https://www.codewars.com/kata/54fe05c4762e2e3047000add/train/javascript

### Solution 😎
```Javascript
function Ship(draft,crew) {
 this.draft = draft;
 this.crew = crew;
}

//YOUR CODE HERE...
Ship.prototype.isWorthIt = function () {
  let draftAfterCrew = this.draft - (this.crew * 1.5);
  return draftAfterCrew > 20;
}
```

## Week challenges (Thursday) 💻
## 1. Convert a String to a Number!
### Description
https://www.codewars.com/kata/544675c6f971f7399a000e79/train/javascript

### Solution 😎
```Javascript
const stringToNumber = function(str){
  // put your code here
  let number = Number(str);
  return number;
}
```
## 2. Convert number to reversed array of digits
### Description
https://www.codewars.com/kata/5583090cbe83f4fd8c000051/train/javascript

### Solution 😎
```Javascript
function digitize(n) {
  //code here
  let digits = n.toString().split('');
  let reversedDigits = digits.reverse();
  let reversedNumber = reversedDigits.map(function(digit) {
    return Number(digit);
  });
  return reversedNumber;
}
```
## 3. Truthy and Falsy
### Description
https://www.codewars.com/kata/595c2988d946a13298000157/train/javascript

### Solution 😎
```Javascript
const truthy = [1, 'Hello', true, [], {}]; // At least 5 elements that evaluate to true
const falsy = [0, '', false, null, undefined]; // At least 5 elements that evaluate to false
```
## 4. Training JS #4: Basic data types--Array
### Description
https://www.codewars.com/kata/571effabb625ed9b0600107a/train/javascript

### Solution 😎
```Javascript
function getLength(arr){
  //return length of arr
  return arr.length;
}
function getFirst(arr){
  //return the first element of arr
  return arr[0]
}
function getLast(arr){
  //return the last element of arr
  return arr[arr.length -1]
}
function pushElement(arr){
  var el=1;
  //push el to arr
  arr.push(el);
  return arr
}
function popElement(arr){
  //pop an element from arr
  arr.pop()
  return arr
}
```