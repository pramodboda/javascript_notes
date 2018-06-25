
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
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTExNjkzNzUxOTQsMjAyMDMyNjY5NF19
-->