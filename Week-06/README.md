# Javascript - Week 06
## Week challenges (Tuesday) 💻

## 1. Variables
### Description
https://www.jshero.net/en/koans/var.html

### Solution 😎
```Javascript
let firstname = 'Lata';
```

## 2. What is x?
### Description
https://www.jshero.net/en/koans/jsx01.html

### Solution 😎
```Javascript
'Geeta'
```

## 3. Several variables
### Description
https://www.jshero.net/en/koans/var2.html
### Solution 😎
```Javascript
let flower =  'rose';
let tree = 'maple';
```

## 4. Reassignment
### Description
https://www.jshero.net/en/koans/jsx02.html

### Solution 😎
```Javascript
'Toe'
```

## 6. Assign variables
### Description
https://www.jshero.net/en/koans/jsx03.html

### Solution 😎
```Javascript
'Hardy'
```
# Javascript - Week 06
## Week challenges (Wednesday) 💻

## 1. Functions
### Description
https://www.jshero.net/en/koans/function.html

### Solution 😎
```Javascript
function hello () {
return 'Hello world!';
}
```

## 2. Multiple functions
### Description
https://www.jshero.net/en/koans/function2.html

### Solution 😎
```Javascript
function a () {return 'Hello a!';};
function b () {return 'Hello b!';};
```

## 3. Function calls
### Description

### Solution 😎
```Javascript
function greet() {return 'Haydo!'};
let salutation = greet();
```

## 4. What is x? (function version)
### Description
https://www.jshero.net/en/koans/jsx05.html

### Solution 😎
```Javascript
'How do you do?'
```

## 5. Parameters
### Description
https://www.jshero.net/en/koans/parameter.html

### Solution 😎
```Javascript
function echo (word) {return word;} 
```

# Javascript - Week 06
## Week challenges (Thursday) 💻

## 1. Strings
### Description
https://www.jshero.net/en/koans/string.html

### Solution 😎
```Javascript
function greet (word) {return 'Hello ' + word + '!';}
```
## 2. String: length
### Description
https://www.jshero.net/en/koans/stringlength.html

### Solution 😎
```Javascript
function length (word) {return word.length;}
```
## 3. String: toUpperCase()
### Description
https://www.jshero.net/en/koans/stringupper.html

### Solution 😎
```Javascript
function toCase (word) {return word.toLowerCase() + '-' + word.toUpperCase()}
```
## 4. String: charAt()
### Description
https://www.jshero.net/en/koans/stringcharat.html

### Solution 😎
```Javascript
function shortcut (word1, word2) {return word1.charAt(0) + word2.charAt(0)}
```

## 5. String: indexOf()
### Description
https://www.jshero.net/en/koans/stringindexof.html

### Solution 😎
```Javascript
function indexOfIgnoreCase (word1, word2) {
const lowerWord1 = word1.toLowerCase();
const lowerWord2 = word2.toLowerCase();

return lowerWord1.indexOf(lowerWord2);
}
```