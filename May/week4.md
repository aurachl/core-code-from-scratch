<h1 align="center">Ⓜ️ May Ⓜ️</h1>

## _(Monday) May 02_ 📢

`Learning about:` 💡
* **for of**
> The `for of` statement creates a loop iterating over iiterable data structures such as `Arrays, Strings, Maps, NodeLists`, and more.

> Example
```javascript
const cars = ['Toyota', 'BMW', 'Honda'];
  for (let x of cars) {
    console.log(x);
}
```
>Output
```ruby
"Toyota"
"BMW"
"Honda"
```

* **Array Filter**
> The `array filter` method creates a new array filled with elements that pass a `test` provided by a `function`.

> Example
```javascript
const numbers = [1, -8, 12, -34, -50, 5, 12]

const filters = numbers.filter(value => value >= 0);

console.log(filters);
```
>Output
```ruby
[1, 12, 5, 12]
```

* **Array Reduce**
> The `array reduce` method executes a `reducer function` for the array elements returning a `single value`.

> Example
```javascript
const prices = [123, 55, 48, 22, 17, 5, 1]

const tot = prices.reduce(
  (accum,curr) => accum + curr);
  
console.log(tot);
```
>Output
```ruby
271
```

* **Array Map**
> The `array map` creates a new array from `calling a function` for `every array element`.

> Example
```javascript
const persons = [
  {firstname : "Juan", lastname: "Perez"},
  {firstname : "Isabel", lastname: "Lopez"},
  {firstname : "Marta", lastname: "Cuervo"}
];

function getFullName(item) {
  return [item.firstname,item.lastname].join(" ");
}

console.log(persons.map(getFullName));
```
>Output
```ruby
["Juan Perez", "Isabel Lopez", "Marta Cuervo"]
```


## _(Tuesday) May 03_ 📢

`Learning about:` 💡
* **Regular Expressions (RegEx) Video & MDN Documentation**
> The `Regular Expressions` are tools used to `find patterns` within text, regularlly used to `validate` text and `search` through text. Uses elements like `search patterns` and `flags`.

> Example
```javascript
let text = "ABCDEFGHIJK";
let n = text.search(/E/i);
console.log(n);
```
>Output
```ruby
4
```

* **Regexr Tool**
> `RegExr.com` is an online tool to `learn, build, & test` Regular Expressions. Supports `JavaScript & PHP/PCRE RegEx` giving `results` update `in real-time` as you type and `validating patterns` with suites of `tests`.

> Expression
```ruby
//RegEx
\b[\w\.-]+@[\w\.-]+\.\w{2,4}\b
```
>Tests
```ruby
aura@gmail.com ✅
auragmail.com ❌
juan@hotmail.com ✅
```

* **String Replace & MDN Documentation**
> The `String Replace` method returns a new string with `some or all matches` of a `pattern replaced` by a `replacement`. The pattern can be a `string` or a `RegExp`, and the replacement can be a `string` or a `function called` for each match.

> Example
```javascript
let str = 'A red car goes around the red house with a red mail box.';
let newstr = str.replace(/red/g, 'blue');

console.log(newstr); 
```
>Output
```ruby
"A blue car goes around the blue house with a blue mail box."
```

## _(Wednesday) May 04_ 📢

>### Simple Validation Of A Username `Exercise` 🛃
```javascript 
function validateUsr(username) {
  const rules = /^[a-z0-9_]{4,16}$/;
  return rules.test(username); 
}
```

>### Get Number From String `Exercise` 🔢
**Using String Methods** 🔗
```javascript 
function getNumberFromString(s) {
  return Number(s
  .match(/\d/g)
  .join(''));
} 
```
**Using Array Methods** 📅
```javascript 
function getNumberFromString(s) {
  return Number(s
  .split('')
  .filter(number => number <= '9' && number >= '0')
  .join(''));
}
```

## _(Thursday) May 05_ 📢

>### String Cleaning `Exercise` ♻️
```javascript 
function stringClean(s){
  return s.replace(/[0-9]/g,''); 
}
```

>### Password Validation `Exercise` 🔐
```javascript 
function validate(password) {
  const rules = /^(?=.*[a-z])(?=.*[A-Z])(?=.*\d)[a-zA-Z0-9]{6,}$/;
  return rules.test(password);
}
```

## [📎 Back to main page !📎](/home/readAura.md)
