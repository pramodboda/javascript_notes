JavaScript Notes
=
<a id="toc"></a>
## About Pramod Boda
**Artist** | **UI Designer and Developer** | **Motion Graphic Designer**


## Steps to achieve JS
- Complete in-depth learning basics and advanced concepts on JavaScript with practical.
- Think, plan and work on small JavaScript projects, list them and complete one by one.
- Gather all completed projects and add into one huge web application project.
- Start Learning JS Frameworks.

## Basics to cutting edge techniques
- JavaScript Complete Guide
- JavaScript by Example
- JavaScript and JSON Essentials
- Mastering JavaScript Functional Programming
- Object-Oriented Programming with JavaScript
- Data Structures in JavaScript
- Learning JavaScript Data Structures and Algorithms
- The Complete JavaScript Developer - MEAN stack zero-to- hero
- Grunt.JS : Automate web development tasks and save your time.
- Machine Learning with JavaScript 
- Augmented Reality for JavaScript Developers


## Index
1. [Introduction](#jsIntroduction)
2. [Lexical Structure](#jsLexicalStructure)
3. [Variables](#jsVariables) 
4. [Data Types](#jsDataTypes)
6. [Operators](#jsOperators)

<a id="jsIntroduction"></a>
## Introduction
### What is JavaScript?
- JavaScript is the Programming language of the **Web**
- JavaScript is part of the triad of technologies that all developers must learn

Language  |  Role  |  Description
------  |  ---------  | ----------
HTML  | Content  |  to specify the content of the web pages.
CSS  |  Presentation  |  to specify the presentation of the web pages.
JS  |  Behavior  |  to specify the behavior of the web pages.

- JavaScript is a high-level programming language.
- JavaScript is a case-sensitive language.
	- This means that language `keywords`, `variables`, `function` names, and other `identifiers` must always be typed with a consistent capitalization of letters.

		```javascript
		 var name = "Pramod Boda"; //initiated variable 'name'
		 Name; // will not be same as 'name'
		 NAME; // will not be same as 'name'
		 name; => "Pramod Boda"
		```

- All web browsers support it without the need for plug-ind by means of a built-in JavaScript engine.
- JavaScript is used on desktops, games consoles, tablets, and smart phones.
- Including JavaScript interpreters, making JavaScript the most ubiquitous programming language in history.
- JavaScript well-suited to object-oriented and functional programming style.
- The overwhelming majority of modern websites use JavaScript, and all web browsers.
- JavaScript has long since out grown its scripting - language roots to become a robust and efficient general - purpose language.

[<img src="images/toc.png" width="24" height="24" style="float: right;"/>](#toc)

<a id="jsLexicalStructure"></a>
## Lexical Structure

- The lexical structure of a programming language is the set of elementary rules that specifies how you write programs in that language.

### Character Set
- JavaScript programs are writing using the Unicode character set.
- Unicode is a superset of ASCII and Latin-1 and supports virtually every written language currently used on the planet.

### Case sensitivity
- JavaScript is a case-sensitive language. This means that language `keywords`, `variables`, `function` names, and other `identifies` must always be typed with consistent capitalization of letters.
```javascript
 var name = "Pramod Boda"; //initiated variable 'name'
 Name; // will not be same as 'name'
 NAME; // will not be same as 'name'
 name; => "Pramod Boda"
```

> Note: however, thet HTML is not case-sensitive(althought XHTML is).

- Many client-side JavaScript objects and properties have the same names as the HTML tags and attributes they represent. 
- While these tags and attributes names can be typed in any case in HTML, In JavaScript they typically must be all lowercase.

> The HTML onclick event handler attribute is sometimes specified as onClick in HTML, but it must be specified as onclick in JavaScript code(or in XHTML documents).

### Comments
- JavaScript supports two style of comments.
- Any text between a // and the end of a line is treated as a comment. and is ignored by JavaScript.
- Single comment example:
```javascript
 // This is a Single line comment.
```

- Any text between the characters /* and */ is also treated as a comment; These comments may span mutiple lines but may not be nested.
- Multi-Line comment example:
```javascript
 /* 
 * This is a
 * Multiple lines
 * comment.
 */
```

### Literals 

- A literals is a data that appears directly in a program.
```javascript
 46 // The Number forty six.
 4.6 // The Number four point six.
 "Hylo World" // A String of text.
 'Hi' // Another String.
 true // A Boolean value.
 false // another Booleans value.
 /javascript/gi // A regular expression literal (for pattern matching)
 null // Absence of object.
```

```javascript
 x:3, y:5 // An object initializer
 [1,2,3,a,b,c,4,5] // An array initializer.
```

### Identifiers
- An identifires is simple a name. In JavaScript, identifires are used to name variables and functions and to provide labels for certain loops in JavaScript code.
- These are all legal identifiers: 
```javascript
 var trueVar // variable initialization
 my_variable_name() // function name
 var v143 // variable initialization
 _trueVariable() // function name
 var $strVariable // variable initialization
```

#### Mathematical symbols
```javascript
 var si = true;
 var π = 3.14;
```

### Reserved Words

- You cannot use these words as `identifiers` in your programs.

| * | * | * | * | * |
| -------- | ----- | ----- | ----- | ----- |
| `break` | `delete` | `function` | `return` | `typeof` |
| `case` | `do` | `if` | `switch` | `var` |
| `catch` | `else` | `in`  | `this` | `void` |
| `continue` | `false` | `instanceof` | `throw` | `while` |
| `debugger` | `finally` | `new` | `true` | `with` |
| `default` | `for` | `null` | `try` |  |

**Non-reserved words that act like reserved words**
- The `NaN`, `Infinity`, `undefined` properties of the global ogject are immutable or read-only properties in ES5. So even though `var NaN = 42;` in the global scope wouldn't throw an error, it wouldn't actually do anything
- To avoid confusion, I'd suggest you to avoiding the use of these `variable` names.
```javascript
 //In the global scope
 var NaN = 42;
 console.log(NaN); // NaN
 
 //...but elsewhere
 (function(){
	 var NaN = 42;
	 console.log(NaN); // 42
 }());
```

### Dynamic Typing
JavaScript is a loosely typed or a dynamic language.

[<img src="images/toc.png" width="24" height="24" style="float: right;"/>](#toc)
<a id="jsVariables"></a>
## Variables
**Defining a variable**
```javascript
 var myVariable = "This is a variable!";
```
- This `variable` is called a `string` because it has ASCII characters(a-z, A-Z, 0-9, !@#$%^&*()?|\/)

**Using a variable**
```javascript
 var num = 140; // Variable initialization.
```
**Calling or using a variable**
```javascript
 num; // Calling a variable.
 sum = 3 + num; // Using a variable, addition the expression and initalizing into 'sum' variable.
```
[<img src="images/toc.png" width="24" height="24" style="float: right;"/>](#toc)
<a id="jsDataTypes"></a>
## Data Types
The latest ECMAScript standard defines seven data types in JavaScript:
- Six data types that are primitives:
  - `Number`
  - `String`
  - `Boolean`
  - `Undefined`
  - `Null`
  - `Symbol` (new in ECMAScript 2015) 
- `object` are the most complex data type
	- `Array`
	- `Date`
	- `Function` 
	- `RegExp`

```javascript
 typeof 143
 => "number"
```
```javascript
 typeof "Pramod"
 => "string"
```
```javascript
 typeof true
 => "boolean"
```
```javascript
 typeof undefined
 => "undefined"
```
```javascript
 typeof null
 => "object"
```
```javascript
 typeof []
 => "object"
```
```javascript
 typeof {}
 => "object"
```
```javascript
 typeof NaN
 => "number"
```
## Numbers
- A *number* type serves both for integer and floating point numbers.
- When a *number* appears directly in a JavaScript program, it's called a *Numeric literals*.
- JavaScript supports numeric literals in several  formats.
```javascript
 6
 4
 54613244
``` 
### Types of Numbers
```javascript
 var jsInteger = 16; // 32-bit number (from -2,147,483,648 to 2,147,483,647)
 var jsLong = 96542464354564345; // 64-bit number (from -9,223,372,036,854,775,808 to 9,223,372,036,854,775,807)
 var jsFloat = 2.6; // 32-bit floating-point number (decimal)
 var jsDouble = 3545435745.56454; // 64-bit floating-point number
```
-  Besides regular numbers, there are other values so-called "special numeric values" which  also belong to that type: `Infinity`, `-Infinity`, and `NaN`.
- #### What happens when you divide by zero in JavaScript?
	 ```javascript
      3564554/0 //=> ??
      143/ +0 //=> ??
      143/ -0 //=> ??
	```
[Read more about Numbers](https://github.com/pramodkumarboda/javascript_notes/blob/master/numbers.md)

## Strings
```javascript
var myString = "This is a string text."
```
#### Concatenation
We can also add strings which will concatenate them, or put them together.
```javascript
 var myStringConcatenate = "This is "+"a string text." // This is a string text.

 var firstName = "Pramod";
 var lastName = "Boda";
 console.log(firstName + lastName); // PramodBoda
 console.log(firstName+ " " +lastName); // Pramod Boda


 firstName.concat(lastName) // "PramodBoda"

 var nickName = "Pro";
 (firstName+" "+lastName).concat("("+nickName+")") // "Pramod Boda(Pro)"
```

#### String interpolation
- JavaScript allows multi-line strings also. 
```javascript
console.log(`I am string statement first line
I am string statement second line
I am string statement third line `);

output:
I am string statement first line
I am string statement second line
I am string statement third line
```
- This kind of string is also known as template string can be use for string interpolation.

- JavaScript allows Python-like string interpolation using this syntax.
```javascript
 var a=10, b=20;
 
 console.log("Sum of  value is: "+ (a+b) +" and multiplication is: " + (a*b));
 
 Output:
 Sum of  value is: 30 and multiplication is: 200
```
- However, with string interpolation, things become a bit clearer:
```javascript
 var a=10, b=20;
 
 console.log(`Sum of  value is :${a+b}
 multiplication is: ${a*b}`);
 
 output:
 Sum of value is: 30
 multiplication is: 200
```

[Read more about Strings](https://github.com/pramodkumarboda/javascript_notes/blob/master/strings.md)



## Boolean
- A `boolean` value represents truth or falsehood.
	- On | Off
	- Yes | No
	- True | False
- There are only two possible values of this type, we called as `true` and `false` .
- Those are reserved keywords for JavaScript.
- `true` and `false` values are generally the result of comparisons you make in your JavaScript programs. 

```javascript
var myBoolean = true;
var myBoolean2 = false;
```
- _Comparison_ and _Logical_ operators(will be discussed in [operators](#) section) are used to test for `true` or `false`.
## Null
- The special `null` value does not belong to any type of those described above.
- It forms a separate type of its own, which contains only the `null` value:
```javascript
 var casteStatus= null;
 ```
- It's just a special value which had the sense of "nothing", "empty" or "value unknown".
- The code above states that the `casteStatus` is unknown or empty for some reason. 
- `null` is a language keyword that evaluates to a special value that is usually used to indicate the absence of any `object` value.
- It is one of JavaScript's primitive values.
- `null` is one of the standard built-in `object`.
- The value `null` is written with a literal: `null`
- In JavaScript `null` is not a "reference to non-existing object" or a "null pointer" like in some other languages.

```javascript
 function getVowels(str){
	 var p = str.match(/[aeiou]/gi);
	 if(m === null){
		 return 0;
	 }
	 return p.lenght;
 }
 console.log(getVowels('sky'));
 // expected output: 0
 // observe how null is used above getVowels(str) function.
```


## Undefined
- The special value `undefined` stands apart. its makes a type of its own just like `null`.
- The meaning of `undefined` is "value is not assigned".
- If a `variable` is declared, but not assigned, then its value if exactly `undefined`:
```javascript
 var x;
 console.log(x); // shows "undefined"
``` 
- Technically, it is possible to assign `undefined` to any variable: 
```javascript
 var x = 143;
 x = undefined;
 console.log(x);// "undefined"
```
- But it's not recommended to do that. Normally, we use `null` to write an "empty" or an "unknown" value into the variable
- `undefined` is only used for checks, to see if the variable is assigned or similar.
- `undefined` is a property of the _global object_; i.e., it is a variable in global scope, that means `undefined` is a predefined `global variable` that is initialized to the `undefined` value.
- `undefined` is not a language keyword like `null`.
- The initial value of `undefined` is the primitive value `undeifned`.
- The `undefined` value represents a deeper kind of absence of a value.
- It is the `value` of the variables that have not been initialized and the `value` you get when you query the value of an `object` property or an `array` element that does not exist, is know as `undefined`.
- The `undefined` value is also returned by 	`functions`  that have no return value, and the value of `function` parameters for which no argument is supplied.
```javascript
 var value =  (function(){})();  // returns undefined
 (function(undefined){  // parameter is undefined  })();
```
- in **ECMAScript 3**, `undefined` is a read/ write variable, and it can be set to any value. This error is corrected in **ECMAScript 5** and `undefined` is read-only in that version of the language.
- If you apply the `typeof` operator to the `undefined` value, it returns `"undefined"`, indicating that this value is the sole member of a special type.

**Strict equality and `undefined`**
```javascript
 function testIsUndefined(t){
	if(t === undefined){
		return "This is a undefined value!";
	}
	else{
		return "It has a value!";
	}
	return t;
 }
 
 var x;
 console.log(testIsUndefined(x));
 // expected output: "This is a undefined value!"
```

**`typeof` operator and `undefined`**
Alternatively, `typeof` can be used:
```javascript
 function testIsUndefined(t){
	if(typeof t === "undefined"){
		return "This is a undefined value!";
	}
	else{
		return "It has a value!";
	}
	return t;
 }
 
 var x;
 console.log(testIsUndefined(x));
 // expected output: "This is a undefined value!"
```
one reason to use `typeof` is that it does not throw an error if the `variable` has not been declared.
```javascript
 //x has not been declared before
 if(typeof x == 'undefined'){
	//evalutes to true without errors
	//these statements executes
 }

 if(x === undefined){
	//throws a ReferenceError
 }
```
However, this kind of technique should be avoided.
**`void` operator and `undefined`**
The `void` operator is a third alternative.
```javascript
 var x;
 if(x === void 0){
  // these statements execute
 }
// y has not been declared before
if(y === void 0){
 // throws a  - Uncaught ReferenceError: y is not defined.
}
```
```javascript
 var array =  [1,  2,  3];
 var foo = array.foo;  // foo property doesn't exist, returns undefined
 var item = array[5];  // no item exists in the array at index 5, returns undefined
```
## Difference between `null` and `undefined`
```javascript
 typeof null // "object" (not "null" for legacy reasons)
 
 typeof undefined		// "undefined"
 
 null === undefined		// false
 
 null == undefined		// true
 
 !null					// true
 
 isNaN(6 + null)		// false 
 // Because
 6 + null // is 6, 6 is a number
 
 isNaN(6 + undefined)	// true
 // Because
 6 + undefined // will be NaN 

 Object.prototype.toString.call(null);  // [object Null]
 Object.prototype.toString.call(undefined);  // [object Undefined]
 
```
- From the preceding examples, it is clear that `undefined` and `null` are two distinct types: `undefined`is a type itself (undefined) while `null` is an object. 
## Object
- The `object` type is a special type.
- The `object` constructor creates an `object` wrapper for the given value.

### Getting object type by constructor name
**String**
```javascript
 Object.prototype.toString.call("String");
 //=> "[object String]"
```
**Number**
```javascript
 Object.prototype.toString.call(143);
 //=> "[object Number]"
```
**Boolean**
```javascript
 Object.prototype.toString.call(true);
 //=> "[object Boolean]"
```
**Object**
```javascript
 Object.prototype.toString.call(Object());
 //=>"[object Object]"

 Obect.prototype.toString.call({});
 //=> "[object Object]"
```
**Function**
```javascript
 Object.prototype.toString.call(function(){});
 //=> "[object Function]"
```
**Date**
```javascript
 Object.prototype.toString.call(new Date(2018,06,22));
 //=> "[object Date]"
```
**Regex**
```javascript
 Object.prototype.toString.call(new RegExp());
 //=> "[object RegExp]"

 Object.prototype.toString.call(/foo/);
```
**Array**
```javascript
 Object.prototype.toString.call([]);
 // => "[object Array]"
```
**Null**
```javascript
 Object.prototype.toString.call(null);
 // => "[object Null]"
```

**Undefined**
```javascript
 Object.prototype.toString.call(undefined);
 // => "[object Undefined]"
```
**Error**
```javascript
 Object.prototype.toString.call(Error());
 // => "[object Error]"
```

### Best ways to check for each type
```javascript
 var foo;

 typeof foo == 'undefined'
 =>true

 isNaN(foo);
 =>true

 foo === undefined
 =>true
```
```javascript
 var a = 4564;
 isNaN(a);
 // => False
 
 var a = "dkjfg.87dsm";
 isNaN(a);
 // => true
```

[<img src="images/toc.png" width="24" height="24" style="float: right;"/>](#toc)

<a id="jsOperators"></a>
## Operators

- JavaScript has following types of operators: 
	- [Assignment operators](#)
	-  [Comparison operators](#)
	- [Logical operators](#)
	-  [Arithmetic operators](#)
	- [Bitwise operators](#)
	- [String operators](#)
	- [Conditional (ternary) operator](#)
	- [Comma operator](#)
	-  [Unary operators](#)
	- [Relational operators](#)
### Assignment Operators
- Assignment operators are used to assign values to JavaScript variables.

Assume `a=10` and `b=20`
Operator | Example | Same as | Output
------ | ------ | ------ | ------ 
`=` | `a=b` | `a=b` | `20`
`+=` | `a+=b` | `a=a+b` | `30`
`-=` | `a-=b` | `a=a-b` | `-10`
`*=` | `a*=b` | `a=a*b` | `200`
`/=` | `a/=b` | `a=a/b` | `0.5`
`%=` | `a%=b` | `a=a%b` | `10`
`<<=` | `a<<=b` | `a=a<<b` | `10485760`


### Comparison Operators
Assume `a=4`

Operator | Description | Comparing | Output
------ | ------ | ------ | ------ 
`==` | equal to | `a == 6` | `false`
`===` | equal and equal type | `a === 4` | `true`
`!=` | Not equal to | `a != 6` | `true`
`!==` | not equal value or not equal type | `a !== 6` | `true`
`>` | greater than | `a > 6` | `false`
`<` | less than | `a < 6` | `true`
`>=` | greater than or equal to | `a >= 4` | `true`
`<=` | less than or equal to | `a <= 4` | `true`
`?` | ternary operator | `(a<=3) ? "greater than or equal to 4":"less than or equal to 4"` | less than or equal to 4

### Conditional (Ternary) Operator
JavaScript also contains a conditional operator that assigns a value to a variable based on some condition.
#### Example
#### HTML:
```html
 <h3>Vote Eligible Check</h3>
 <input type="text" id="userAge">
 <div id="voteEligibleStatus"></div>
```
#### JS:
```javascript
 var userAge = document.getElementById('userAge');
 var voteEligibleStatus = document.getElementById('voteEligibleStatus');
 voteEligibleStatus.style.display =  "none";

 userAge.addEventListener("input", voteEligibleCheck,  false);
 
 function voteEligibleCheck()  {
	 var age = userAge.value;
	 if  (isNaN(age))  {
		 var ageEligibleStatus =  "Given input is not a number";
	 } else  {
		 // Conditional (Ternary) Operator
		 var ageEligibleStatus =  (age <  18)  ?  "not eligible"  :  "eligible";
		 }
	 voteEligibleStatus.innerHTML = ageEligibleStatus +  " to vote.";
	 voteEligibleStatus.style.display =  "block";
	 voteEligibleStatus.classList.add("alert-success");
	 if  (age ==  null  || age ==  "")  {
		 voteEligibleStatus.innerHTML =  " ";
		 voteEligibleStatus.style.display =  "none";
	 }
 }
```




### What will be the output and why?
```javascript
1>2>3 ==>??
3>2>1 ==>??
```

## Stay Tuned ...






