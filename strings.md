
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

Strings can be created from other types using `String()` function

```javascript
 var intString = String(143);
 // "143"
 
 var booleanString = String(true);
 // "true"
 
 var objString = String({})
 // "[object Object]"
 
 var nullString = String(null);
 // "null"
```
Or, you can also create or convert Numbers, Booleans, or Objects to Strings by using `toString()` function, But it will not convert `null`, `undefined`, `String`.
```javascript
 var floatString = (242.1657).toString();
 // "242.1657"
 
 var booleanString = (false).toString();
 // "false"

 var objString = ({}).toString();
 // "[object Object]"

 var nullString = (null).toString();
 // Error : will not convert to string
 
 var undefinedString = (undefined).toString();
 // Error : will not convert to string
```


### String Methods

| Methods | Description |
| -------- | ------------- |
| `charAt()` | Return the character at the specified index(position). |
| `charCodeAt()` | Returns the Unicode of the character at the specified index. |
| `concat()` | Joins two or more strings, and returns a new joined strings. |
| `endsWith()` | Checks whether a string ends with specified string/ characters |
| `fromCharCode()` | Converts Unicode values to characters.  |
| `includes()` | Checks whether a string contains the specified string/characters. |
| `indexOf()` | Returns the position of the first found occurrence of a specified value in a string. |
| `lastIndexOf()` | Returns the position of the last found occurrence of a specified value in a string. |
| `localeCompare()` | Compares two strings in the current locate |
| `match()` | Searches a string for a match against a regular expression, and returns the matches. |
| `repeat()` | Returns a new string with a specified number of copies of an existing string. |
| `replace()` | Searches a string for a specified value, or a regular expression, and returns a new string where the specified values are replaced. |
| `search()` | Searches a string for a specified value, or a regular expression. |
| `slice()` | Extracts a part of a string and returns a new string. |
| `split()` | Splits a string into an array of substrings. |
| `startsWith()` | Checks whether a string begins with specified characters. |
| `substr()` | Extracts the characters from a string, beginning at a specified start position, and through the specified number of character. |

| `toString()` | returns a `number` as a `string`. |
| `toExponential()` | returns a `string`, with `number` rounded and written using exponential notation. |
| `toFixed()` |returns a `string`, with the `number` written with a specified number of decimals.|
| `toPrecision()` | returns a `string`, with a `number` written with a specified length |
| `valueOf()` | returns a *number* as a `Number`, returns a *string* as a `String` |
```javascript
var x = 140;
x.toString(); // returns "140"
(x+3).toString(); // returns "143"
(140+3).toString(); // returns "143"
```
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTg1ODE3MjI2NCwyMDIwMzI2Njk0XX0=
-->