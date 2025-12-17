```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Title</title>
  <link rel="stylesheet" href="style.css">
  <script src="script.js"></script>
</head>
<body>

<!-- Headings -->
<h1>..</h1> ... <h6>..</h6>

<!-- Text -->
<p>Paragraph</p>
<br>
<hr>
<b>Bold</b> <strong>Strong</strong>
<i>Italic</i> <em>Emphasis</em>
<u>Underline</u>
<mark>Highlight</mark>
<small>Small</small>

<!-- Links -->
<a href="url" target="_blank">Link</a>
<a href="mailto:email">Email</a>

<!-- Images -->
<img src="img.jpg" alt="desc" width="" height="">

<!-- Lists -->
<ul><li>Item</li></ul>
<ol><li>Item</li></ol>
<dl><dt>Term</dt><dd>Desc</dd></dl>

<!-- Tables -->
<table>
  <tr><th>H</th><th>H</th></tr>
  <tr><td>Data</td><td>Data</td></tr>
</table>

<!-- Forms -->
<form action="#" method="GET/POST">
  <input type="text" name="">
  <input type="password" name="">
  <input type="email" name="">
  <input type="number" name="">
  <input type="checkbox" name="">
  <input type="radio" name="">
  <input type="submit" value="Send">
  <textarea name=""></textarea>
  <select><option>Option</option></select>
</form>

<!-- Media -->
<audio src="" controls></audio>
<video src="" controls width="" height=""></video>

<!-- Semantic Tags -->
<header></header>
<nav></nav>
<main></main>
<section></section>
<article></article>
<aside></aside>
<footer></footer>

<!-- Div & Span -->
<div></div>
<span></span>

<!-- Scripts & Links -->
<script></script>
<link rel="stylesheet" href="">

<!-- Meta & SEO -->
<meta name="description" content="">
<meta name="keywords" content="">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<!-- Comments -->
<!-- Comment -->

<!-- Special -->
<br> <hr> &nbsp; &copy; &lt; &gt; &amp;
```
```css
Yes! Here’s a compact **A–Z CSS cheat sheet** in short syntax form, designed to fit on 1 page for fast revision:

---

### **CSS Cheat Sheet (A–Z, Short Syntax)**

**A**

* `align-items: flex-start|center|flex-end|stretch;`
* `animation: name duration timing-function delay iteration-count direction;`

**B**

* `background: color|image|repeat|position|size;`
* `border: width style color;`
* `border-radius: 10px;`

**C**

* `color: #hex|rgb|name;`
* `cursor: pointer|default|move|text;`

**D**

* `display: block|inline|inline-block|flex|grid|none;`
* `direction: ltr|rtl;`

**F**

* `flex: grow shrink basis;`
* `flex-direction: row|column|row-reverse|column-reverse;`
* `float: left|right|none;`
* `font: style weight size/line-height family;`

**G**

* `gap: 10px;`
* `grid-template-columns: repeat(3, 1fr);`
* `grid-template-rows: auto;`

**H**

* `height: 100px|%;`
* `hover: selector { style }`

**J**

* `justify-content: flex-start|center|flex-end|space-between|space-around;`

**L**

* `line-height: 1.5;`
* `list-style: none|disc|circle|square;`

**M**

* `margin: 10px 20px;`
* `max-width: 100%;`
* `min-width: 200px;`

**O**

* `opacity: 0.5;`
* `overflow: visible|hidden|scroll|auto;`

**P**

* `padding: 10px 20px;`
* `position: static|relative|absolute|fixed|sticky;`
* `pointer-events: none|auto;`

**R**

* `resize: none|both|horizontal|vertical;`

**S**

* `shadow: box-shadow: 2px 2px 5px #000; text-shadow: 1px 1px #333;`
* `scroll-behavior: smooth;`
* `text-align: left|center|right|justify;`
* `text-decoration: none|underline|line-through;`
* `transition: property duration timing-function delay;`

**T**

* `top|right|bottom|left: 0|10px;`
* `transform: rotate(45deg)|scale(1.2)|translateX(10px);`
* `transition: all 0.3s ease;`

**V**

