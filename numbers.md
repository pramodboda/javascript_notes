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

### `Number` Methods

- The global method **Number()** can convert string to `numbers`.
- Empty `strings` convert to `0` Zero.
- Anything else converts to `NaN` (Not a Number). 

**Converting Variables to Numbers**
**Global Number Methods**
- There are 3 JavaScript methods that can be used to convert `variables` to `numbers`.
- These methods are not only `number` methods, but also `global` JavaScript methods.
- JavaScript `global` methods can be used on all JavaScript `data types`.


| Method | Description |
| ------ | ------- |
| `Number()` | returns a `number`, converted from its arguments. |
| `parseFloat()` | Parses its argument and returns a `floating point number` |
| `parseInt()` | Parses its argument and returns an `integer`|

### Other  `Number` Methods
| Method | Description |
| ------ | ------- |
| `isFinite()` | Checks whether a value is a `finite number` |
| `isInteger()` | Checks whether a value is an `integer` |
| `isNaN()` | Checks whether a value is Number.NaN |
| `isSafeInteger()` | Checks whether a value is a safe integer |

### The `Number()` Method
```javascript
 // Converting any data type to Number
 Number(true);
 // returns 1
 Number(false);
 // reutrns 0
 Number(" ")
 // returns 0  
 Number("")
 // returns 0
 Number("1.43")
 // returns 1.43
 Number("143")
 // returns 143
 Number(" 143")
 // returns 143
 Number("143 ")
 // returns 143
 Number("545 454")
 // returns NaN
 Number("Pramod")
 // returns NaN
 Number("1234567890!@#$%^&*()");
 // returns NaN
```
> If the `number` cannot be converted, NaN (Not a Number) is returned.

### The `Number()` method used on `Dates`
- **Number()** can also convert a `Date` to a `Number`
```javascript
 Number(new Date("2018-06-08"))
 // returns 1528416000000
```
> The **Number()** method above returns the number of milliseconds since 1.1.1970.

### The `parseFloat()` Method
- **parseFloat()** parses a string and returns a number.
- Spaces are allowed.
- Only the first number is returned.
```javascript
 parseFloat("143");
 // 143
 parseFloat("1.43");
 // 1.43
 parseFloat("14.3");
 // 14.3
 parseFloat("1 4 3");
 // 1
 parseFloat("143 years");
 // 143
 parseFloat("years 143");
 // NaN
 parseFloat("years" 143);
 // NaN
 parseFloat("Pramod Boda");
 // NaN
 parseFloat(true);
 // NaN
 parseFloat(false);
 // NaN
```
> If the `number` cannot be converted, NaN (Not a Number) is returned.

### The `parseInt()` Method
- **parseInt()** parses a string and returns a whole number.
- Spaces are allowed.
- Only the first number is returned.
```javascript
 parseInt("143"); 
 // 143
 parseInt("1.43"); 
 // 1
 parseInt("14.3"); 
 // 14
 parseInt("1 4 3"); 
 // 1
 parseInt("143 years"); 
 // 143
 parseInt("years 143"); 
 // NaN
 parseInt("years", 143); 
 // NaN
 parseInt("Pramod Boda");
 // NaN
 parseInt(true);
 // NaN
 parseInt(false);
 // NaN
```
> If the `number` cannot be converted, NaN (Not a Number) is returned.


### Number Properties

| Property | Description |
| --------- | -------- |
| `MAX_VALUE` | Returns the `largest number` possible in JavaScript |
| `MIN_VALUE` | Returns the `smallest number` possible in JavaScript |
| `NEGATIVE_INFINITY` | Represents a `nagative infinity` (returned on overflow) |
| `NaN` | Represents a `"Not-a-Number"` value |
| `POSITIVE_INFINITY` | Represents `infinity` (returned on overflow) |
| `constructor` | returns a function that created JavaScript's `Number property`  |
| `prototype` | Allows you to add `properties` and `methods` to an `object`. |

**Always use correct syntax**
```javascript
 var a = Number.MAX_VALUE;
 console.log(a); // Return Value: A Number, 1.7976931348623157e+308
 
 var b = Number.MIN_VALUE;
 console.log(b); // Return Value: A Number, 5e-324
 
 Number.NEGATIVE_INFINITY // -Infinity
 
 Number.NaN // NaN
 
 Number.POSITIVE_INFINITY // Infinity
 
```


### The `MAX_VALUE` Property

- The **`Number.MAX_VALUE`** property represents the maximum numeric value representable in JavaScript.
- This static property has a value of `1.7976931348623157e+308`.
- `MAX_VALUE` is a static property of the JavaScript Number object. You can only use it as `Number.MAX_VALUE`.

