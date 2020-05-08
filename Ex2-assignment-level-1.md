# String Methods

## Practice String Methods-writeTextAnswer

Go to this [link](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/charAt) and look for the name of method to learn about it.

**Write in your own way of understanding (dont copy paste)**

Only if you are done with step 1 you should go ahead.

1. Practice it by yourself in console (4-5 times to understand)
2. Data types of parameters
3. Return value type
4. Example (3)
5. In your words what this method does.

Example:

1. `charAt`

   - This method accepts one parameter (index) of number data type.
   - It returns the charater on specific index (provided through parameter)
   - Example:
     ```js
     let name = "Arya Stark";
     name.charAt(2); //"y"
     let sentance = "A quick brown fox jumped over a lazy dog";
     sentance(4); // "i"
     let houseName = "Starks";
     houseName.charAt(0); // "S"
     ```
   - `charAt` accepts a index (number data type) and return the character on that index.

2. `toUpperCase`

  - ToUpperCase doesn't require any kind of parameters
  - This method changes a string to uppercase   
  - Example: 
    let name = "Robin Singh";
     name.toUpperCase(); //"ROBIN SINGH"
     let sentence = "a for apple";
     sentence.toUpperCase();// "A FOR APPLE";
     let dogName = "poachie";
     dogName.toUpperCase(); // "POACHIE"
  - toUpperCase converts a string to uppercase(the changes aren't made in the variables though, it just displays the strings in upper case.)


3. `toLowerCase`
  - ToUpperCase doesn't require any kind of parameters
  - This method changes a string to lowercase   
  - 
  - Example: 
   let name = "Robin Singh";
     name.toLowerCase(); //"robin singh"
     let sentence = "A FOR APPLE";
     sentence.toLowerCase();// "a for apple";
     let dogName = "POACHIE";
     dogName.toLowerCase(); // "poachie"
  - toLowerCase converts a string to lowercase(the changes aren't made in the variables though, it just displays the strings in lower case.)

4. `trim`
  - Trim doesn't need any parameters
  - It removes the white space before and after characters
  - Example: 
   let name = "   Robin Singh   ";
     name.trim(); //"Robin Singh"
     let sentence = "    A FOR APPLE        ";
     sentence.trim();// "A FOR APPLE";
     let dogName = "   POACHIE   ";
     dogName.trim(); // "POACHIE"   
  - Trim removes white space and returns the string(the changes aren't made in the variable though)

5. `trimEnd`
  - TrimEnd doesn't need any parameters
  - It removes the white space after characters
  - Example: 
   let name = "   Robin Singh   ";
     name.trimEnd(); //"   Robin Singh"
     let sentence = "    A FOR APPLE        ";
     sentence.trimEnd();// "    A FOR APPLE";
     let dogName = "   POACHIE   ";
     dogName.trimEnd(); // "   POACHIE"   
  - TrimEnd removes white space at the end and returns the string(the changes aren't made in the variable though)

6. `trimStart`
  - TrimStart doesn't need any parameters
  - It removes the white space before the characters
  - Example: 
   let name = "   Robin Singh   ";
     name.trimEnd(); //"Robin Singh   "
     let sentence = "    A FOR APPLE        ";
     sentence.trimEnd();// "A FOR APPLE        ";
     let dogName = "   POACHIE   ";
     dogName.trimEnd(); // "POACHIE   "   
  - TrimStart removes white space at the start and returns the string(the changes aren't made in the variable though)

7. `concat`
  - Concat accepts multiple parameters
  - It fuses multiple string to create one single string
  - Example: 
      let a = "Hey ";
      let b = "There";
      a.concat(b)//"Hey There"
      let c = ", What's up?"
      a.concat(b,c)//"Hey There, What's up? "
      let d = "Google is watching us!"
      a.concat(b,c,d) //"Hey There, What's up? Google is watching us!" 
  - Concat fuses multiple strings and makes them one. It doesn't have any effect on the original variables. 

8. `endsWith`
  -  This method accepts two parameters. The first one is used to search the particular string/part of string, the second one is optional and sets the length of the string. 
  -  It tells you whether a string ends with certain characters
  -  Example: 
     let name = "Karan";
     let search = "ran";
     name.endsWith(search);//true
     name.endsWith("ar", 3);// true    
    name.endsWith("x");//false
  - This method checks if the string ends with certain characters. //CASE SENSITIVE

9. `includes`
  - Include accepts two parameters : one is the searchValue and the other is of number
  - it checks if a certain character/string is present in the array
  - Example: 
let name = "Karan";
     let search = "ara";
     name.includes(search);//true
     name.includes("ar", 1);// true    
    name.includes("x");//false   

  - In simple words, it allows us to search a string within a string. 

10. `indexOf`
  - It accepts two parameters, search term and and integer from which you have to start searching. 
  - It returns the index of the element
  - Example: 
    const abc = ["who", "def", "ghi", "jkl"]
    let searchTerm = "ghi";
    abc.indexOf(searchTerm);//2
    abc.indexOf("jkl");//3
    searchTerm = "who";
    abc.indexOf(searchTerm, 3);//-1
  - This method takes the search term, and finds its index. It even  takes an integer as a starting point to find the string. Also, it returns -1 if it can't find the index for the given search term. 

11. `lastIndexOf`
  -  Accepts two parameters: search term and fromIndex
  -  It shows the index of the last element of a string
  -  Example: 
      const names = ["Hound", "Mountain", "Beric", "Hound"] 
      let searchName = "Hound";
      colors.lastIndexOf(searchName);// 3
      colors.lastIndexOf("Mountain");// 1
      colors.lastIndexOf("Beric");// 2
  - This method looks for the last index of your search term.

12. `padEnd`
  -  This method accepts two parameters. One is the lenght of the string that you want to extend and two is the chacter(s)
  - Applies extra characters to the end of the string
  - Example: 
     let x = "egg";
     x.padEnd(5,"g");//eggggg
     let x = "bake";
     x.padEnd(9,"e");//bakeeeeeee
     x.padEnd(10," ");//bake       ;
  - This method adds content to the end of a string

13. `padStart`
  - Accept two parameter, string length and character to be added 
  - Applies extra characters to the start of the string
  - Example: 
    let x = "egg";
     x.padStart(10,"e");//eeeeeeeeegg
     let x = "bake";
     x.padStart(9,"b");//bbbbbbbake
     x.padStart(10," ");//       bake;
  - This method adds content to the start of a string  


14. `repeat`
  - One parameter - a number to repeat the string as many times as you want
  - Repeats the string
  - Example: 
   let name = "blip";
   name.repeat(2);//"blipblip"
  
   name.repeat(0);//" "
  
   name.repeat(-5);//error 
  - Repeat method just repeats the string using the given number

15. `replace`
  - Accepts two parameters, string that needs to be changed and the new string that you need to replace it with 
  - replaces the string
  - Example: 
   let x = "Hello World";
   x.replace("Hello", "Hi")//Hi World

   x.replace("World", "Universe")//Hello Universe
  
   x.replace("World", " ")//Hello 
  - Basically, this method replaces the content in the string

16. `slice`
  - Takes two indexes as parameters
  - This method slices extracts characters from one string and creates a new one

  - Example: 
   let city = "Delhi";
   city.slice(2); //hi

   city.slice(1);//lhi

   city.slice(0, 2);// Del
  - This method extracts data from a string to create a new one

17. `split`
  - Takes 2 parameters, one is separator and one is the limit of the length 
  - This method splits the string into arrays 
  - Example: 
   
   let game = "cricket";
   game.split("") //["c", "r", "i", "c", "k", "e", "t"]
   game = "cricket , volleyball"
   game.split(",");// ["cricket", "volleyball"]  
  
   game.split();// ["cricket"]
  - This method splits a string into arrays based on your input

18. `substring`
  - Takes two parameters, one is index start and the other is index end
  - Returns a part of a string starting from the index start point
  - Example: 
   
   let name = "Ghost";
   name.substring(1,4);//host

   name.substring(1);//host
  
   name.substring(3);//st
  - Extract a part of a string


## writeCode

Using above methods you practiced above, do the following.

```js
let from = "Syrio Forel";
let quote = "There is only one thing we say to death: Not today";
let to = "Arya Stark";

/*
1. Find the index of the first 'is' in the variable quote. And store it in a new variable named indexOfIs
*/
// Your code goes here
let indexOfIs = quote.indexOf("is"); //ANS : 6
/*
2. Find the character at, the index indexOfIs (Problem 1) in quote.
*/
//Unable to understand the question

/*
3. Log the message saying `The index of first is in quote is 7`
*/
 //Unable to understand the question


/*
4. Log the message for first 6 characters of quote like this.
The character at index 0 is 'T'
The character at index 1 is 'h'
The character at index 2 is 'e'
The character at index 3 is 'r'
The character at index 4 is 'e'
The character at index 5 is ' '
*/
let arr = quote.split("", 6);
function log(char, index) {
  console.log(`The character at index ${index} is ${char}`)
}
arr.forEach(log)

/*
5. Using the variable from , to and quote variable dispaly this message
"Syrio Forel said There is only one thing we say to death: Not today to Arya Stark." (use concat method)
*/

from.concat(" said ", quote," to ",to);


/*
6. Does from, to and quote ends with "rk". Check all three.
*/
from.endsWith("rk"); //false
to.endsWith("rk");  //false
quote.endsWith("rk"); //true
/*
7. Does quote includes the word "Only"
*/
quote.includes("Only") // false

/*
8. Does quote includes the word " we"
*/
quote.includes(" we"); // true

/*
9. Find the index of the the word `we` in quote
*/
quote.indexOf("we");

/*
10. Split the quote into individual word and store it in a variable name quoteSplitted
*/
let quoteSplitted = quote.split(" ");
/*
11. Change the word "today" in quoteSplitted to "tomorrow" and join all the words to form a sentance.
*/
quoteSplitted[quoteSplitted.length - 1] = "tomorrow";
quoteSplitted.join(" ");


/*
12. Find the index of second "o" in quote. Use indexOf
*/
let indexOfFirstO = quote.indexOf("o");
quote.indexOf("o",indexOfFirstO + 1);

/*
13. Find the last index of letter "a" in quote.
*/
quote.lastIndexOf("a")

/*
14. Find the second last index of letter "a" in quote.
*/
let lastIndexOfA = quote.lastIndexOf("a");
quote.lastIndexOf("a",lastIndexOfA);


/*
15. Make the quote 70 character long. If it has less characters add rest as .......
Example: "Hello" (convert to 10 characters) => "Hello....."
*/
quote.padEnd(70,".");

/*
16. Do same as (15) but the ... should come in start.
*/
quote.padStart(70,".");

/*
17. Log the repeat of "Hello World!" 10 times.
*/
"Hello World!".repeat(10);

/*
18. Replace today to tomorrow in quote.
*/
let replacedStr = quote.replace("today", "tomorrow");

/*
19. Replace Stark to Lannister in quoteTo
*/
let surname = to.replace("Stark","Lannister");

/*
20. Make the quote of length 30 and put ... at the end. (use slice)
*/
quote.slice(0,27).padEnd(30,".");

/*
21. Find out does quote, quoteFrom, quoteTo starts with "A"
*/
quote.startsWith("A"); //false
quote.startsWith("A"); //false
quote.startsWith("A"); //true


## Practice Array Methods-writeTextAnswer

Go to this [link](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array#) and look for the name of method to learn about it.

**Write in your own way of understanding (dont copy paste)**

Only if you are done with step 1 you should go ahead.

1. Practice it by yourself in console (2-3 times to understand)
2. Data types of parameters
3. Return value type
4. Example (3)
5. In your words what this method does.
6. Does it mutate the original value (check https://doesitmutate.xyz)

Example:

1. `concat`

   - n(any) number of values (number, string, boolean, array, null, undefined, object and function.)
   - It returns a single Array consisting of by all the values passed as parameters in the same order.
   - Example:
     ```js
     let numbers = [1, 2, 3];
     numbers.concat(4); //[1,2,3,4]
     let sentanceArray = "A quick brown fox jumped over a lazy".split(" ");
     sentanceArray.concat("dog").join(" "); //"A quick brown fox jumped over a lazy dog"
     let colors = ["red", "green", "blue"];
     colors.concat("black", "red", 21, true); // ['red','green','blue','black', 'red', 21, true]
     ```
   - `concat` accepts n number of values and returns one array with all the values in same order. It doesnot change the original array.
   - No it doesnot mutate the original array

2. `join`
 - This method accepts one parameter(separator) that is optional, the default separator is a comma
 - It fuses all the elements
 let fullName = ["Stone Cold","Steve","Austin"]
 fullName.join();//"Stone Cold, Steve, Austin";

 fullName.join(" ");//"Stone Cold Steve Austin";

 This method allows you to combine items within the array

3. `flat`
It accepts one optional parameter that is of depth
Flat is used to reduce number of brackets in a nested array

var x = [1,2,3,4, [5,6,7,[8,9,10]]]
x.flat();//[ 1, 2, 3, 4, 5, 6, 7, (3) […] ]

x.flat(2);// [ 1, 2, 3, 4, 5, 6, 7, 8, 9, 10 ]

x.flat(1);// var x = [1,2,3,4, 5,6,7,[8,9,10]]

Flat method helps to remove nesting from an array

4. `push`
This method needs one or more parameters
It adds values to an array

let cars = ["Maruti","Honda","Lambhorgini"]

cars.push("Merc");//adds merc to the list

cars.push(); //  no changes

cars.push ("Bugatti", "Ashton Martin")

Push adds elements towards the end of an array

5. `indexOf`
Accepts two parameters - String of which index you want and a number stating whether you are looking at the first, second or any other string with the samle value

let cars = ["Maruti","Honda","Lambhorgini", "Honda", "Maruti"]

cars.indexOf("Honda");// 1
cars.indexOf("Honda", 2);// 3
cars.indexOf("Bajaj");//-1

This method checks the index of an array and reflects it.

6. `lastIndexOf`
Similar to the previous method, but looks for the last occurence of the index

Examples:
let cars = ["Maruti","Honda","Lambhorgini", "Honda", "Maruti"]

cars.lastIndexOf("Honda");//2)
cars.lastIndexOf("Maruti");//4)
cars.lastIndexOf("caer");//-1)

This method checks the last occurence of index of an array and reflects it.


7. `includes`
Takes two parameters - value to find and it's starting index.

It returns the values in true or false based on whether the value is included

Examples :
let cars = ["Maruti","Honda","Lambhorgini", "Honda", "Maruti"]

cars.includes("Maruti");//True
cars.includes("Ferrari");//False
cars.includes("Honda");//True

THis method checks if a certain value is there in the array.

8. `reverse`
Accepts no parameters
Returns a reversed array

let cars = ["Maruti","Honda","Lambhorgini", "Honda", "Maruti"]
cars.reverse()// [ "Maruti", "Honda", "Lambhorgini", "Honda", "Maruti" ]

THis method just reverses the entire array and mutates the structure of the array


9. `every`



10. `shift`
Accepts no parameters
Removes and returns the first element of an array

let alcohol = ["old monk", "signature", "blue lablel"];
alcohol.shift();//["signature", "blue lablel"];

let numbers = [10,11,12,14];
numbers.shift();//[11,12,14]

let games = ["gta", "COD", "pubg"]
games.shift();//["COD", "pubg"]
Shift removes the first element of an array

11. `splice`
Accepts three parameters - starting index, deleteCount and items to be placed in the array. deleteCOunt and items are optional but if you only mention the starting index it will delete the arrays after that index.

let names = ['ed','edd','eddie'];
names.splice(1,1) // starts from 1 and removes 1

names.splice(1, 0, 'dexter');//adds 'dexter to the list

names.splice(0, 1, "popeye")// starts from ed, removes ed and adds popeye

Splice can be used to add/delete/replace string in an array

12. `find`

13. `unshift`
Accepts no parameters
Removes and returns the last element of an array

let alcohol = ["old monk", "signature", "blue lablel"];
alcohol.unshift();//["old monk", "signature"];

let numbers = [10,11,12,14];
numbers.shift();//[10, 11,12]

let games = ["gta", "COD", "pubg"]
games.shift();//["gta","COD"]
Shift removes the first element of an array

14. `findIndex`

15. `filter`

Creates a new array with elements that pass a certain test

var numbers = [1, 3, 6, 8, 11];

var lucky = numbers.filter(function(number) {
  return number > 7;
});

// [ 8, 11 ]

16. `flat`
This method removes array nestings 

const animals = [['1', '2'], ['3', '4']];

const flatAnimals = animals.flat();

console.log(flatAnimals);

// ['1', '2', '3', '4']

17. `forEach`
This method lets you access each element in an array

const letters = ['a', 'b', 'c'];

letters.forEach((letter, index, arr) => {
  console.log(letter,index, arr);
});

// The console will output
// 'a', 0, ['a', 'b', 'c']
// 'b', 1, ['a', 'b', 'c']
// 'c', 2, ['a', 'b', 'c']


18. `map`

THis mehtod iterates over an array and creates a new array of the same size

var names = ["tom”, “jerry”, “ron”];

var newNames = names.map(function(name) {
	return ‘weird ’ + name;
});


19. `pop`
Removes an item from the end of an array

let dogs = ['pachie', 'hippo', 'kalu'];

dogs.pop();

20. `reduce`

21. `slice`
The slice method returns a new array with a copied element from the original array.

const myArr = ['1', '2', '3', '4'];

const myArrCopy = myArr.slice();

console.log(myArrCopy); // ['1', '2', '3', '4']


const myArrCopy = myArr.slice(2);

console.log(myArrCopy); // ["1", "2"]




## writeCode

Using above methods you practiced above, do the following.

```js
// Use the below two arrays and practice array methods
var numbers = [1, 12, 4, 18, 9, 7, 11, 3, 101, 5, 6, 9];
var strings = ["This", "is", "a", "collection", "of", "words"];

// - Find the index of `101` in numbers

let index101=numbers.indexOf(101);
console.log(index101)//8

// - Find the last index of `9` in numbers
let lastIndex = numbers.lastIndexOf(9)
console.log(index101)// 11

// - Convert value of strings array into a sentance like "This is a collection of words"
let fusedSent = strings.join(" ");
console.log(fusedSent)// 

// - Add two new words in the strings array "called" and "sentance"
strings.push("called", "sentence")


// - Again convert the updated array (strings) into sentance like "This is a collection of words called sentance"
newStrings = strings.join(" ")



// - Remove the first word in the array (strings)
strings.shift()


// - Find all the words that contain 'is' use string method 'includes'
let WordsIs = function(word) {
return word.includes("is")
}

strings.filter(WordsIs)


// - Find all the words that contain 'is' use string method 'indexOf'


// - Check if all the numbers in numbers array are divisible by three use array method (every)
let checkIfDivisble = function(num) {
  return num % 3 === 0;
}
numbers.every(checkIfDivisible)//false

// -  Sort Array from smallest to largest
numbers.sort(function(a, b) {
    return a - b;
});

// - Remove the last word in strings
strings.(pop)


// - Find largest number in numbers
Math.max.apply(null, numbers))


// - Find longest string in strings

// - Find all the even numbers
let EvenNums = function(number) {
  return number % 2 === 0;
}
let even = numbers.filter(EvenNums);
console.log(even);

// - Find all the odd numbers

let OddNums = function(number) {
  return number % 2;
}
let odd = numbers.filter(OddNums);
console.log(odd);

// - Place a new word at the start of the array use (upshift)
strings.unshift("goa");


// - Make a subset of numbers array [18,9,7,11]
let Sub = numbers.slice(3,7);
console.log(Sub);


// - Make a subset of strings array ['a','collection']
let stringSub = strings.slice(2,4);
console.log(stringSub);



// - Replace 12 & 18 with 1221 and 1881
let replaceVal = function(number) {
  if(number == 12) return 1221;
  if(number == 18) return 1881;
  return number;
}
let replaceNumbers = numbers.map(replaceVal);
console.log(replaceNumbers);

// - Replace words in strings array with the length of the word
let stringLengths = function(word) {
  return word.length;
}
let newString = strings.map(stringLengths);
console.log(newString);//


// - Find the sum of the length of words using above question

// - Customers Array
var customers = [
  { firstname: "Joe", lastname: "Blogs" },
  { firstname: "John", lastname: "Smith" },
  { firstname: "Dave", lastname: "Jones" },
  { firstname: "Jack", lastname: "White" }
];

// - Find all customers whose firstname starts with 'J'
let CustJ = function(cust) {
  return cust.firstname.startsWith("J")
}
let nameWithJ = customers.filter(CustJ);
console.log(nameWithJ);

// - Create new array with only first name
var firstNewName = customers[0].firstname
firstNewName.split()

// - Create new array with all the full names (ex: "Joe Blogs")
let createFullName = function(customer) {
  return `${customer.firstname} ${customer.lastname}`;
}
let fullNames = customers.map(createFullName);


// - Sort the array created above alphabetically
fullNames.sort();


// - Create a new array that contains only user who has at least one vowel in the firstname.
```