* `visibility: visible|hidden;`
* `vertical-align: top|middle|bottom;`

**W**

* `width: 100px|%;`
* `white-space: nowrap|pre|normal;`
* `word-wrap: break-word;`

**Z**

* `z-index: 1|10|auto;`

```
# java script
- javascript is used to give instruction to computer
- java script dynamically typed - you can change old values and reassign
* variable 
- case sensetive = a A,letter,digit,underscore,$ avilable,first character - _or $ or abc(letter)
- reserved  word != variable 

```js
1. Variables

let a = 10;
const b = 20;
var c = 30;


2. Data Types

typeof 10    // "number"
typeof "hi"  // "string"
typeof true  // "boolean"
typeof {}    // "object"
typeof []    // "object"
typeof null  // "object"
typeof (()=>{}) // "function"


3. Operators

+  -  *  /  %  
== != === !==  
> < >= <=  
&&  ||  !
+=  -=  *=  /=  
++  --


4. If / Else

if(x>5){ }
else if(x==5){ }
else{ }


5. Ternary

let r = x>5 ? "yes" : "no";


6. Functions

function f(a,b){ return a+b; }

const f2 = function(a,b){ return a+b; };

const f3 = (a,b) => a+b;

(function(){ })(); // IIFE


7. Recursion

function fact(n){
  if(n<=1) return 1;
  return n * fact(n-1);
}


8. Arrays

let arr = [1,2,3];

arr[0];  
arr.length;

arr.push(4);
arr.pop();
arr.shift();
arr.unshift(0);

arr.includes(2);
arr.indexOf(2);

arr.map(x=>x*2);
arr.filter(x=>x>1);
arr.reduce((a,b)=>a+b);
arr.forEach(x=>console.log(x));


9. Objects

let obj = {a:1, b:2};

obj.a;
obj["b"];

obj.c = 3;      // add
delete obj.b;   // delete

Object.keys(obj);
Object.values(obj);


10. Loops

for(let i=0;i<5;i++){}

while(x<5){ x++; }

do{ }while(x<5);

for(let x of arr){}
for(let k in obj){}


11. Strings

let s = "Hello";
s.length;
s.toUpperCase();
s.toLowerCase();
s.slice(1,3);
`${a} text`


12. DOM (Basic)

document.getElementById("id");
document.querySelector(".cls");
document.querySelectorAll("p");

el.textContent = "hi";
el.innerHTML = "<p>hi</p>";
el.style.color = "red";

el.addEventListener("click", ()=>{});


13. JSON

JSON.stringify(obj);
JSON.parse(str);


14. Math

Math.floor();
Math.ceil();
Math.round();
Math.random();


15. Date

let d = new Date();
d.getFullYear();
d.getMonth();
d.getDate();


16. Errors (Basic)

try { }
catch(e){ }
finally { }


17. Export / Import

export default f;
import f from "./file.js";
```
- React
```jsx
1. Component Creation

// Functional Component
const App = () => <div>Hello</div>;

// Class Component
class App extends React.Component {
  render() { return <div>Hello</div>; }
}


2. JSX

<div className="cls">{variable}</div>
{/* Comments */}
// Conditional
{condition && <p>Show</p>}
{condition ? <A/> : <B/>}


3. Props

const Child = ({name}) => <p>{name}</p>;
<Child name="Pallavi" />


4. State (useState)

const [count, setCount] = useState(0);
setCount(count + 1);


5. useEffect

useEffect(() => { /* side effect */ }, []); // on mount
useEffect(() => { /* effect */ }, [count]); // on count change


6. Event Handling

<button onClick={handleClick}>Click</button>
const handleClick = e => console.log(e);


7. Forms

<input value={name} onChange={e => setName(e.target.value)} />


8. Lists & Keys

arr.map((item, i) => <li key={i}>{item}</li>)


9. Conditional Rendering

{isLoggedIn ? <Dashboard/> : <Login/>}


10. Fragments

<React.Fragment>...</React.Fragment>
<></>


11. Context

const MyContext = React.createContext();
<MyContext.Provider value={val}>
  <Child/>
</MyContext.Provider>
const val = useContext(MyContext);


