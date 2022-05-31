<h1 align="center">Ⓜ️ May Ⓜ️</h1>

## _(Monday) May 30_ 📢

`Learning about:` 💡
* **Object-Oriented Programming 📹 Resume Video**

>### Get Started With `TypeScript` 🪟
```typescript 
function addNumbers(num1:number, num2:number) {
    return num1 + num2;
  }
  console.log(addNumbers(3, 6));
```
>### Demostration
<img src="/May/assets/getstartedts.gif" alt="Get Started TS Microsoft" width="500"> `Badge` <img src="/May/assets/module1.png" alt="Abstraction" width="400">


>### Declare Variable Types In `TypeScript` ⌨️
```typescript 
// Module 2: Declare variable types in TypeScript
//  EXERCISE 1
let firstName:string;
let lastName:string;
let fullName:string;
let age:number;
let ukCitizen:boolean;

firstName = 'Rebecca';
lastName = 'Smith';
age = 42;
ukCitizen = false;
fullName = firstName + " " + lastName;

if (ukCitizen) {
    console.log("My name is " + fullName + ", I'm " + age + ", and I'm a citizen of the United Kingdom.");
} else {
    console.log("My name is " + fullName + ", I'm " + age + ", and I'm not a citizen of the United Kingdom.");
}

// EXERCISE 2
let x:number;
let y:number;
let a:number;

x = 5;
y = 7;
a = x + y;

console.log(a);

// EXERCISE 3
enum Season{
  Fall,
  Winter,
  Spring,
  Summer
}

function whichMonths(season: Season) {
   let monthsInSeason: string;  
    switch (season) {
        case Season.Fall:
            monthsInSeason = "September to November";
            break;
        case Season.Winter:
            monthsInSeason = "December to February";
            break;
        case Season.Spring:
            monthsInSeason = "March to May";
            break;
        case Season.Summer:
            monthsInSeason = "June to August";
    }
return monthsInSeason;
}

console.log(whichMonths(Season.Fall));

// EXERCISE 4
let randomNumbers: number[]= [];
let nextNumber:number;
   
   for (let i = 0; i < 10; i++) {
       nextNumber = Math.floor(Math.random() * (100 - 1)) + 1;
       randomNumbers.push(nextNumber);
   }  
console.log(randomNumbers);
```
>### Demostration
<img src="/May/assets/decvartype.gif" alt="Variables types TS Microsoft" width="500"> `Badge` <img src="/May/assets/module2.png" alt="Abstraction" width="400">

## _(Tuesday) May 31_ 📢
>### Title `Exercise`
```typescript 
```
---

<h3 align="center"> 🇯 🇺 🇳 🇪 </h3>

---
## _(Wednesday) June 01_ 📢
>### Title `Exercise`
```typescript 
```
## _(Thursday) June 02_ 📢
>### Title `Exercise`
```typescript 
```
## [📎 Back to main page !📎](/home/readAura.md)
