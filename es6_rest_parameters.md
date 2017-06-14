# ES6 Rest Parameters

### Learning Objectives
- How to use the (...) operator in es6
- Compare multiple argument functions in es5 vs es6
- Proper implementation of rest parameters




### ES5 multiple argument function

```js
function display(groupNames, moreGroupNames){
	var sortedNames = [groupNames, moreGroupNames].sort();
	var div = document.getElementById('output');
  if (sortedNames.includes('Jeremy')){
  var teamName = 'BWS<br />';  
  } else {
  var teamName = 'That other team<br />';
  }
	div.innerHTML = div.innerHTML + teamName + sortedNames + '<br />';
}

display('Jeremy', 'Elan', 'Mat', 'Shojib', 'Bob', 'Stephen');
```

### ES6 multiple argument function

```js
function display(...groupNames){
	var sortedNames = groupNames.sort();
	var div = document.getElementById('output');
  if (sortedNames.includes('Jeremy')){
  	var teamName = 'BWS<br />';  
  } else {
  	var teamName = 'That other team<br />';
  }
	div.innerHTML = div.innerHTML + teamName + sortedNames + '<br />';
}

display('Jeremy', 'Elan', 'Mat', 'Shojib', 'Bob', 'Stephen');

```

---
# Turn and Talk

- What are some of the differences between the old syntax and the new?





# Exercise P2

- Using the new ES6 inheritance features, clean up the two constructors we just converted

