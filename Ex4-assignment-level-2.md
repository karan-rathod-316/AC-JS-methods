## writeCode

```js
let words = [
  "mystery",
  "brother",
  "aviator",
  "crocodile",
  "pearl",
  "orchard",
  "crackpot",
  "rhythm"
];
// - Write a function findLongestWord that takes an array of words and returns the longest word from the array. (Use above array "words" to test it). If there are 2 with the same length, it should return the first occurrence.



// - Convert the above array "words" into an array of length of word instead of word.

let lenOfWords = words.map(word => word.length);
console.log(lenOfWords);


// - Create a new array that only contains word with atleast one vowel.

// - Find the index of the word "rhythm"
let indexOfRhythm = words.indexOf("rhythm");
console.log(indexOfRhythm);


// - Create a new array that contians words not starting with vowel.
let vowelStart = function(word) {
  let vowels = ["a","e","i","o","u"];
  return vowels.includes(word[0]);
}

let vowelStart = words.filter(vowelStart);
console.log(vowelStart);


// - Create a new array that contianse words not ending with vowel
let noVowelEnd = function(word) {
  let vowels = ["a","e","i","o","u"];
  return !vowels.includes(word[0]);
}
let vowelNotStart = words.filter(noVowelEnd);
console.log(noVowelEnd);



let numbers = [6, 12, 1, 18, 13, 16, 2, 1, 8, 10];

// - Create a sumArray function that takes an array of number as a parameter, and calculate the sum of all its numbers
let getSum = function(numbers) {
  let sum = numbers.reduce((sum,number) => sum + number,0);
  return sum;
}

console.log(getSum(numbers)); //87


// - Make a new array that contains number multiplied by 3 like [6, 18, 27 ...]
let tripledArray = numbers.map(number => number * 3);
console.log(tripledArray);


// - Create a new array that contains only even numbers
let isEven = function(number) {
  return number % 2 === 0;
}
let arrayOfEvenNums = numbers.filter(isEven);

// - Create  a new array that contains only odd numbers.
let isOdd  = function(number) {
  return number % 2 !== 0;
}
let oddNos = numbers.filter(isOdd);
console.log(oddNos);

// - Create a new array that should have true for even number and false for odd numbers.
let arrayOfBol = function(number){
  return number % 2 ? false : true
}
let trueFalseArr = numbers.map(arrayOfBol);
console.log(trueFalseArr);


// - Sort the above number in assending order.
let ascendingOrder = numbers.sort((a,b) => a - b);
console.log(ascendingOrder);

// - Does sort mutate the original array?
//Yes


// - Find the sum of the numbers in the array.
let sum = numbers.reduce((sum,number)=> sum + number, 0);
console.log(sum); 


//- Write a function averageNumbers that receives an array of numbers and calculate the average of the numbers

let strings = [
  "seat",
  "correspond",
  "linen",
  "motif",
  "hole",
  "smell",
  "smart",
  "chaos",
  "fuel",
  "palace"
];
// - Write a function averageWordLength that receives an array of words2 and calculate the average length of the words.
```

## String Methods-writeCode

- Write a JavaScript function to check whether input value is a string or not.

```js
/* Requirements
  @name isString
  @parameter (any value) val
  @return Boolean
*/

let isString = function(val) {
  return typeof val === "string";
}

// Test
console.log(isString("tony stark")); // true;
console.log(isString([1, 2, 4, 0])); // false;
```

- Write a JavaScript function to check whether a string is blank or not.

```js
/* Requirements
  @name isBlank
  @parameter (any value) val
  @return Boolean
*/

// your code goes here

// Test
console.log(isBlank("")); // true;
console.log(isBlank("abc")); // false;
```

- Write a JavaScript function to split a string and convert it into an array of words.

```js
/* Requirements
  @name stringToArray
  @parameter (string) text
  @return Array
*/
// your code goes here
let stringToArray = function(text) {
  let array = text.split(" ");
  return array;
}
// Test
console.log(stringToArray("Hello World")); // ["Robin", "Singh"];
console.log(stringToArray("Lady Bird")); // ["Lady", "Bird"];
```

- Write a JavaScript function to return specified number of characters from a string.

```js
/* Requirements
  @name truncate
  @parameter (string, number) text, len
  @return String
*/
// your code goes here

// Test
console.log(truncate("Robin Singh", 4)); //"Robi";
```

- Write a JavaScript function to convert a `string` in abbreviated form.

```js
/* Requirements
  @name abbrevName
  @parameter (string) fullName
  @return String
*/
// your code goes here

// Test
console.log(abbrevName("Robin Singh")); //"Robin S."
```

- Write a JavaScript function to hide email addresses to protect from unauthorized user.

```js
/* Requirements
  @name protect
  @parameter (string) email
  @return String
*/
// your code goes here

// Test
console.log(protect("robin_singh@example.com")); // "robin...@example.com"
```

- Write a JavaScript function to parameterize a string.

