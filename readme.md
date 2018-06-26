JavaScript Notes
=
<a id="toc"></a>
## About Pramod Boda
**Artist** | **UI Designer and Developer** | **Motion Graphic Designer**



## Index
1. [Introduction](#jsIntroduction)
2. [Lexical Structure](#jsLexicalStructure)
4. [Variables](#jsVariables) 
5. [Data Types](#jsDataTypes)

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

## Undefined
## Null

## Object

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
## Operators
### What will be the output and why?
```javascript
1>2>3 ==>??
3>2>1 ==>??
```

## Stay Tuned ...






