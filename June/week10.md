<h1 align="center">🇯 June 🇯</h1>

## _(Monday) June 13_ 📢

### React / Node.JS ⚛️

### Before we begin, here's a quick `FAQ` to introduce some key concepts 🚪
* **What is Node.js?** *Node.js is a `server-side` JavaScript `runtime environment` that executes `JavaScript` code.*
* **What is npm?** *The `default package manager` for Node.js is npm. A package manager makes it easier to `publish and share` Node.js source code libraries. The npm package manager simplifies library `installation, updating, and uninstallation`.*
* **What is React?** *React is a `front-end framework` for creating a `user interface` (UI).*
* **What is JSX?** *JSX is a JavaScript `syntax extension` typically used with React to `describe UI elements`. You must transpile `JSX code` to plain `JavaScript` before it can run in a `browser`.*
* **What is webpack?** *Webpack `bundles JavaScript files` so they can `run in a browser`, and can also transform or package other resources and assets. Webpack can specify a compiler, such as `Babel or TypeScript`, to transpile `JSX or TypeScript` code to plain `JavaScript`.*

### Differences between Node.js and React.js 🛑

<table><tr><th>Node.js</th><th>React.js</th></tr></thead><tbody><tr><td>Node.js used as a back-end framework</td><td>React is used for developing user interfaces.</td></tr><tr><td>It supports the Model–view–controller (MVC) framework.</td><td>Does not support the Model–view–controller (MVC) framework.</td></tr><tr><td>It runs on chrome’s v8 engine and uses an event-driven, non-blocking I/O model, which is written in C++.</td><td>It uses Node.js to compile and optimize the JavaScript code and easy to create UI Test cases.</td></tr><tr><td>Node.js handles requests and authentication from the browser, make database calls, etc.</td><td>It makes API calls and processes in-browser data.</td></tr><tr><td>Here the Real-time data streaming is handled easily.</td><td>In React complex architecture makes it hard to keep track of the traditional approach.</td></tr><tr><td>Framework for JavaScript execution having the largest ecosystem of open source libraries.</td><td>Facebook-backed Open Source JS library.</td></tr><tr><td>The language used is only JavaScript.</td><td>The language used is JSX and JavaScript.</td></tr><tr><td>There is no DOM (Document Object Model) concept that is Used.</td><td>Here the Virtual DOM (Document Object Model) is Used that makes it faster.</td></tr><tr><td>It is easy to write microservices in Node.Js</td><td>Microservices are difficult to be written in React.Js</td></tr><tr><td>It is highly scalable.</td><td>Scalability is still a challenge.</td></tr><tr><td>It has a simple architecture.</td><td>It has a complex architecture.</td></tr></table>

## _(Tuesday) June 14_ 📢

>### Covering the basics 🧬

### What Is React (React js) & Why Is It So Popular? ⭐
React is a JavaScript `library` for building fast and interactive `user interfaces`. It was developed at `Facebook` in 2011 and currently it's the `most popular` JavaScript library for building user interfaces becoming an amazing tool that helps to expand job opportunities as a `front-end developer`.

React applications are `components`, a component is essentially a piece of the user interface so when building applications with react we build a bunch of `independent isolated and reusable components` and then compose them to build `complex user interfaces`.

### Learning React 🚩
<img src="/June/assets/reacttest.gif" alt="Learning React" width="400">

>### Easter Egg List in `ReactJS` 🐰
```javascript 
import React from 'react';

export const EggList = (props) => {;
  let list = props.eggs.map((item, index) => {
    return <EasterEgg key = {index} name = {item}/>;      
  });
  
  return(<ul>{list}</ul>);
};

export const EasterEgg = (props) => {
  return <li>{props.name}</li>
};
```

## _(Wednesday) June 15_ 📢

>### Node.JS Core 🧠
### Questions ❓
<table>
  <tr><td>What is Node.JS?</td>
    <td>📗An open-source and cross-platform JavaScript runtime environment that introduces a lot of innovative thinking and approaches for JavaScript server-side development helping many developers.</td></tr>
  <tr><td>What problem does Node.JS solve?</td>
    <td>✔️Handles thousands of concurrent connections with a single server without introducing the burden of managing thread concurrency <br>
   ✔️Developers that write JavaScript for the browser with Node.JS are able to write the server-side code in addition to the client-side code without the need to learn a completely different language.</td></tr>
  <tr><td>What is the V8 Javascript Engine?</td>
    <td>✔️V8 is an open source runtime engine written in C++.<br>
    ✔️Chrome V8, or just V8, can execute JavaScript code either within or outside of a browser, which makes server-side scripting possible.</td></tr>
  <tr><td>Is Node.JS really necessary in the Development ecosystem?</td>
    <td>📗Node.js apps brings with them a huge advantage: the comfort of programming everything - the frontend and the backend - in a single language.</td></tr>
  <tr><td>What is the difference between Node.JS and any other browser?</td>
    <td>📗A big difference is that in Node.js you control the environment, compared to the browser environment, where you don't get the luxury to choose what browser your visitors will use, making the web app development easier.</td></tr>
  <tr><td>What is NVM and Why is it useful for Node.JS developers?</td>
    <td>✔️Node Version Manager (NVM) is a tool used to manage multiple active Node.js versions.<br>
    ✔️Makes it easier to manage multiple Node. js versions on a single environment.</td></tr>
