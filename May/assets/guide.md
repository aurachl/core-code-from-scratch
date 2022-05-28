<h1 align="center"> 👓 OOP in TypeScript Guide 👓 </h1>

>### ¿What is OPP? 🌐
<code> Object Oriented programming (OOP) is a programming paradigm that relies on the concept of classes and objects. It is used to structure a software program into simple, reusable pieces of code blueprints (usually called classes), which are used to create individual instances of objects. </code>

>### OPP Four Principles 🗺️
>#### Abstraction 🌎
<code> Objects only reveal internal mechanisms that are relevant for the use of other objects, hiding any unnecessary implementation code. This concept helps developers more easily make changes and additions over time. </code>

`Example`
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
<img src="./assets/abstraction.gif" alt="Abstraction" width="500">

>#### Inheritance 👥
<code> Relationships and subclasses between objects can be assigned, allowing developers to reuse a common logic while still maintaining a unique hierarchy.</code>

`Example`
```typescript 
```

>#### Polymorphism ☄️  
<code> Objects can take on more than one form depending on the context. The program will determine which meaning or usage is necessary for each execution of that object. </code>

`Example`
```typescript 
```

>#### Encapsulation 🧱
<code> This characteristic of data hiding provides greater program security and avoids unintended data corruption. </code>  

`Example`
```typescript 
```

>### Special functions 
>#### Class 📰
<code> Classes contain properties (methods and attributes) which hold variables and operations.</code>

`Example`
```typescript 
```

>#### Object 🚨
<code> Objects are variables too. But objects can contain many values. </code>

`Example`
```typescript 
```

>#### Instance ⏲️
<code> An instance is a specific realization of any object. An object may be different in several ways, and each realized variation of that object is an instance. </code>

`Example`
```typescript 
```

>#### Interface 📝
<code> Interfaces are similar to type aliases, except they only apply to object types. </code>

`Example`
```typescript 
```

>#### Access Modifiers ✍️
<code> Accessibility restriction is the way how encapsulation or information hiding is implemented. This tenet of information hiding isolates the concern of one class from another. </code>

`Example`
```typescript 
```

>#### Constructors 🚧
<code> Responsible for allocating memory for the objects of the class. </code>

`Example`
```typescript 
```
