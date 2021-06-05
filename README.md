# cit281-p2

# Project 2: Isolating Functions and creating .gitignore files

### Overview
In this project I pracvticed refactoring code in order to seperate functions and eliminate global variables. I also gained more experience using git commands and creating .gitignore files

### Project Code
```markdown
/*
    CIT 281 Project 2
    Name: Devin Guardino
*/

// Returns a random number between min (inclusive) and max (exclusive)
const getRandomInteger = function(min, max) {
    return Math.floor(Math.random() * (max - min) + min);
}

//Returns a single random lowercase letter
const getRandomLetter = function() {
    const alphabet = "abcdefghijklmnopqrstuvwxyz"
    return alphabet[Math.floor(Math.random() * alphabet.length)]
  }

//Returns a string of random letters with a length between a minimum and maximum input value
const getRandomString = function(minLength, maxLength) {
    let result = "";

    for (let i = 0; i < getRandomInteger(minLength, maxLength); i++) {
        result = result + getRandomLetter();
    }

return result;
}

console.log(getRandomString(10, 20))

let getSortedString = string => string.toCharArray().sort();


console.log (getSortedString("sakjfhhfjsdfj"))
```

```markdown
/*
    CIT 281 Project 2
    Name: Devin Guardino
*/

// Returns a random number between min (inclusive) and max (exclusive)
function getRandomInteger(min, max) {
    return Math.floor(Math.random() * (max - min) + min);
}

//Returns a single random lowercase letter
function getRandomLetter() {
    const alphabet = "abcdefghijklmnopqrstuvwxyz"
    return alphabet[Math.floor(Math.random() * alphabet.length)]
  }

//Returns a string of random letters with a length between a minimum and maximum input value
function getRandomString(minLength, maxLength) {
    let result = "";

    for (let i = 0; i < getRandomInteger(minLength, maxLength); i++) {
        result = result + getRandomLetter();
    }

return result;
}

console.log(getRandomString(10, 20))

let getSortedString = string => string.toCharArray().sort();


console.log (getSortedString("sakjfhhfjsdfj"))
```
