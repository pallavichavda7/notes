## HTML
for better view  press ctrl+k , v
### SHORTCUTS
* Better view  * ctrl+ k then v,
* word wrap = alt+z,
* short cuts find vs code = ctrl+k ctrl+s
* Ctrl +K = clear console
* Cmd + k = clear console in mac
* Ctrl +R = refresh crome or console
* Ctrl +/= comment out
* /n next line print
* /p space tab print
* Ctrl + x = for the cuting the line
- boiler plate ! enter
- emmet abrivations type *lorem 120 (number of word 120)
- ctrl + shift for backwards do things
-  copy from sourse to add in foler which you are working paste image in vs code
-  tab - write tag name press tab for compleeting the tag
- alt +Z for toogle word wrap 
- tap prettier for good view of wrriten codes
- link:css for connect css file
- ctrl+/ for comment out
- shift+alt+down for copy uper line of the code

### HTML Learning Path: Beginner to Advanced
* intro - HTML was invented by TIM BERNERS-LEE, a British scientist.He Developed HTML in 1991 while working at CERN (European organization for nuclear reserch) to create system for sharing and linking documents over the internet, which became, worldwideweb(later renamed Nexus),and the first web server,CERN HTTpd.
 - current version of HTML is HTML 5.2 

#### Beginner Level

1. *Introduction to HTML*
   - *Definition:* HTML (HyperText Markup Language) is the standard language for creating web pages.
   <head> - meta deta contain hidden things/data
   <body> - showing things
   - *Basic Structure:*
```html
     <!DOCTYPE html>
     <html>
       <head>
         <title>Page Title</title>
       </head>
       <body>
         <h1>This is a Heading</h1>
         <p>This is a paragraph.</p>
       </body>
     </html>
```

2. *Basic HTML Tags*
* Tag - < > opening and closing</> tag
* Elements - < >  in between tags bettween writen things </>
* Empty Tag - tags dont have closing tages examples - br tag,img tag  
* Attribute - within tages the somthing writen to perform somthing * atr 1 = "" in h1 tags *alt = "" in img tag * width = " px" in img tag *src= "link", in img tag *target ="_blank" - open in new tag "_parrent" "_top" "_self"   

```html
    - *Headings:* <h1> to <h6> 
     <h1> this is a heading example H1 is biggest H6 is smallest</h1> 
    - *Paragraph:* <p> continues lines of para</p>
    - line break: <br> emty tag * no closing
    - *Links:* <a href="url">link text</a>
    - *Images:* <img src="image.jpg" alt="description">
    - *Lists:* 
    - Unordered: <ul><li>Item</li></ul>
    - Ordered: <ol><li>Item</li></ol>
```
3. *Attributes*
```html
   - *Global Attributes:* id, class, style
   - *Specific Attributes:* src for <img>, href for <a>, alt for <img>
```
4. *Forms and Input*

   - *Form Element:* <form>
   - *Input Types:* <input type="text">, <input type="password">, <input type="submit">
   - *Labels:* <label>


- *Form Element:*
 <form>
   - *Input Types:* <input type="text">, <input type="password">, <input type="submit">
   - *Labels:* <label>
   

#### Intermediate Level
1. *HTML5 Semantic Elements*
```html   
   - <header>, <nav>, <section>, <article>, <aside>, <footer>
```   
   - Benefits: Improved accessibility, better SEO, easier to read code.

2. *Tables*
   ```HTML
   - Structure: <table>, <tr>, <td>, <th>
   ```
   - Example:
```html
     <table>
       <tr>
         <th>Name</th>
         <th>Age</th>
       </tr>
       <tr>
         <td>John</td>
         <td>30</td>
       </tr>
     </table>
```
out put :
<table>
       <tr>
         <th>Name</th>
         <th>Age</th>
       </tr>
       <tr>
         <td>John</td>
         <td>30</td>
       </tr>
</table>


3. *Forms and Advanced Input Types*
   - New Input Types: email, tel, url, number, range, date, color
   - Form Validation: required, minlength, maxlength, pattern

4. *Multimedia Elements*
   - *Audio:* <audio src="audio.mp3" controls></audio>
   - *Video:* <video src="video.mp4" controls></video>

#### Advanced Level
1. *Responsive Web Design*
   - *Viewport Meta Tag:* <meta name="viewport" content="width=device-width, initial-scale=1.0">
   - *Media Queries:* 
     ```css
     @media (max-width: 600px) {
       body {
         background-color: lightblue;
       }
     }
     ```

2. *Canvas and SVG*
   - *Canvas:* <canvas id="myCanvas" width="200" height="100"></canvas>
   - *SVG:* <svg width="100" height="100"><circle cx="50" cy="50" r="40" stroke="black" stroke-width="3" fill="red"/></svg>

3. *Web Storage*
   - *LocalStorage:*
     ```javascript
     localStorage.setItem("key", "value");
     let value = localStorage.getItem("key");
     
   - *SessionStorage:*
     ```javascript
     sessionStorage.setItem("key", "value");
     let value = sessionStorage.getItem("key");
     ```

4. *APIs and Forms*
   - *Fetch API:*
     ```javascript
     fetch('https://api.example.com/data')
       .then(response => response.json())
       .then(data => console.log(data));
     ```

5. *Best Practices and Accessibility*
   - *Semantic HTML:* Use appropriate HTML5 tags for content.
   - *ARIA (Accessible Rich Internet Applications):*
     html
     <button aria-label="Close">X</button>
     

# Preparation for Interviews
1. *Important Concepts:*
   - HTML Syntax and Tags
   - Semantic HTML
   - Forms and Validation
   - Multimedia Elements
   - Responsive Design
   - Web Storage (LocalStorage and SessionStorage)
   - Accessibility (ARIA)

2. *Common Interview Questions:*
   - *What is the difference between HTML and HTML5?*
   answer:
   - *Explain the purpose of the doctype declaration.*
   - *How do you create a hyperlink in HTML?*
   - *What are semantic elements in HTML5?*
   - *How can you include audio and video in an HTML document?*
   - *What is the purpose of the meta viewport tag in responsive design?*
   - *Describe the difference between localStorage and sessionStorage.*
   - *How do you ensure a website is accessible?*

### Additional Resources
1. *Free Online Courses:*
   - [freeCodeCamp HTML and HTML5](https://www.freecodecamp.org/learn/responsive-web-design/basic-html-and-html5/)
   - [Codecademy HTML Course](https://www.codecademy.com/learn/learn-html)
   - [W3Schools HTML Tutorial](https://www.w3schools.com/html/)

2. *Books:*
   - HTML and CSS: Design and Build Websites by Jon Duckett
   - Learning Web Design by Jennifer Niederst Robbins

3. *Practice:*
   - Build simple web pages and gradually increase complexity.
   - Participate in coding challenges on platforms like [CodePen](https://codepen.io/), [LeetCode](https://leetcode.com/), and [HackerRank](https://www.hackerrank.com/domains/tutorials/10-days-of-html-css).
