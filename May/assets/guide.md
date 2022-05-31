<h1 align="center"> 👓 OOP in TypeScript Guide 👓 </h1>

>### ¿What is OPP? 🌐
<code> Object Oriented programming (OOP) is a programming paradigm that relies on the concept of classes and objects. It is used to structure a software program into simple, reusable pieces of code blueprints (usually called classes), which are used to create individual instances of objects. </code>

>### OPP Four Principles 🗺️
>#### Abstraction 🌎
<code> Objects only reveal internal mechanisms that are relevant for the use of other objects, hiding any unnecessary implementation code. This concept helps developers more easily make changes and additions over time. </code>

`Code`
```typescript 
export default class abstraction {
  automaker: string;
  model: string;
  year: number;
  color: string;
  private owner: string = '';

  constructor(
    automaker: string,
    model: string,
    year: number,
    color: string,
  ) {
    this.automaker = automaker;
    this.model = model;
    this.year = year;
    this.color = color;
  } 

  carDescription() {
  console.log('Enter Car Details...🚗')
  return `${this.automaker} ${this.model} ${this.year} ${this.color}`;
  }

  registerCar(buyerName:string):void {
    this.owner=buyerName;
  }

  carSold() {
    console.log('Register the Owner...📋')
    console.log(`${this.owner} has bougth the brand new ${this.automaker} ${this.model} ${this.year}!!`);
  }
}
```
`Demonstration`

<img src="/May/assets/abstraction.gif" alt="Abstraction" width="350">

>#### Inheritance 👥
<code> Relationships and subclasses between objects can be assigned, allowing developers to reuse a common logic while still maintaining a unique hierarchy.</code>

`Code`
```typescript 
//Parent Class
export default class car {
  protected automaker: string;
  model: string;
  year: number;
  color: string;
  protected owner: string = '';
  

  constructor(
    automaker: string,
    model: string,
    year: number,
    color: string,
  ) {
    this.automaker = automaker;
    this.model = model;
    this.year = year;
    this.color = color;
  } 

  carDescription() {
  console.log('Enter Car Details...🚗')
  return `${this.automaker} ${this.model} ${this.year} ${this.color}`;
  }

  registerCar(buyerName:string) {
    this.owner=buyerName;
  }

  carSold() {
    console.log('Register the Owner...📋')
    console.log(`${this.owner} has bougth the brand new ${this.automaker} ${this.model} ${this.year}!!
    
    `);
  }
}
//Child Class
import car from './car'
export default class insurancePolicy extends car {
    private policyID: number;
    constructor(
      automaker: string,
      model: string,
      year: number,
      color: string,
      policyID: number
    ) {
      super(automaker, model, year, color);
      this.policyID = policyID;
      } 
      carSold(){
        super.carSold();
        console.log('Register the Insurance Policy...🚨')
        console.log(`${this.owner} Car's insurance policy number is ${this.policyID}.`);
      }   
    }
```
`Demonstration`

<img src="/May/assets/inheritance.gif" alt="Inheritance" width="500">

>#### Polymorphism ☄️  
<code> Objects can take on more than one form depending on the context. The program will determine which meaning or usage is necessary for each execution of that object. </code>

`Code`
```typescript 
export class car {
  Rent(type:string) : this {
    console.log(`${type} has been rented.🏁`);
    return this;
  }

  Record() : this {
    console.log(`Car was rented at ${new Date().toLocaleString()}⏱️`);
    return this;
  }

  Return(type:string) : this {
    console.log(`${type} has been returned at ${new Date().toLocaleString()}💵`);
    return this;
  }
}

export class ElectricCar extends car {
  Charge() : this {
    console.log(`Electric car has been charged.🔋`);
    return this;
  }
}

export class GasCar extends car {
  Refill() : this {
    console.log(`Gas car has been refilled.⛽`);
    return this;
  }
}
```
`Demonstration`

<img src="/May/assets/polymorphism.gif" alt="Polymorphism" width="500">

>#### Encapsulation 🧱
<code> This characteristic of data hiding provides greater program security and avoids unintended data corruption. </code>  

`Code`
```typescript 
export default class car {
  automaker: string;
  model: string;
  year: number;
  readonly cylinders: number = 6;
  readonly countryofOrigin: string;
 
  constructor( 
  automaker:string,
  model: string,
  year: number,
  country: string
  ){
    this.automaker = automaker;
    this.model = model;
    this.year = year;
    this.countryofOrigin = country;
  }
}
```
`Demonstration`

<img src="/May/assets/encapsulation.gif" alt="Encapsulation" width="500">

>### Special functions 
>#### Class 📰
<code> Classes contain properties (methods and attributes) which hold variables and operations.</code>

`Code`
```typescript 

```
`Demonstration`



>#### Object 🚨
<code> Objects are variables too. But objects can contain many values. </code>

`Code`
```typescript 

```
`Demonstration`



>#### Instance ⏲️
<code> An instance is a specific realization of any object. An object may be different in several ways, and each realized variation of that object is an instance. </code>

`Code`
```typescript 

```
`Demonstration`



>#### Interface 📝
<code> Interfaces are similar to type aliases, except they only apply to object types. </code>

`Code`
```typescript 

```
`Demonstration`



>#### Access Modifiers ✍️
<code> Accessibility restriction is the way how encapsulation or information hiding is implemented. This tenet of information hiding isolates the concern of one class from another. </code>

`Code`
```typescript

```
`Demonstration`



>#### Constructors 🚧
<code> Responsible for allocating memory for the objects of the class. </code>

`Code`
```typescript 

```
`Demonstration`



## [🔙 Back to Week 7 🔙](/May/week7.md)

<h3 align="center"> ⚡⚡⚡⚡⚡⚡⚡⚡⚡⚡⚡⚡⚡⚡⚡⚡⚡⚡ </h3>

## [📎 Back to main page !📎](/home/readAura.md)

