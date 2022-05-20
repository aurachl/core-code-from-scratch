<h1 align="center">Ⓜ️ May Ⓜ️</h1>

## _(Monday) May 16_ 📢

`Learning about:` 💡
* **Everyday types in TypeScript**

>### Square(n) Sum `TypeScript Exercise` 🧮
```typescript 
export function squareSum(numbers: number[]): number {
  return numbers.reduce(
    (prev:number, curr:number) => prev + Math.pow(curr,2),
    0
  );
}
```

>### Growth Of A Population `TypeScript Exercise` 🧟
```typescript 
export class G964 {

    public static nbYear = (p0, percent, aug, p) => {
      percent = percent / 100;
      if(aug === null) aug = 0; 
      let count = 0;
      while (p0 < p) {
        p0 = Math.floor(p0 + p0 * percent + aug);
        count++;
      }  
      return count; 
    }
}
```

>### Mumbling `TypeScript Exercise` 🙊
```typescript 
export function accum(s: string): string {
  return s
    .split("")
    .map((l, i) => l.toUpperCase() + l.toLowerCase().repeat(i))
    .join("-");
}
```

>### A Wolf In Sheep's Clothing `TypeScript Exercise` 🐺🐑
```typescript 
export function warnTheSheep(queue: string[]): string {
  const position = queue.reverse().indexOf('wolf');
  return position === 0 ? 'Pls go away and stop eating my sheep' : 
  `Oi! Sheep number ${ position }! You are about to be eaten by a wolf!`;
}
```
    
## _(Tuesday) May 17_ 📢
>### A Rule Of Divisibility By 13  `TypeScript Exercise` 1️⃣3️⃣
```typescript 
export function thirt(n: number): number {
  const arr: number[] = [1,10,9,12,3,4];
  while (n >= 100){
    let sum:number = 0;
    let test:number = n;
    let i: number = 0;
    while (test != 0){
      sum += (test % 10) * arr[ i++ % 6];
      test = Math.floor(test / 10);
    }
    n = sum;
  }
  return n;
}
```

>### Playing With Digits `TypeScript Exercise` 🎮
```typescript 
export class G964 {

    public static digPow = (n: number, p: number) =>
      (n=(String(n)
      .split('')
      .reduce((sum: number , d: string) => 
              sum + (+d) ** p++, 0) / n), n % 1 ? -1 : n);
    }
```

>### Valid Braces `TypeScript Exercise` 🔍
```typescript 
export function validBraces(braces: string): boolean {
  while (/\(\)|\[\]|\{\}/g.test(braces))
  {
    braces = braces.replace(/\(\)|\[\]|\{\}/g,"")
  }
 return !braces.length;
}
```

>### Tic-Tac-Toe `JavaScript Exercise` ❌⭕❌
```javascript 
function solveTTT(board) {
  var xwin = [
    [0, 1, 2],
    [3, 4, 5],
    [6, 7, 8],
    [0, 3, 6],
    [1, 4, 7],
    [2, 5, 8],
    [0, 4, 8],
    [2, 4, 6],
  ];
  for (var i in xwin)
    if (xwin[i].map((x) => board[x]).join('') == 'XX')
      return xwin[i].reduce((x, y) => (board[y] == '' ? x + y : x), 0);
  for (var i in board) if (board[i] == '') return +i;
}
```

>### Tic-Tac-Toe-Like Table Generator `JavaScript Exercise` ⭕❌⭕
```javascript 
function displayBoard(board, width){
  let result = "";
  for (let i = 0; i < board.length; i++) {
    if (i > 0 && i % width === 0) {
      result += "---".repeat(width) + "-".repeat(width - 1) + "\n";
    }

    result += " " + board[i] + " ";

    if (i + 1 < board.length) {
      if ((i + 1) % width === 0) result += "\n";
      else result += "|";
    }
  }
  return result;
}
```

