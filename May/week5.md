<h1 align="center">Ⓜ️ May Ⓜ️</h1>

## _(Monday) May 09_ 📢

>### Find The Missing Letter `Exercise` 🔍
```javascript 
function findMissingLetter(array) {
//We move the array elements into a string to make the search easy
  let string = array.join("");
  //Let's move between the letters on the string with the help of 'for'
    for (let i = 0; i < string.length; i++) {
    //Now, using the Unicode values of the letters with 'charCodeAt' we check if the order don't match
      if (string.charCodeAt(i + 1) - string.charCodeAt(i) != 1) {
      //In the case of finding that something is missing, we return that letter
      return String.fromCharCode(string.charCodeAt(i) + 1);}
    }
}
```

>### Reverse Or Rotate? `Exercise`↩️
```javascript 
function revrot(str, sz) {
  //Validates initial conditions
  if (sz <= 0 || str == '' || sz > str.length) return '';
  const arr = [];
  //String to array
  const s = str.split('');
  //Defines the number of chunks according to 'sz' value
  while (s.length >= sz) {
    arr.push(s.splice(0, sz));
  }
  //Apply 'map' instruction to the array
  const res = arr.map((x) => {
    //Calculate the sum of the cubes of the digits in the array
    const sum = x.reduce((a, c) => a + Math.pow(c, 3), 0);
    //Validate if the sum is divisible by 2
    if (sum % 2) {
      //Sent first digit to the back
      x.push(x[0]);
      x.shift();
      return x.join('');
    } else {
      //Reverse chunk
      return x.reverse().join(''); 
    }
  });
  //Show result
  return res.join('');
}
```

## _(Tuesday) May 10_ 📢

`Learning about:` 💡
* **TypeScript Handbook**
> The `TypeScript Handbook` is intended to be a `comprehensive document` that `explains TypeScript` to everyday `programmers`. You can `read` the handbook by going from `top to bottom` in the `left-hand` navigation. The documentation includes the `basics, objects types,  type manipulation, classes, modules`, etc.

* **Type vs Interface in TypeScript**
> The difference between types and interfaces in TypeScript used to be more clear, but with the latest versions of TypeScript, they’re becoming more similar.

`Interfaces` are basically a way to `describe data shapes`, for example, an object.

`Type` is a definition of a `type of data`, for example, a union, primitive, intersection, tuple, or any other type.

`Interfaces` are better when you `need to define a new object or method of an object`. 

`Types` are better when you `need to create functions`, for example. Let’s imagine that we have a function that’s going to return an object called, type alias is more recommended for this approach

>### TypeScript Object Type `Exercise` 📑
```typescript
//We create the 'User' interface were we gonna define the types
export interface User {
  name: string;
  age: number;
  occupation: string;
}

//We use the interface
export const users: User[] = [
    {
        name: 'Max Mustermann',
        age: 25,
        occupation: 'Chimney sweep'
    },
    {
        name: 'Kate Müller',
        age: 23,
        occupation: 'Astronaut'
    }
];

//We validate that we're using the correct types
export function logPerson(user: User) {
    console.log(` - ${user.name}, ${user.age}`);
}

console.log('Users:');
users.forEach(logPerson);
```

>### TypeScript Unions `Exercise` 🇩🇪
```typescript 
interface User {
    name: string;
    age: number;
    occupation: string;
}

interface Admin {
    name: string;
    age: number;
    role: string;
}

//Using the 'Union' types we create the type 'Person' that have the values of User and Admin
export type Person = User | Admin;

//Now we use that new type/array
export const persons: Person[] /* <- Person[] */ = [
    {
        name: 'Max Mustermann',
        age: 25,
        occupation: 'Chimney sweep'
    },
    {
        name: 'Jane Doe',
        age: 32,
        role: 'Administrator'
    },
    {
        name: 'Kate Müller',
        age: 23,
        occupation: 'Astronaut'
    },
    {
        name: 'Bruce Willis',
        age: 64,
        role: 'World saver'
    }
];

//Validate
export function logPerson(user: Person) {
    console.log(` - ${user.name}, ${user.age}`);
}

persons.forEach(logPerson);
```

## _(Wednesday) May 11_ 📢

`Learning about:` 💡
* **FP vs OOP**
* **OOP**
* **Fundamental Concepts of Object Oriented Programming**

## _(Thursday) May 12_ 📢

>### What's Your Poison? `Exercise` 💀
```javascript 
function find(rats) {
  return rats.reduce((total, a) => total + Math.pow(2, a), 0);
}
```

>### Array.diff `Exercise` 💨
```javascript 
function arrayDiff(a, b) {
  return a.filter((diff) => !b.includes(diff));
}
```

## [📎 Back to main page !📎](/home/readAura.md)
