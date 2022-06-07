<h1 align="center">Ⓜ️ May Ⓜ️</h1>

## _(Monday) May 23_ 📢

`Learning about:` 💡
* **Enquirer**
> Stylish `CLI prompts` that are user-friendly, intuitive and easy to create. Is fast, easy to use, and lightweight enough for small projects, while also being `powerful and customizable` enough for the most advanced use cases.

>### Input `Example` ❓
<img src="./assets/input.png" alt="Input" width="500">

>### Form `Example` 📌
<img src="./assets/form.png" alt="Form" width="500">

>### Select `Example` 📎
<img src="./assets/select.gif" alt="Select" width="500">

>### Select By Id `Example` 🔢
<img src="./assets/selectbyID.gif" alt="SelectbyID" width="500">

>### Confirm `Example` ✅
<img src="./assets/confirm.gif" alt="Confirm" width="500">

>### OOP in TypeScript Guide `Exercise` 👓
>#### [Learning about 🧠 What is OPP? 😶‍🌫️ The Four Principles and other functions 🤯 HERE!!](/May/assets/guide.md)

## _(Tuesday) May 24_ 📢
>### Food Menu 👩‍🍳 `Exercise`
<img src="./assets/menuapp.gif" alt="Menu App" width="500">

>### Movies 📽️ `Exercise`

>### Menu and Exit 🎬
<img src="./assets/menumovies.gif" alt="Menu Movies" width="500">

>### Add Action Movie 🚓
<img src="./assets/addactionmovie.gif" alt="Add Action Movie" width="500">

>### Add Horror Movie 🪦
<img src="./assets/addhorrormovie.gif" alt="Add Action Movie" width="500">

>### Action Movies List 🚀
<img src="./assets/actionmovieslist.png" alt="Add Action Movie" width="500">

>### Horror Movies List ☠️
<img src="./assets/horrormovieslist.png" alt="Add Action Movie" width="500">

>### Increment Explosions ☢️
<img src="./assets/moreexplosions.gif" alt="Add Action Movie" width="500">

>### Increment Jump Scares 😨
<img src="./assets/morejumpscares.gif" alt="Add Action Movie" width="500">

## _(Wednesday) May 25_ 📢
>### Interfaces Guided `Exercise`
```typescript 
interface Loan {
        principal: number,
        interestRate: number 
    }

    interface ConventionalLoan extends Loan {
    months: number      
    }

function calculateInterestOnlyLoanPayment(loanTerms: Loan):string {   
    let interest:number = loanTerms.interestRate / 1200; 
    let payment:number;
    payment = loanTerms.principal * interest;
    return 'The interest only loan payment is ' + payment.toFixed(2);
}

function calculateConventionalLoanPayment(loanTerms: ConventionalLoan):string { 
    let interest:number = loanTerms.interestRate / 1200;
    let payment:number;
    payment = loanTerms.principal * interest / (1 - (Math.pow(1 / (1 + interest), loanTerms.months)));
    return 'The conventional loan payment is ' + payment.toFixed(2);
}
```
>### Demonstration
<img src="/May/assets/guideint.gif" alt="Implement Interfaces TS Microsoft" width="550"> `Badge` <img src="/May/assets/module3.png" alt="Module 3" width="400">

>### Build Tower `Exercise`
```typescript 
export const towerBuilder = (nFloors: number): string[] => {
  let array = [];
  for (let i = nFloors; i >= 1; i--) {
    let space = (nFloors - i);
    let stars = i * 2 - 1;
    array.push(" ".repeat(space) + "*".repeat(stars) + " ".repeat(space));
  }
  return array.reverse();
}
```

>### Meeting `Exercise`
```typescript 
export function meeting(s: string): string {
   return s
    .split(';')
    .map((el) => '(' + el.split(':').reverse().join(', ').toUpperCase() + ')')
    .sort()
    .join('');
}
```

## _(Thursday) May 26_ 📢
`Learning about:` 💡
* **Object Oriented Programming - The Four Pillars of OOP** 💠

> Abstraction 
>> Objects `only reveal internal mechanisms` that are `relevant for the use` of other objects, hiding any unnecessary implementation code. This concept helps developers more easily make changes and additions over time. 

> Inheritance 
>> Relationships and subclasses between objects can be assigned, `allowing developers to reuse a common logic` while still maintaining a unique hierarchy.

> Polymorphism
>> Objects can `take on more than one form` depending on the context. The program will determine which `meaning or usage is necessary` for each execution of that object. 

> Encapsulation
>> This characteristic of `data hiding` provides greater program `security` and `avoids` unintended data corruption. 

* **Abstract Classes vs Interfaces** 🥊
> The key difference between interfaces and abstract classes in any programming language is that `classes allow you to define implementation details`. `Interfaces solely define how data is structured`. Classes allow you to define methods, fields, and properties. Classes also provide a way to template objects, defining default values.

> Unlike other programming languages where interfaces can only be used with classes, TypeScript allows you to `use an interface to define a data structure without the need for a class`. You can use `interfaces to define` parameter objects for functions, define the structure for various framework properties, and define how objects look from remote services or APIs.

* **Abstract Classes** 💭
> Abstract classes are like a `mixture of implementing interfaces and extending a class in one step`. You can create a class with `optional methods and properties`, but also indicate which `methods and properties must be implemented in the derived class`. Note that your base class, despite enforcing abstract rules, is still able to itself implement any interfaces you desire.

## [📎 Back to main page !📎](/home/readAura.md)
