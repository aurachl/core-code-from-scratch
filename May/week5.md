<h1 align="center">Ⓜ️ May Ⓜ️</h1>

## _(Monday) May 09_ 📢

>### Find The Missing Letter `Exercise` 🔍
```javascript 
function findMissingLetter(array) {
  let string = array.join("");
    for (let i = 0; i < string.length; i++) {
      if (string.charCodeAt(i + 1) - string.charCodeAt(i) != 1) {
      return String.fromCharCode(string.charCodeAt(i) + 1);}
    }
}
```

>### Reverse Or Rotate? `Exercise`↩️
```javascript 
function revrot(str, sz) {
  if (sz <= 0 || str == '' || sz > str.length) {
    return ''; }
    const arr = [];
    const s = str.split('');
  while (s.length >= sz) {
    arr.push(s.splice(0, sz));}
    const res = arr.map((x) => {
    const sum = x.reduce((a, c) => a + Math.pow(c, 3), 0);
  if (sum % 2) {
    x.push(x[0]);
    x.shift();
    return x.join('');
    } else {
    return x.reverse().join(''); }
  });
  return res.join('');
}
```

## _(Tuesday) May 10_ 📢

>### Name `Exercise`↩️
```javascript 

```

## _(Wednesday) May 11_ 📢

>### Name `Exercise`
```javascript 

```

## _(Thursday) May 12_ 📢

>### Name `Exercise` ♻
```javascript 

```

## [📎 Back to main page !📎](/home/readAura.md)
