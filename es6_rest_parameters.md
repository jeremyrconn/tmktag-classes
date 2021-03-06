# ES6 Using (...) 
# Rest Parameters and Spread Syntax

### Learning Objectives
- How to use the (...) operator in es6
- Differences between Rest Parameter and Spread Syntax
- Compare multiple argument function declarations in es5 & es6
- Compare calling functions with multiple arguments in es5 & es6


## Rest Parameters

### ES5 multiple argument function

```js
function display(company, name, age, title, sport){
	this.company = company;
	this.name = name;
  	this.age = age;
  	this.title = title; 
  	this.sport = sport || 'Baseball';
}

display('MLBAM', 'Jeremy', '40', 'Software Engineer', 'Hockey');

```

### ES6 multiple argument function

```js
function display(company, ...teamData){
	this.company = company;
	this.name = teamData[0];
  	this.age = teamData[1];
  	this.title = teamData[2]; 
  	this.sport = teamData[3] || 'Baseball';
}


display('MLBAM', 'Jeremy', '40', 'Software Engineer', 'Hockey');

```

<details>
<summary>(...) Operator</summary>

- When using `(...)` with a function declaration any following arguments when the function is called will be grouped into that `Rest Parameter` as an array. The rest parameter must always be the last argument in the function declaration.

- When you call a function and apply `(...)` to an object like an array it will assign the contents of the array to multiple variables in the order they appear in the array. This is `Spread Syntax`.

</details>

## Spread Syntax

### ES5 calling a function with multiple arguments from an array

```js
var person = ['Jeremy', '40', 'Software Engineer', 'Hockey'];
display('MLBAM', person[0], person[1], person[2], person[3])

```

### ES6 calling a function with multiple arguments from an array

```js
var person = ['Jeremy', '40', 'Software Engineer', 'Hockey'];
display('MLBAM', ...person)


```
---
# Turn and Talk

- What are some of the differences between the old syntax and the new?



