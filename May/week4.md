<h1 align="center">Ⓜ️ May Ⓜ️</h1>

## _(Monday) May 02_ 📢

`Learning about:` 💡
* **for of**
* **Array Filter**
* **Array Reduce**
* **Array Map**

## _(Tuesday) May 03_ 📢

`Learning about:` 💡
* **Regular Expressions (RegEx) & MDN documentation**
* **String Replace & MDN Documentation**
* **Regexr Tool**
* **More about RegEx**

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

```

>### Password Validation `Exercise` 🔐
```javascript 
function validate(password) {
  const rules = /^(?=.*[a-z])(?=.*[A-Z])(?=.*\d)[a-zA-Z0-9]{6,}$/;
  return rules.test(password);
}
```

## [📎 Back to main page !📎](/home/readAura.md)
