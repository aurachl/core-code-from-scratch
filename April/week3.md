<h1 align="center">🅰️ April 🅰️</h1>

## _(Monday) April 25_ 📢

>### Who Likes It? `Exercise` 👍
```javascript 
function likes(names) {
  if (names.length === 0) return "no one likes this";
  if (names.length === 1) return `${names[0]} likes this`;
  if (names.length === 2) return `${names[0]} and ${names[1]} like this`;
  if (names.length === 3) return `${names[0]}, ${names[1]} and ${names[2]} like this`;
  else return `${names[0]}, ${names[1]} and ${names.length -2} others like this`;
  }
```

>### Bit Counting `Exercise` 🧮
```javascript 
var countBits = function(n) {
  let byn = n.toString(2);
  let array1 = Array.from(byn);
  let total = array1.reduce((total, value) => total + Number(value), 0);
  return Number(total);
};
```

>### Your Order, Please `Exercise` 🔠🔡🔢
```javascript 
function order(words){
    if (words.length == 0){return words}
  let wordsarr = words.split(' ');
  let search = words.match(/\d/g);
  let ordstr = [];
    for (let i=1;i<=search.length;i++){
    let order = search.indexOf(i.toString())
    ordstr.push(wordsarr[order]) }
  return ordstr.join(' ')
}
```

## _(Tuesday) April 26_ 📢

>### Simple Pig Latin `Exercise` 🌀
```javascript 
function pigIt(str){
  const arr = str.split(' ')
  return arr
    .map((word) => {
    return word.match(/[A-z]/i)
    ? `${word.substr(1)}${word.substr(0, 1)}ay`
    : word
    })
  .join(' ')
}
```

>### Counting Duplicates `Exercise` 👀
```javascript 
function duplicateCount(text){
  const characters = new Set(); 
  const repeated = new Set();
  for (const char of text.toLowerCase()) {
    if (characters.has(char)) { repeated.add(char);} 
    else { characters.add(char); }
  }
  return repeated.size;
}
```

>### Decode The Morse Code `Exercise` 🚢
```javascript 
decodeMorse = function(morseCode) {
  function decodeMorseLetter(letter) { return MORSE_CODE[letter]; }
  function decodeMorseWord(word) { return word.split(' ').map(decodeMorseLetter).join(''); }
  return morseCode.trim().split('   ').map(decodeMorseWord).join(' ');
    }
```

## _(Wednesday) April 27_ 📢

>### Title
`Highlight` 
## _(Thursday) April 28_ 📢

>### Title
## [📎 Back to main page !📎](/home/readAura.md)
