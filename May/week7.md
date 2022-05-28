<h1 align="center">Ⓜ️ May Ⓜ️</h1>

## _(Monday) May 23_ 📢

`Learning about:` 💡
* **Enquirer**

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
>#### [Learning about 🧠 What is OPP? 😶‍🌫️ The Four Principles and other functions 🤯 HERE!!](May/assets/guide.md)

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

```

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
* **Abstract Classes vs Interfaces** 🥊
* **Abstract Classes** 💭

## [📎 Back to main page !📎](/home/readAura.md)
