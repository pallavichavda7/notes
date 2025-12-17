# CSS
### SHORTCUTS
* Better view  * ctrl+ k then v,
* Ctrl +K = clear console
* Cmd + k = clear console in mac
* Ctrl +R = refresh crome or console
* Ctrl +/= comment out
* /n next line print
* /p space tab print
* Ctrl + x = for the cuting the line



#### INTRODUCTION

The inventor of CSS (Cascading Style Sheets) is Håkon Wium Lie. He proposed the concept of CSS while working with Tim Berners-Lee at CERN in 1994. CSS was developed to enable the separation of document content from document presentation, including layout, colors, and fonts.

### Key Points about Håkon Wium Lie and CSS:
1. *Proposal:* Håkon Wium Lie proposed CSS on October 10, 1994, as a way to improve the presentation and styling of web documents.
   
2. *Development and Standardization:*
   - CSS was developed in collaboration with Bert Bos, who was also instrumental in shaping its early specifications.
   - The first official CSS specification (CSS1) was published by the World Wide Web Consortium (W3C) in December 1996.
   
3. *Impact on Web Design:*
   - CSS revolutionized web design by allowing developers to separate content (HTML) from presentation (CSS), making web pages more flexible and easier to maintain.
   - It enabled more sophisticated design and layout techniques compared to the limited styling options available in HTML alone.

4. *Evolution:*
   - CSS has evolved significantly over the years, with several versions being released, each introducing new features and capabilities.
   - The most recent version as of now is CSS3, which introduced numerous new properties and modules, such as flexbox, grid layout, animations, and transitions.

### Importance of CSS:
- *Design Flexibility:* Allows precise control over the layout, appearance, and styling of web pages.
- *Maintainability:* Separates content from presentation, making it easier to update and manage large websites.
- *Accessibility:* Enhances the accessibility of web content by providing multiple ways to present information.
- *Advanced Techniques:* Learn about responsive design, CSS preprocessors (like Sass and LESS), and modern layout techniques like flexbox and grid.


### Key Aspects of CSS3:
1. *Modular Structure:*
   - CSS3 is divided into several modules, each focusing on different aspects of styling and layout.
   - Examples include the CSS Grid Layout Module, CSS Flexbox Layout Module, CSS Animations, and CSS Transitions.

2. *Key Modules and Their Status:*
   - *Selectors Level 3:* Provides advanced selectors like attribute selectors, pseudo-classes, and pseudo-elements.
   - *Box Model:* Includes properties for margin, border, padding, and width.
   - *Backgrounds and Borders:* Enhances background and border capabilities with new properties like border-radius and background-size.
   - *Text Effects:* Introduces properties for text shadows, word wrapping, and text overflow.
   - *2D/3D Transformations:* Allows for rotation, scaling, and other transformations of elements.
   - *Transitions and Animations:* Provides ways to animate changes in CSS properties smoothly.
   - *Flexbox and Grid Layouts:* Offers powerful layout mechanisms for creating responsive designs.

