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
>### Title `Exercise`
```typescript 

```

## _(Thursday) May 19_ 📢
>### Title `Exercise`
```typescript 

```

## [📎 Back to main page !📎](/home/readAura.md)
