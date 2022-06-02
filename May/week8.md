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
>### Demonstration
<img src="/May/assets/getstartedts.gif" alt="Get Started TS Microsoft" width="500"> `Badge` <img src="/May/assets/module1.png" alt="Module 1" width="400">


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
>### Demonstration
<img src="/May/assets/decvartype.gif" alt="Variables types TS Microsoft" width="500"> `Badge` <img src="/May/assets/module2.png" alt="Module 2" width="400">

## _(Tuesday) May 31_ 📢

`Learning about:` 💡
* **Abstract Classes vs Interfaces📹**

>### Develop Typed Functions `Exercise`
```typescript 
//EXERCISE 1
    interface compareFunctionType {
        (a: number, b:number): number;
    }

let sortDescending: compareFunctionType = (a, b) => {
    if (a > b) {
        return -1;
    } else if (b > a) {
        return 1;
    } else {
        return 0;
    }
}

let sortAscending : compareFunctionType = (a, b) => {
    if (a > b) {
        return 1;
    } else if (b > a) {
        return -1;
    } else {
        return 0;
    }
}

function buildArray(items:number, sortOrder: 'ascending'|'descending'):number[] {
    let randomNumbers:number[] = [];
    let nextNumber:number;
    for (let counter = 0; counter < items; counter++) {
        nextNumber = Math.ceil(Math.random() * (100 - 1));
        if (randomNumbers.indexOf(nextNumber) === -1) {
          randomNumbers.push(nextNumber);
        } else {
          counter--;
        }
    }
    if (sortOrder === 'ascending') {
      return randomNumbers.sort(sortAscending);
    } else {
      return randomNumbers.sort(sortDescending);
    }
}
//TEST
let myArray1 = buildArray(12, 'ascending');
let myArray2 = buildArray(8, 'descending');
console.log(myArray1);
console.log(myArray2);

//EXERCISE 2
function loanCalculator (principle:number, interestRate:number, months=12):string {
    let interest:number = interestRate / 1200;   // Calculates the monthly interest rate
    let payment:number;
    payment = principle * interest / (1 - (Math.pow(1/(1 + interest), months)));
    return payment.toFixed(2);
}
//TEST
let myLoan = loanCalculator(1000, 5);
console.log(myLoan);
```
>### Demonstration
<img src="/May/assets/devtypfunc.gif" alt="Develop Typed Functions TS Microsoft" width="500"> `Badge` <img src="/May/assets/module4.png" alt="Module 4" width="400">

>### Declare and Instantiate Classes  `Exercise`
```typescript 
class BuildArray {
 
    private _items: number;
    private _sortOrder: 'ascending'|'descending';

    constructor(items:number, sortOrder:'ascending'|'descending'){
        this._items = items;
        this._sortOrder = sortOrder;
    }
 
    get items() {
        return this._items;
    }
    set items(items) {
        this._items = items;
    }
    get sortOrder() {
        return this._sortOrder;
    }
    set sortOrder(sortOrder) {
        this._sortOrder = sortOrder;
    }
   
    private sortDescending = (a: number, b: number) => {
        if (a > b) {
            return -1;
        } else if (b > a) {
            return 1;
        } else {
            return 0; }
    }

    private sortAscending = (a: number, b: number) => {
        if (a > b) {
            return 1;
        } else if (b > a) {
            return -1;
        } else {
            return 0;
        }
    }

    buildArray(): number[] {
        let randomNumbers: number[] = [];
        let nextNumber: number;
        for (let counter = 0; counter < this.items; counter++) {
            nextNumber = Math.ceil(Math.random() * (100 - 1));
            if (randomNumbers.indexOf(nextNumber) === -1) {
                randomNumbers.push(nextNumber);
            } else {
                counter--;
            }
        }
        if (this.sortOrder === 'ascending') {
            return randomNumbers.sort(this.sortAscending);
        } else {
            return randomNumbers.sort(this.sortDescending);
        }
    }
}

let testArray1 = new BuildArray(12, 'ascending');
let testArray2 = new BuildArray(8, 'descending');
//TEST
console.log(testArray1.buildArray());
console.log(testArray2.buildArray());
```
>### Demonstration
<img src="/May/assets/decinstclass.gif" alt="Declare and Instantiate Classes TS Microsoft" width="500"> `Badge` <img src="/May/assets/module5.png" alt="Module 5" width="400">

---

<h3 align="center"> 🇯 🇺 🇳 🇪 </h3>

---
## _(Wednesday) June 01_ 📢
>### Define Generics `Exercise`
```typescript 

```
>### Demonstration
<img src="/May/assets/defgen.gif" alt="Define Generics TS Microsoft" width="500"> `Badge` <img src="/May/assets/module6.png" alt="Module 6" width="400">

>### Make the Deadfish Swim `Exercise`
```typescript 

```

## _(Thursday) June 02_ 📢
>### Title `Exercise`
```typescript 
```
## [📎 Back to main page !📎](/home/readAura.md)
