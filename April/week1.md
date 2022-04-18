<h1 align="center">🅰️ April 🅰️</h1>

## _(Tuesday) April 05_ 📢

>### Interpreted And Compiled Programming Languages
- In a simple way we can say that:

   An interpreted language is read line by line, can be cross-plataform, interpreter required and the source code is public.

   A program with compiled language can be run when the coding is completed, we can share the executable but depends on the platform that we used initially and the source code is private.

>### Is Java compiled or interpreted, or both?
- Java is considered an hybrid language, that means both compiled and interpreted.

>### Pseudocode currency converter exercise
```
1. START
2. USD <-- GET 
3. BitValue <-- GET
4. BTC <-- USD * BitValue
5. PRINT BTC
6. END
```

## _(Wednesday) April 06_ 📢

>### Your date of birth in the matrix 💊
`My year of birth:` 1993   

**Converted to binary**
| 1024  |  512  |  256  |  128  |   64  |   32  |   16  |   8   |   4   |    2  |   1   |
|:-----:|:-----:|:-----:|:-----:|:-----:|:-----:|:-----:|:-----:|:-----:|:-----:|:-----:|
|   1   |   1   |   1   |   1   |   1   |   0   |   0   |   1   |   0   |   0   |   1   |

`Result:` **11111001001**

>### MIPS 💾
_1. Create a program to add two numbers given by the user_
```assembly
.data   
	#Values   
	      title: .asciiz "\nProgram Addition\n"
	      number1: .asciiz "\nEnter the first number:\n"
	      number2: .asciiz "\nEnter the second number:\n"
	      result: .asciiz  "\nThe result is:\n" 
  .text
  	#Print the title
	      main:
	      li $v0, 4
              la $a0, title
              syscall
	#Ask first number
              li $v0, 4
              la $a0, number1
              syscall
              li $v0, 5
              syscall
              move $t0, $v0
	#Ask second number
              li $v0, 4
              la $a0, number2
              syscall
              li $v0, 5
              syscall
              move $t1, $v0
	
	#Order the Addition
              add $t2, $t0, $t1
        
        #Print the result 
              li $v0, 4
              la $a0 result
              syscall
              li $v0, 1
              move $a0, $t2
              syscall 
```

_2. Create a program that display your name_

```assembly
.data
        greeting: .asciiz "\nMy name is Aura, nice to meet you :)\n"
  .text
        main:
              li $v0, 4
              la $a0, greeting
              syscall 
```
## _(Thursday) April 07_ 📢

>### Print special numbers 🔍 
`Iterative flow control using for`
```javascript
var num ='';

for (var num = 0; num <= 100; num++) {
    if (num % 2 ==0)
    console.log(num);
}
```
>### Bad Code 💀
`Bad‼️`
```javascript
var cond = false;
//❌ It's not the right comparison for the condition
if ((cond = true)) {
  console.log('The cond variable is true');
} else {
  console.log('The cond variable is false');
}
```
`Good✅`
```javascript
var cond = false;
//👍 It's the rigth abstract equality comparison for the condition
if (cond == true) {
    console.log('The cond variable is true');
} else {
    console.log('The cond variable is false');
}
```
>### Bad Code 2 🚫
```javascript
var n = 100;

if (n == 100) {
    console.log('This is a special number!');
}
else if (n < 1000 && n % 10 == 0 && n != 100) {
    console.log('This number is almost special');
} 
else if (n != 100 || n % 10 !==0) {
    console.log('Just a regular number');
}
```

## [📎 Back to main page !📎](https://github.com/aurachl/core-code-from-scratch/blob/e677ad52bedf877fc64ea62753f6b95c15360173/readAura.md)