</table>

>### Node.JS Module System Core 🧪
### Questions ❓
<table>
  <tr><td>What is a Javascript Module?</td>
    <td>📒A module is a function or group of similar functions grouped together within a file and containing the code to execute a specific task when called into a larger application.<br>
      In JavaScript is just a file containing related code, using the import and export keywords to share and receive functionalities respectively across different modules.</td></tr>
  <tr><td>Why are Javascript Modules necessary?</td>
    <td>📒To provide mechanisms for splitting JavaScript programs up into separate modules that can be imported when needed. Node.js has had this ability for a long time, and there are a number of JavaScript libraries and frameworks that enable module usage.</td></tr>
  <tr><td> What module standards are available in Node.JS?</td>
    <td>✔️http<br>
      ✔️url<br>
      ✔️querystring<br>
      ✔️path<br>
      ✔️fs<br>
      ✔️util</td></tr>
  <tr><td>What are the differences between ESModules and CommonJS modules?</td>
    <td>✔️ES modules are the standard for JavaScript, while CommonJS is the default in Node.js<br>
      ✔️Older Node.js versions don’t support ES modules<br>
      ✔️CommonJS offers flexibility with module imports<br>
      ✔️CommonJS loads modules synchronously, ES modules are asynchronous<br> </td></tr>
  <tr><td>Which types of modules exist in Node.JS?</td>
    <td>✔️Core Modules<br>
      ✔️Local Modules<br>
      ✔️Third Party Modules</td></tr>
</table>

>### Node.JS Module System Practice 💻
>#### Operations
```javascript 
function sum(num1, num2) {
  return num1 + num2;
}
  
function minus(num1, num2) {
  return num1 - num2;
}
  
module.exports = { sum, minus };
```

>#### Main
```javascript 
const { sum, minus } = require("./operations");

let firstNumber = 8
let secondNumber = 4

const add = sum(firstNumber, secondNumber)
const less = minus(secondNumber,firstNumber)

console.log(add)
console.log(less)
```

>### Client-Server Model 🔗 
### Questions ❓
<table>
  <tr><td>What is a Server?</td>
    <td>📡A Server in the IT world is a remote computer that provides access to data and services. Servers are usually physical devices such as rack servers, though the rise of cloud computing has brought virtual servers into the equation. The server handles processes like e-mail, application hosting, Internet connections, printing, and more.</td></tr>
  <tr><td>What is a Client?</td>
    <td>📡A Client is either a person or an organization using as a service. In the IT context, the client is a computer/device, also called a Host, that actually uses the service or accepts the information. Client devices include laptops, workstations, IoT devices, and similar network-friendly devices.</td></tr>
  <tr><td>Is a server just another physical computer?</td>
    <td>📡Depending on the situation, a server program may operate on either a physical computer or a virtual machine, but in the end is just another physical computer/device.</td></tr>
  <tr><td>Is there any similarity between human communication and the client-server model?</td>
    <td>📡Yes, for example the Sender-Message-Channel-Receiver Model of Communication</td></tr>
  <tr><td> Is the client-server model applicable only to the Web?</td>
    <td>📡Not necessarily, it's possible to processes data locally relying on a server to store persistent data.</td></tr>
</table>

> **Is a server just another physical computer?** 
<table>
  <tr><td>Why do we refer to a certain class of applications as Servers?</td>
    <td>📡Usually are network computers that store and run an application for client computers, and their function, occupy a large chunk of computing territory between database servers and the end user.</td></tr>
  <tr><td>What is the difference?</td>
    <td>📡They may need to connect to other servers to acquire information or provide services.</td></tr>
</table>

> **Is the client-server model applicable only to the Web?** 
<table>
  <tr><td>Can you mention any other example of this model outside the Web?</td>
    <td>✔️Printer Manager<br>
    ✔️File servers<br>
    ✔️Inventory</td></tr>
</table>
   
## _(Thursday) June 16_ 📢

>### APIs Core 💾

>### From JSON to REST 🛗

>### REST API Clients 📦

>### Express.JS Core 🎯

## [📎 Back to main page !📎](/home/readAura.md)
