JavaScript Notes
=
## About Pramod Boda
**Artist** | **UI Designer and Developer** | **Motion Graphic Designer**


# Index
1. [Introduction](#introduction)
2. [Lexical Structure](#lexicalStructure)
3. [Data Types]()

<a id="introduction"></a>
# Introduction
## What is JavaScript?
- JavaScript is the Programming language of the **Web**
- JavaScript is part of the triad of technologies that all developers must learn

Language  |  Role  |  Description
------  |  ---------  | ----------
HTML  | Content  |  to specify the content of the web pages.
CSS  |  Presentation  |  to specify the presentation of the web pages.
JS  |  Behavior  |  to specify the behavior of the web pages.

- JavaScript is a high-level programming language.
- JavaScript is a case-sensitive language.
	- This means that language keywords, variables, function names, and other identifiers must always be typed with a consistent capitalization of letters.

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

<a id="lexicalStructure"></a>
## Lexical Structure

- The lexical structure of a programming language is the set of elementary rules that specifies how you write programs in that language.

### Character Set
- JavaScript programs are writing using the Unicode character set.
- unicode is a superset of ASCII and Latin-1 and supports virtually every written language currently used on the planet.

### Case Sencitivity
- JavaScript is a case-sensitive language. This means that language keywords, variables, funations names, and other identifies must always be typed with consistent capitalization of letters.
```javascript
var name = "Pramod Boda"; //initiated variable 'name'
Name; // will not be same as 'name'
NAME; // will not be same as 'name'
name; => "Pramod Boda"
```

> Note: however, thet HTML is not case-sensitive(althought XHTML is).

- Many client-side JavaScript objects and properties have the same names as the HTML tags and attributes they represent. 
- While these tags and attributes names can be typed in any case in HTML, In JavaScript they typically must be all lowercase.

> The HTML onclick event handler attribute is sometimes specified as onClick in HTML, but it must be specified as onclick in JavaScript code( or in XHTML documents).

### Comments
- JavaScript supports two style of comments.
- Any text between a // and the end of a line is treated as a comment. and is ignored by JavaScript.
- Single comment example:
-  ```javascript
		// This is a Single line comment.
	 ```

- Any text between the characters /* and */ is also treated as a comment; These comments may span mutiple lines but may not be nested.
- Multi-Line comment example:
-  ```javascript
		/* 
		* This is a
		* Multiple lines
		* comment.
		*/
	 ```





