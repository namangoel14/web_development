# web_development
This repository describes the web development fundamental concepts which uses to build a basic web app.
# CSS: 
- CSS give style to raw HTML.
- CSS is Cascasding style sheet.
- CSS is uses to provide style our web page.
- CSS makes the responsive websites. 
- HTML is responsible for structure a website.
- CSS is responsible for design. 

- CSS Syntax: 

p {
    color: black;
}

Where, 
p, is a SELECTOR, 
color, indicates the PROPERTY of css, and
black, is VALUE of the PROPERTY.

- 3 ways to add CSS in markup(HTML):
1. Inline CSS,
2. Internal CSS, and
3. External CSS

- Inline CSS -> eg; <p style="border: 2px solid black; background-color: green;">Paragraph</p>
The CSS represent inside the html file only for the each line. 

- Internal CSS -> This type also include inside the html file but we define inside the style block in head of the html.
eg; 
<head>
<style>
    p{
        background-color: black;
        border: blue;
    }
</style>
</head>

- External CSS -> This type wants to create the external CSS file within the same path and link the file in the html file inside the head block.
eg; 
practice.css

p{
    border: 4px solid red;
    background-color: yellow;
}

practice.html
<head>
<link rel="stylesheet" href="practice.css"></link>
</head>

Where, 
rel is the relationship of the stylesheet.

- SELECTORS -> 
1. CSS selector are used to find the element whose property will be set. 
2. Selectors are used to target the html elements. 
3. Selectors makes it easy for us to easily target single/multiple HTML elements in the markup. 
4. There are some types are CSS selectors elements: 
4.1. CSS Element Selector
4.2. CSS Id Selector
4.3. CSS Class Selector
4.4. CSS grouping Selector
  
eg;

<head>
    <style>
         /* CSS ELEMENT SELECTOR  */
        p {
            /* CSS class-"paraClass" This is my CSS Class SelectorI/pd Selector */
            background-color: yellow;
            class-"paraClass" This is my CSS Class Selector}/p
            border: 4px solid black;
        #paraId{
            font-weight: bold;
            border: 3px solid red;
        }
        /* CSS Class Selector */
        .count1{
            border: 4px solid black;
            background-color: lightgray;
            padding: 30px;
            width: 600px;
            border-radius: 4px;
        }
        #firstId .firstClass {
            color: blue;
            background-color: lightblue;
            font-style: italic;
        }
    </style>
</head>
<body>
    <p>This is my element selector paragraph.</p>
    <p id="paraId">This is my ID Selector paragraph</p>
    <p class="count1">This is my CSS Class Selector</p>
    <p class="count1">This is my CSS Class Selector</p>
    <p class="count1">This is my CSS Class Selector</p>
    <p id="firstId">This is the grouping selector</p>
    <p id="firstClss">This is the Grouping selector</p>
</body>