### Continuous Development:
- The W3C regularly updates and publishes new modules and revisions. For the most current and detailed status of CSS specifications, you can refer to the [W3C CSS Current Work](https://www.w3.org/Style/CSS/current-work) page.


# CSS and CSS3:  Guide

#### SHORTCUTS
- LINK:CSS for attaching file in html
- #box1 - create box1
- .classname

#### Beginner Level

1. *Introduction to CSS*
   - *Definition:* CSS (Cascading Style Sheets) is used to style and layout web pages.
   - *Basic Syntax:*
     ```css
     selector {
       property: value;
     }
     ```
   - *Example:*
     ```css
     p {
       color: blue;
     }
     ```

2. *Adding CSS to HTML*
   - *Inline Styles:* in html tag attribute or inline of html
     ```html
     <p style="color: blue;">This is a blue paragraph.</p>
     ```
   - *Internal Styles:* in html style tag in css
     ```html
     <head>
       <style>
         p {
           color: blue;
         }
       </style>
     </head>
     ```
   - *External Stylesheet:*
     ```html
     <head>
       <link rel="stylesheet" type="text/css" href="styles.css">
     </head>
     ```
     ```css
     /* styles.css */
     p {
       color: blue;
     }
     ```

3. *Basic Selectors*
   - *Element Selector:*
     ```css
     p {
       color: red;
     }
     ```
   - *Class Selector:*
     ```css
     .myClass {
       color: green;
     }
     ```
   - *ID Selector:* for identify of same keywords
     ```css
     <div id="myId1">text</div>
     #myId {
       color: yellow;
     }
     ```
   - Boiler plate or shortcut
   pading -element k bich or border tak ka gap
   margin - element k bhr se element tak 
    *> select every thing all styles to by default
    ,>both
```css
         *{
            margin:0%;
            padding:0%;
            box-sizing:border-box;
          }
          html,body{
            width:100%;
            height:100%;
        }
```


4. *Basic Properties* 
   - *Text Properties:*
    ```css
    h1 {color: red;
     color: rgb(0,0,69);
     font-size: 16px;
     text-align: center;
     font-family:'Gill Sans';
    }
    ``` 
   - *Background Properties:*
    ```css
     background-color: lightblue;
     background-image: url('background.jpg');
    ``` 

#### Intermediate Level
1. *Box Model*
   - *Understanding the Box Model:* %- full screen 100%,half of screen - 50%
        border internal hota  h,border radius curve banega
        example circle
        ```css
        <div id="box1"></div>
        #box1{
          background-color:aqua;
          height:200px;
          width:200px;
          border-radius : 50%;
        }
        ```
    ```css
     div {
       width: 100px;
       height: 100px;
       padding: 10px;
       border: 5px solid black;
       margin: 20px;
     }
     ```

2. *Positioning*
   - *Static Positioning:*
    ```css
     div {
       position: static;
     }
    ```
   - *Relative Positioning:*
     ```css
     div {
       position: relative;
       top: 10px;
       left: 10px;
     }
     ```
   - *Absolute Positioning:*
      uske parent ko 
     ```css
     div {
       position: absolute;
       top: 50px;
       left: 50px;
     }
     ```
   - *Fixed Positioning:*
     ```css
     div {
       position: fixed;
       bottom: 0;
       right: 0;
     }
     ```


3. *Flexbox* left right lana box ko
 kisi bhi chiz ko bich me lane
   - *Basic Flexbox Container:*
     ```css
     .container {
       display: flex;
     }
     ```
   - *Align Items:* text in between heading ko center me lana
     ```css
     .container {
       display: flex;
       align-items: center;
       justify-content: center;
       <!-- justify-content: space-between; -->
       }
     ```
example
```html
<body>
<div id=box1>i am box1</div>
<div id=box2>i am box2</div>
</body>
```
```css
html,body{
  width:100%;
  height: 100%;
}
body{
  background-color:antiquewhite;
  display:flex ;
  align-items:center ;
  justify-content:center;
}
div{
  text-align:center;
  width:30%;
  height:30% ;
  font-size:xx-large;

}
#box1{
  background-color:aqua;
}
#box2{
  background-color:rgb(0,255,0);
}
```


4. *Grid Layout*
   - *Basic Grid Container:*
     ```css
     .container {
       display: grid;
       grid-template-columns: 1fr 2fr;
       grid-template-rows: auto;
     }
     ```

extra learning
- translate x asses thi move krva y se bhi hoga
```css
.box1{
    translate: 10px;
    transform:translate (-50%,-50%); 
}    
```
- rotate element
```css
#box1{
    rotate: 45 deg;
}    
```
- hover effect 
```css
#square:hover{
  background-color:black;
}
```

#### Advanced Level

1. *CSS3 Transitions and Animations*
   - *Transitions:*
     ```css
     .box {
       width: 100px;
       height: 100px;
       background-color: red;
       transition: background-color 0.5s ease;
     }
     .box:hover {
       background-color: blue;
     }
     ```
   - *Animations:*
     ```css
     @keyframes example {
       from {background-color: red;}
       to {background-color: yellow;}
     }
     .box {
       width: 100px;
       height: 100px;
       background-color: red;
       animation: example 5s infinite;
     }
     ```

2. *CSS3 Media Queries*
   - *Responsive Design:*
     ```css
     @media (max-width: 600px) {
       .container {
         background-color: lightblue;
       }
     }
     ```

3. *CSS3 Pseudo-Classes and Pseudo-Elements*
   - *Pseudo-Classes:*
     ```css
     a:hover {
       color: red;
     }
     ```
   - *Pseudo-Elements:*
     ```css
     p::before {
       content: "Note: ";
       font-weight: bold;
     }
     ```

4. *Advanced Selectors*
   - *Attribute Selectors:*
     ```css
     a[href^="https"] {
       color: green;
     }
     ```
   - *Combinators:*
     ```css
     div > p {
       color: blue;
     }
     div + p {
       color: green;
     }
     ```

### Interview Preparation

1. *Important Concepts:*
   - Understanding of the Box Model
   - Positioning Elements (static, relative, absolute, fixed)
   - Flexbox and Grid Layout
   - Media Queries for Responsive Design
   - CSS3 Transitions and Animations
   - Pseudo-Classes and Pseudo-Elements
   - Specificity and Inheritance

2. *Common Interview Questions:*
   - *What is the CSS Box Model?*
   - *Explain the difference between relative and absolute positioning.*
   - *How does flexbox work?*
   - *What are media queries, and how do you use them?*
   - *Describe CSS specificity and how it works.*
   - *What are pseudo-classes and pseudo-elements? Give examples.*
   - *How can you create animations in CSS?*

### Example Projects
1. *Responsive Portfolio Website*
   - Use Flexbox and Grid for layout.
   - Apply media queries for responsiveness.
   - Implement CSS transitions for hover effects.

2. *Interactive Form*
   - Style forms with CSS.
   - Use pseudo-classes for validation states.
   - Add transitions for smooth user experience.

3. *Animated Landing Page*
   - Utilize keyframe animations.
   - Create visually appealing transitions.
   - Ensure responsiveness with media queries.

### Additional Resources
1. *Online Tutorials:*
   - [MDN Web Docs](https://developer.mozilla.org/en-US/docs/Web/CSS)
   - [W3Schools CSS Tutorial](https://www.w3schools.com/css/)
   - [CSS-Tricks](https://css-tricks.com/)

2. *Books:*
   - CSS: The Definitive Guide by Eric A. Meyer
   - Learning Web Design by Jennifer Niederst Robbins

3. *Practice Platforms:*
   - [CodePen](https://codepen.io/)
   - [LeetCode](https://leetcode.com/)
   - [HackerRank](https://www.hackerrank.com/domains/tutorials/10-days-of-html-css)