```javascript
 var x = 143;  
 x.MAX_VALUE;
 console.log(x); // returns 'undefined'.
```
- Using `x.Max_VALUE`, where `x` is a number or a Number object, will return `undefined`

> Note: `Numbers` larger than MAX_VALUE are represented as `infinity`. 

```javascript
 function multiply(x, y) {
  if (x * y > Number.MAX_VALUE) {
    return ("Process as Infinity");
  }
  return (x * y);
 }
 console.log(multiply(1.7976931348623157e+308, 1));
 // expected output: 1.7976931348623157e+308

 console.log(multiply(1.7976931348623157e+308, 2));
 // expected output: "Process as Infinity"
```

### The `MIN_VALUE` Property

- The **`Number.MIN_VALUE`** property represents the smallest positive numeric value re-presentable in JavaScript.
- The `MIN_VALUE` property is the number closest to 0
- `MIN_VALUE` has a value of approximately `5e-324`. 
- Values smaller than `MIN_VALUE` ("underflow values") are converted to 0.
- Because `MIN_VALUE` is a static property of `Number`, you always use it as `Number.MIN_VALUE`, rather than as a property of a `Number` object you created.

- `MIN_VALUE`  is a static property of the JavaScript Number object. You can only use it as  `Number.MIN_VALUE`.
```javascript
 var x = 143;  
 x.MIN_VALUE;
 console.log(x); // returns 'undefined'.
```
- Using `x.MIN_VALUE`, where `x` is a `number` or a `Number object`, will return `undefined`
> Note: `Numbers` smaller than MIN_VALUE are converted as `0`. 
```javascript
 function multiply(x, y) {
  if (x * y < Number.MIN_VALUE) {
    return "Process as -Infinity";
  }
  return (x * y);
 }
 console.log(multiply(5e-324, 1));
 // expected output: 5e-324
 
 console.log(multiply(-1.7976931348623157e+308, 2));
 // expected output: Process as -Infinity
```


### The `NEGATIVE_INFINITY` Property
```javascript
 function func() {
   console.log(Number.NEGATIVE_INFINITY);
 }
 func();
 // => -Infinity
```
```javascript
 function func() {
    var n = (-Number.MAX_VALUE) * 2;
    console.log(n);
 }
 func();
 // => -Infinity
```

### The `NaN` Property
- The `NaN` property represents "Not-a-Number" value.
- This property indicates that a value is not a legal number.
- The `NaN` property is the same as the `Number.NaN` property.

> Tip: Use the isNaN(). global function to check if a value is a NaN value.
 
```javascript
 var a = 4564;
 isNaN(a);
 // => False
 
 var a = "dkjfg.87dsm";
 isNaN(a);
 // => true
```

### The `POSITIVE_INFINITY` Property
- The `POSITIVE_INFINITY` property represents positive infinity `(+infinity)`
- Positive infinity can be explained as something that is higher than any other number.
- `POSITIVE_INFINITY` is a static property of the JavaScript Number object.
```javascript
 var a = 143;  
 a.POSITIVE_INFINITY;
 // => undefined
```
- Using `a.POSITIVE_INFINITY`, where `a` is a `number` or a `Number object`, will return `undefined`.
- You will be using it as  `Number.POSITIVE_INFINITY`.
```javascript
 98754604586/0
 // => Infinity
```
```javascript
 function foo() {
   console.log(Number.POSITIVE_INFINITY);
 }
 foo();
 // => Infinity
```
```javascript
 function foo() {
    var n = (Number.MAX_VALUE) * 2;
    console.log(n);
 }
 foo();
 // => Infinity
```
### The `constructor` Property
- All `objects` produced by built-in `construction functions` in JavaScript have a property called `constructor`.
- In JavaScript, the `constructor` property returns the `constructor function` for an `object`.
- The return value is a reference to the `function`, not the name of the function
- For JavaScript `numbers` the `constructor` property returns `function Number(){[native code]}`
- For JavaScript `strings` the `constructor` property returns `function String(){[native code]}`
- For JavaScript `booleans` the `constructor` property returns `function Boolean(){[native code]}`
```javascript
 new String("abc").constructor === String
 // => true
```

### The `prototype` Property
- The `prototype` property allows you to add properties and methods to an `object`.
- When constructing a `property`, All `numbers` will be given the `property`, and its `value`, as default.
- When constructing a `method`, All `numbers` will have this `method` available. 

> `Number.prototype` does not refer to a single number `object`, but to the `Number()` object itself.

> `Prototype` is a `global object constructor` which is available for all JavaScript `objects`.
<!--stackedit_data:
eyJoaXN0b3J5IjpbMTgxNjY3Nzg1Nl19
-->