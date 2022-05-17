<h1 align="center">Ⓜ️ May Ⓜ️</h1>

## _(Monday) May 16_ 📢

`Learning about:` 💡
* **Everyday types in Typescript**

>### Square(n) Sum `Typescript Exercise` 🧮
```typescript 
export function squareSum(numbers: number[]): number {
  return numbers.reduce(
    (prev:number, curr:number) => prev + Math.pow(curr,2),
    0
  );
}
```

>### Growth Of A Population `Typescript Exercise` 🧟
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

>### Mumbling `Typescript Exercise` 🙊
```typescript 
export function accum(s: string): string {
  return s
    .split("")
    .map((l, i) => l.toUpperCase() + l.toLowerCase().repeat(i))
    .join("-");
}
```

>### A Wolf In Sheep's Clothing `Typescript Exercise` 🐺🐑
```typescript 
export function warnTheSheep(queue: string[]): string {
  const position = queue.reverse().indexOf('wolf');
  return position === 0 ? 'Pls go away and stop eating my sheep' : 
  `Oi! Sheep number ${ position }! You are about to be eaten by a wolf!`;
}
```

## _(Tuesday) May 17_ 📢
>### Title `Exercise`
```typescript 

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
