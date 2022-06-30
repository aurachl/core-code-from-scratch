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


console.log(sum(8,4))
console.log(minus(10,2))
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
>### What is an API?
An application programming interface is a connection between computers or between computer programs. It is a type of software interface, offering a service to other pieces of software. A document or standard that describes how to build or use such a connection or interface is called an API specification.
>### What is a Protocol
In computer science, a set of rules or procedures for transmitting data between electronic devices, such as computers. In order for computers to exchange information, there must be a preexisting agreement as to how the information will be structured and how each side will send and receive it.
Among the most important sets of Internet protocols are TCP/IP (Transmission Control Protocol/Internet Protocol), HTTPS (Secure HyperText Transmission Protocol), SMTP (Simple Mail Transfer Protocol), and DNS (Domain Name System).
>### Is the term API only applicable to the communication of programs over the Internet?
There are Private APIs that are often used within an enterprise to improve collaboration. While the API itself is also open as a public API, the difference is it is only open to those that have been granted access. Developers within an organization can take advantage of the functionality from the private API to design and build applications inside the company. Private APIs can leverage the existing functionality of enterprise applications so company employees can communicate more efficiently.
>### Why is structured communication between two programs important?
Structured communcation allows computers/programs to communicate in the same way so the client and server can interact seemlessly. For example, without a protocol, a transmitting computer, for example, could be sending its data in 8-bit packets while the receiving computer might expect the data in 16-bit packets. Protocols are established by international or industrywide organizations.

>> Do we humans use APIs when communicating without technology?
>> 
>> We do use APIs, such as languages and means of communication. By using the same language we make sure our listener understands our message. And by using the same means of communication (letter, messages, e-mail, spoken language), we ensure our messages are being received.

>### Is an API just another program or a standard?
An API is a program that allows the communication between to applications/computer systems. However, given the fact they are so necessary they've become a standard for such programs to communcate and let a complete ecosystem work smoothly.
>###  Do you know any API? Can you list at least 5 examples of APIs?
1. Weather Snippets
2. Log-in Using XYZ
3. Pay with PayPal
4. Twitter Bots
5. Travel Booking
*************************************************************************
>### From JSON to REST 🛗
>### What is HTTP?
The Hypertext Transfer Protocol is an application layer protocol in the Internet protocol suite model for distributed, collaborative, hypermedia information systems.
>### What is JSON?
JSON is an open standard file format and data interchange format that uses human-readable text to store and transmit data objects consisting of attribute–value pairs and arrays. It is a common data format with diverse uses in electronic data interchange, including that of web applications with servers

>>Is JSON the same as a plain Javascript object?
>>
>>The JSON format is syntactically identical to the code for creating JavaScript objects. Because of this similarity, a JavaScript program can easily convert JSON data into native JavaScript objects.

>### What is REST?
REST, or REpresentational State Transfer, is an architectural style for providing standards between computer systems on the web, making it easier for systems to communicate with each other. REST-compliant systems, often called RESTful systems, are characterized by how they are stateless and separate the concerns of client and server.

>>Is REST a programming language, framework, technology, or architecture pattern?
>>
>>Rest is an architecture pattern that improves the way clients and servers interact with each other.

>### What is a Resource in REST?
A resource in REST is a similar Object in Object Oriented Programming or is like an Entity in a Database. Once a resource is identified then its representation is to be decided using a standard format so that the server can send the resource in the above said format and client can understand the same format.

>>What is a resource identifier?
>>
>>Resource identification is the most flexible aspect of designing a REST based system. There is no exact science to identifying resources and there is no right or wrong with resources identified. We can identify resources from domain nouns. A resource could be a document, a video, a business process or even a device.
    
>### What is an HTTP method?
HTTP defines a set of request methods to indicate the desired action to be performed for a given resource. Although they can also be nouns, these request methods are sometimes referred to as HTTP verbs.

>>What HTTP methods does REST use within its architecture rules?
>>
>>There are five methods commonly used within REST: Post, Put, Patch, Get, and Delete.
  
>>Why do we use HTTP methods in REST and how do they relate to resources?
>>
>>HTTP is a communication protocol with a given mechanism for server-client data transfer. It's most commonly used in REST API just because REST was inspired by WWW (world wide web) which largely used HTTP before REST was defined, so it's easier to implement REST API style with HTTP.
>>
>>A REST Resource is data on which we want to perform operations and the HTTP methods help us manipulate that data, that is there intrinsic relationship.
    
>### Is REST the same as HTTP?
While many people continue to use the terms REST and HTTP interchangeably, the truth is that they are different things. REST refers to a set of attributes of a particular architectural style, while HTTP is a well-defined protocol that happens to exhibit many features of a RESTful system.
*************************************************************************
>### REST API Clients 📦
>### Postman only works with REST APIs?
Postman can make HTTP calls using SOAP, a platform-independent messaging protocol specification, in addition to REST, GraphQL, and WebSocket requests. 
>### Is there an alternative to Postman?
Swagger UI, Insomnia REST Client, Paw, Apigee, and cURL are the most popular alternatives and competitors to Postman.
*************************************************************************
>### Express.JS Core 🎯
```javascript 
const express = require('express')
const app = express()
const port = 3000

app.get('/', (req, res) => {
    res.send('Hello World!')
})

app.listen(port, () => {
    console.log(`Express.JS Core Understanding`)
    console.log(`Example running on port ${port}`)
})
```
<img src="/June/assets/hwexpress.gif" alt="Example Express" width="400">

*************************************************************************

## [📎 Back to main page !📎](/home/readAura.md)