```js
/* Requirements
  @name parameterize
  @parameter (string) str
  @return String
*/
let parameterize = function(str) {
  let arrOfStr = str.split(" ").map(word => word.toLowerCase());
  return arrOfStr.join("-");
}

// Test
console.log(parameterize("Robin Singh from USA.")); // "robin-singh-from-usa"
```

- Write a JavaScript function to capitalize the first letter of a `string`.

```js
/* Requirements
@name capitalizeFirst
@parameter (string, number) text, len
@return String
*/
let capitalizeFirst = function(text,len) {
  return text[0].toUpperCase() + text.slice(1);
}


// Test
console.log(capitalizeFirst("js string exercises")); // "Js string exercises"
```

- Write a JavaScript function to capitalize the first letter of each word in a string.

```js

/* Requirements
  @name capitalizeWords
  @parameter (string) text
  @return String
*/

console.log(capitalizeWords("js string exercises")); // "Js String Exercises"
```

- Write a function that takes a string which has lower and upper case letters as a parameter and converts upper case letters to lower case, and lower case letters to upper case.

```js
/* Requirements
  @name swapcase
  @parameter (string) text
  @return String
*/
// your code goes here

// Tets
console.log(swapcase("AaBbc")); // "aAbBC"
```

- Write a function to convert a string into camel case.

Example:

```js
/* Requirements
  @name camelize
  @parameter (string) text
  @return String
*/
// your code goes here

// Test
console.log(camelize("JavaScript Exercises")); // "JavaScriptExercises"
console.log(camelize("JavaScript exercises")); // "JavaScriptExercises"
console.log(camelize("JavaScriptExercises")); // "JavaScriptExercises"
```

- Write a function to uncamelize a string. Example:

```js
/* Requirements
  @name uncamelize
  @parameter (string, string) text, joinStr
  @return String
*/
// your code goes here

// Tets
console.log(uncamelize("helloWorld", "_")); // "hello_world"
```

- Write a function to concatenates a given string n times (default is 1).

```js
/* Requirements
  @name repeat
  @parameter (string, number) text, times
  @return String
*/
let repeat = function(text,times) {
  return text.repeat(times);
}
// Test
console.log(repeat("Ha!", 3)); // "Ha!Ha!Ha!"
```

- Write a function to insert a string within a string at a particular position (default is 1).

```js
/* Requirements
  @name repeat
  @parameter (string, number) text, position
  @return String
*/
let insert = function(text,insertStr,position) {
  return text.slice(0,position) + insertStr + text.slice(position);
}

// Test
console.log(insert("We are doing some exercises.", "JavaScript ", 18)); // "We are doing some JavaScript exercises."
```

- Write a JavaScript function to humanized number (Formats a number to a human-readable string.) with the correct suffix such as 1st, 2nd, 3rd or 4th.

```js
/* Requirements
  @name humanize
  @parameter ( number) num
  @return String
*/
// your code goes here

// Test
console.log(humanize(301)); // "301st"
console.log(humanize(402)); // "402nd"
```

###

Write a function to truncates a string if it is longer than the specified number of characters. Truncated strings will end with a translatable ellipsis sequence ("…") (by default) or specified characters.

```js
/* Requirements
  @name testTruncate
  @parameter (string, number, string) text, len, postfix
  @return String
*/
// your code goes here

// Test
console.log(textTruncate("We are doing JS string exercises.", 15, "!!")); //"We are doing !!"
```

- Write a JavaScript function to chop a string into chunks of a given length.

```js
/* Requirements
  @name chop
  @parameter (string, number) text, size
  @return String
*/
let stringChop = function(text,size) {
  let chops = [];
  for(let i = 0; i < text.length / size; i++) {
    chops.push(text.slice(size * i, size * i + size))
  }
  return chops;
}

// Test
console.log(stringChop("hello world", 2)); // ["he", "ll", "o ", "wo", "rl", "d"]
```

- Write a function to count the occurrence of a substring in a string.

```js
/* Requirements
  @name count
  @parameter (string, string) text, char
  @return Number
*/
// your code goes here

// Test
console.log(count("The quick brown fox jumps over the lazy dog", "the")); // 2
```

- Write a function to strip leading and trailing spaces from a string.

```js
/* Requirements
  @name strip
  @parameter (string) text
  @return String
*/
let strip = function(text) {
  return text.trim();
}
// Test
console.log(strip("   Hello World ")); // "Hello World"
```

- Write a JavaScript function to truncate a string to a certain number of words.

```js
/* Requirements
  @name chopWords
  @parameter (string, number) text, words
  @return String
*/

// Test
console.log(chopWords("The quick brown fox jumps over the lazy dog", 4)); // "The quick brown fox"
```

- Write a function to alphabetize a given string.(A - z)

```js
/* Requirements
  @name alphabetize
  @parameter (string, number) text, times
  @return String
*/
let alphabetize = function(text,times) {
  return text.split("").sort().join("").trim();
}
// Test
console.log(alphabetize("United States")); // 'SUadeeinsttt'
```