12. React Router (v6)

import {BrowserRouter, Routes, Route} from 'react-router-dom';
<BrowserRouter>
  <Routes>
    <Route path="/" element={<Home/>}/>
    <Route path="/about" element={<About/>}/>
  </Routes>
</BrowserRouter>


13. Conditional Class

<div className={isActive ? 'active' : ''}></div>


14. Inline Styles

<div style={{color: 'red', fontSize: '20px'}}>Hi</div>


15. Default Props & PropTypes

Child.defaultProps = {name: "Guest"};
Child.propTypes = {name: PropTypes.string};


16. React Memo / Pure Component

const MemoComp = React.memo(Component);
class PureComp extends React.PureComponent {}


17. Refs

const ref = useRef();
<input ref={ref} />
ref.current.focus();


18. Portals

ReactDOM.createPortal(<Child />, document.getElementById('modal'));


19. Error Boundary (Class Only)

class ErrorBoundary extends React.Component {
  state = {hasError:false};
  static getDerivedStateFromError(){return {hasError:true}}
  render(){return this.state.hasError ? <h1>Error</h1> : this.props.children}
}


20. Key Hooks Summary

useState   // state
useEffect  // side effect
useContext // context
useRef     // DOM ref
useMemo    // memoized value
useCallback // memoized fn
```
# Node js
1. What is Node.js?

Runtime that allows JavaScript to run outside the browser.

Built on Chrome’s V8 engine.

Used to create backend APIs, servers, scripts.

2. Create a Node Project
mkdir myapp
cd myapp
npm init -y


npm init -y → creates package.json.

3. Run a Node File
node app.js
```js
4. Console Output
console.log("Hello Node");

5. CommonJS Modules (require)

Export

// math.js
module.exports = {
  add(a, b) { return a + b; }
};


Import

const math = require('./math');
console.log(math.add(2, 3));

6. ES Modules (import/export)

Add "type": "module" in package.json.

Export

export function add(a, b) {
  return a + b;
}


Import

import { add } from './math.js';

7. Built-in Node Modules
a) fs – File System

Read file:

const fs = require('fs');

fs.readFile('text.txt', 'utf8', (err, data) => {
  console.log(data);
});


Write file:

fs.writeFile('data.txt', 'Hello', () => {});

b) path
const path = require('path');
console.log(path.join(__dirname, 'folder', 'file.txt'));

c) os
const os = require('os');
console.log(os.version());

d) http
const http = require("http");

const server = http.createServer((req, res) => {
  res.end("Hello Server");
});

server.listen(3000);

8. Create Simple API without Express
const http = require("http");

const server = http.createServer((req, res) => {
  if (req.url === "/") res.end("Home Page");
  if (req.url === "/api") res.end(JSON.stringify({ msg: "API data" }));
});

server.listen(3000);

9. Express.js Basics

Install:

npm install express


Create server:

const express = require("express");
const app = express();

app.get("/", (req, res) => {
  res.send("Hello Express");
});

app.listen(3000);

10. Middleware
app.use(express.json()); // Parse JSON body


Custom middleware:

app.use((req, res, next) => {
  console.log(req.method, req.url);
  next();
});

11. Routes
app.get("/users", (req, res) => {
  res.json({ name: "Pallavi" });
});

app.post("/users", (req, res) => {
  res.send("User created");
});

12. Environment Variables

Install dotenv:

npm install dotenv


.env file:

PORT=3000


Use:

require("dotenv").config();
console.log(process.env.PORT);

13. Nodemon (Auto Restart)

Install:

npm install -g nodemon


Run:

nodemon app.js

14. Promises + async/await
function getData() {
  return new Promise(resolve => resolve("Hello"));
}

async function show() {
  const data = await getData();
  console.log(data);
}

show();

15. Error Handling
try {
  JSON.parse("wrong");
} catch (err) {
  console.log("Error:", err.message);
}

16. Work with JSON
const data = { name: "Pallavi" };
console.log(JSON.stringify(data));

17. Importing Third-Party Packages
npm install axios


Use:

const axios = require("axios");