## _(Wednesday) May 18_ 📢
>### Duplicate Encoder `TypeScript Exercise` 🖩
```typescript 
export function duplicateEncode(word: string){
  return word
    .toLowerCase() // Transform the word to lowercase to ignore case
    .split('')    // Transform the string to a array, with each item containing a letter
    .map((letter:string,index:number,convert:string[]) =>{
      // Verify if the word list in lowercase have the first and last appearance, and return correct bracket 
      return convert.indexOf(letter) == convert.lastIndexOf(letter) ? '(' : ')';
    })
    // Have to return everything on a 'string'
    .join('');
}
```

>### Find The Odd Int `TypeScript Exercise` 👀
```typescript 
export const findOdd = (xs: number[]): number => {
 //With the reduce method and using XOR operator (^) we cancel/delete the duplicates returning the number with unique appereance
 return xs.reduce((a:number,c:number) => a^c, 0);
}
```

>### Which Are In? `TypeScript Exercise` ⛔
```typescript 
export class G964 {
  public static inArray(a1: string[], a2: string[]): string[] {
  //The sorted array to return
  let r : string[] = [];
  //Let's search word by word in both arrays
  for(let a1Word in a1){
  for(let a2Word in a2){
    //In the case of one word of a2 contains a1 word as well we 'push' the match to the 'r' array
    if (a2[a2Word].indexOf(a1[a1Word]) >= 0 && r.indexOf(a1[a1Word]) < 0) {
      r.push(a1[a1Word]);
    }
  }
  }
  //Lexicographical order 
  return r.sort();
  }
}
```

>### Sums Of Parts `TypeScript Exercise` 👥
```typescript 
export function partsSums(ls: number[]): number[] {
  let sum = ls.reduce((sum:number, n:number) => sum + n, 0),
  res  = [sum]
  for (let i = 1; i <= ls.length; i++){
    sum -= ls[i-1]
    res.push(sum)
  }
  return res
}
```

>###  Consecutive Strings `TypeScript Exercise` 📠
```typescript 
export function longestConsec(strarr: string[], k: number): string {
  if (k > strarr.length || k < 1) return '';
  return strarr.reduce(function(prevLongest, c, i, a) {
    var str = a.slice(i, i + k).join('');
    return str.length > prevLongest.length ? str : prevLongest;
  }, 
  '');
}
```
   
## _(Thursday) May 19_ 📢
>### Tile `TypeScript Exercise` 🔳🔲🔳🔲
```typescript 
export class Tile {
  letter: string;
  value: number;

  constructor(letter:string, value:number){
    this.letter = letter;
    this.value = value;
   }

  printTile(){
    console.log(`
    ==================
    Letter: ${this.letter}
    Value: ${this.value}
    ==================
    `);
  }
}
```

>### Time `TypeScript Exercise` ⏰
```typescript 
export class Time {
  hour: number;
  minute: number;
  second: number;

  constructor(hour:number, minute:number, second:number){
    this.hour = hour;
    this.minute = minute;
    this.second = second;
   }
  
  printTime () {
    console.log(`
    ==================
    Hours: ${this.hour}
    Minutes: ${this.minute}
    Seconds: ${this.second}
    ==================
   
    `);
  }

  getInSeconds():number {
    const second = this.hour * 3600 + this.minute * 60 + this.second;
    return this.second;
  }
  
}
```

>### Rational `TypeScript Exercise` 🧠
```typescript 
export class Rational {
  numerator: number;
  denominator: number;
  
  constructor(numerator:number, denominator:number){
    this.numerator = numerator;
    this.denominator = denominator;
   }
  
  printRational () {
    console.log(`${this.numerator} / ${this.denominator}`);
  }

  invert () {
    [this.numerator, this.denominator ] = [this.denominator, this.numerator ];
  }

  toFloat () :number {
    return this.denominator / this.numerator ;
  }

  gcd (num:number, den:number):number{
    if (den == 0) return num;
    return this.gcd(den, num % den);
  }
  
  reduce () {
    const gcd = this.gcd(this.numerator, this.denominator);
    this.numerator = this.numerator / gcd;
    this.denominator = this.denominator / gcd;
  }

}
```


## [📎 Back to main page !📎](/home/readAura.md)
