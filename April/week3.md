<h1 align="center">🅰️ April 🅰️</h1>

## _(Tuesday) April 19_ 📢

>### Multiply `Exercise` ❌
```javascript
function multiply (a, b) {
 return a * b;
}
```
>### ASCII Total `Exercise` ⏪
```javascript
function uniTotal (string) {
  let total = 0;
      for(let i = 0; i < string.length; i++) 
      {
          for ( let j=0; j < string[i].length; j++ ) 
          {
            let char_code = string[i].charCodeAt(j);
            total += char_code;
          }
      }
  return total;
} 
```

>### Char From ASCII Value `Exercise` ⏩
```javascript
function getChar(num) {
  return String.fromCharCode(num);
}
```
 
>### Binary Addition `Exercise` 1️⃣0️⃣0️⃣0️⃣1️⃣0️⃣
```javascript
function addBinary(a,b) {
  return (a+b).toString(2)
}
```

>### Student's Final Grade `Exercise` 💯
```javascript
function finalGrade (exam, projects) {
  if (exam > 90 || projects > 10) return 100;
  if (exam > 75 && projects >= 5) return 90;
  if (exam > 50 && projects >= 2) return 75;
  return 0; 
}
```

## _(Wednesday) April 20_ 📢

>### Holiday VIII - Duty Free `Exercise` 🍹
```javascript
function dutyFree(normPrice, discount, hol) 
    let dutyFree= (hol/(normPrice*(discount/100)));
    return Math.trunc(dutyFree);
    }
```

>### Twice As Old `Exercise` 👨👦👴
```javascript
function twiceAsOld(dadYearsOld, sonYearsOld) {
    return Math.abs(dadYearsOld-(sonYearsOld*2));
  }
```

>### Valid Spacing `Exercise` 🔍
```javascript
function validSpacing(s) {
  let spaceRegex = /\s/gi;
  let wordRegex = /[a-z]+/gi;
    if (s.match(spaceRegex) == null || s.length == 0) {
      return true; } 
        else if (s.match(wordRegex) == null) {
          return false; } 
        else if (s.match(spaceRegex).length == s.match(wordRegex).length - 1) {
          return true; }
    return false;
}
```
>#### `A cooler one that I find using ternary operator` 🔎
```javascript
function validSpacing(s) {
  return s=='' ? true : s.split(' ').find(el=> el=='') >= 0 ? false : true
}
```

>### Fake Binary `Exercise` 👻1️0️⃣👻0️⃣1️⃣👻
```javascript
function fakeBin(x) {
  let result = '';
    for (let i = 0; i < x.length; i++) {
      if (parseInt(x[i]) < 5) {
        result += '0'; }
      else {
        result += '1'; }
    }
  return result;
}
```

## _(Thursday) April 21_ 📢

>### Remove All Exclamation Marks From The End Of Sentence `Exercise` ‼️‼️
```javascript
function remove (string) {  
  return string.replace(/!+$/,"");
    }
```

>### Vowel Remover `Exercise` 🔠
```javascript
function shortcut (string) {
  let newstring = string.replace(/[aeiou]/gi,'');
  return newstring;
}
```

>### Rock Paper Scissors! `Exercise` 🗿📄✂️
```javascript
const rps = (p1, p2) => {
  
    if (p1 === p2) 
      return 'Draw!';
    if (p1 === 'rock' && p2 === 'scissors') 
      return 'Player 1 won!';
    if (p1 === 'scissors' && p2 === 'paper') 
      return 'Player 1 won!';
    if (p1 === 'paper' && p2 === 'rock') 
      return 'Player 1 won!';
  
    return 'Player 2 won!';
  }
```

>### Persistent Bugger `Exercise` 🍔
```javascript
function persistence(num) {
  let digits = num.toString();
  let result = 0;
  
  while (digits.length > 1) {
   digits = digits.split('').map(Number).reduce((a, b) => a * b).toString();
   result++;
  }
  
  return result;
}
```

## [📎 Back to main page !📎](/home/readAura.md)