axios.get("https://api.example.com")
  .then(res => console.log(res.data));

18. Connect MongoDB (Mongoose)

Install:

npm install mongoose


Connect:

const mongoose = require("mongoose");

mongoose.connect(process.env.MONGO_URL)
  .then(() => console.log("DB Connected"));
```
19. Export Cheat Sheet (Quick Summary)
You must remember these:

- npm init -y
- require() or import
- module.exports / export
fs, path, os, http
- Express basics: app.get, app.post
- Middleware: express.json()
- async/await
- MongoDB connection with Mongoose
- dotenv for environment variables
- nodemon for restarting

# Express js
```js
(Short Syntax + Runnable Examples + Runtime Output)

1. Install & Setup
Syntax
npm init -y
npm install express

Basic Server
const express = require("express");
const app = express();

app.get("/", (req, res) => {
  res.send("Hello Express");
});

app.listen(3000);

Runtime Output (Terminal)
Server running on port 3000

Browser Output (Visit: http://localhost:3000
)
Hello Express

2. Middleware (Global)
Syntax
app.use(express.json());

Example
app.use((req, res, next) => {
  console.log("Middleware working");
  next();
});

Output (Terminal)
Middleware working
GET /

3. Routing Basics
GET
app.get("/user", (req, res) => {
  res.send("User Page");
});


Output

User Page

POST
app.post("/login", (req, res) => {
  res.send("Logged In");
});


Output

Logged In

PUT
app.put("/update", (req, res) => {
  res.send("Updated");
});


Output

Updated

DELETE
app.delete("/delete", (req, res) => {
  res.send("Deleted");
});


Output

Deleted

4. Route Parameters
Syntax
app.get("/user/:id", (req, res) => {
  res.send(req.params);
});

Example URL
http://localhost:3000/user/10

Output
{
  "id": "10"
}

5. Query Parameters
Syntax
app.get("/search", (req, res) => {
  res.send(req.query);
});

Example URL
http://localhost:3000/search?name=pallavi&age=22

Output
{
  "name": "pallavi",
  "age": "22"
}

6. Sending JSON Response
Syntax
app.get("/data", (req, res) => {
  res.json({ msg: "success", status: 200 });
});

Output
{
  "msg": "success",
  "status": 200
}

7. Static Files
Syntax
app.use(express.static("public"));

Example

Put index.html inside public → automatically served.

Browser Output

Shows your HTML file.

8. Using Express.json() (Body Parser)
Example
app.post("/api", (req, res) => {
  res.send(req.body);
});

Input (Postman)
{
  "name":"Pallavi",
  "skill":"JS"
}

Output
{
  "name":"Pallavi",
  "skill":"JS"
}

9. Express Router (Modular Routing)
userRoutes.js
const express = require("express");
const router = express.Router();

router.get("/", (req, res) => {
  res.send("User Home");
});

module.exports = router;

main file
const userRoutes = require("./userRoutes");
app.use("/users", userRoutes);

Output (Visit)
http://localhost:3000/users

User Home

10. Error Handling Middleware
Syntax
app.use((err, req, res, next) => {
  res.status(500).send("Error: " + err.message);
});

Example Error
app.get("/test", (req, res) => {
  throw new Error("Something broken");
});

Output
Error: Something broken

11. 404 Handling
Syntax
app.use((req, res) => {
  res.status(404).send("Not Found");
});

Output
Not Found

12. Sample Full Express App (Mini)
const express = require("express");
const app = express();
app.use(express.json());

app.get("/", (req, res) => res.send("Home"));
app.post("/add", (req, res) => res.json(req.body));

app.listen(3000, () => console.log("Running"));

OUTPUT

Terminal:

Running


Postman Response:

{ "your": "data" }

```


Class: Blueprint of object → class ClassName { }

Object: Instance of class → ClassName obj = new ClassName();

Constructor: Init object → ClassName() { }

Destructor: Clean up → ~ClassName() { }

Encapsulation: Hide data → private + public getters/setters

Abstraction: Hide implementation → abstract class/interface

Inheritance: Reuse code → class Child : Parent { }

Polymorphism: Many forms → Overloading / Overriding