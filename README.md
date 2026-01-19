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

- Fonts in CSS
In CSS, We have 2 types of fonts: 
1. Web Safe Fonts
2. Web Fonts

- Web Safe Fonts are those fonts which are inbuild in our operating system and we don't have to use from external/3rd partywebsites.
Like: 

<style>
    p {
        font-family: arial;
    }
</style>

So over here the font-family has arial which is inbuild in our operatin system and we can use easily. 

- Web Fonts are those fonts if we want to use some other styles in fonts then we have to use external websites link to include in our html structure to apply them. 
Like: We can use google fonts sites to choose any of them and copy the hyperlink and font-family value to include in our structure/project. 
<head>
    <link rel="stylesheet" href="googleFonts.com/oswaldfont"></link>
    <style>
        p{
            font-family: "oswald";
        }
    </style>
</head>

Now in CSS we have several font properties to apply to make design more responsive: 
eg; 
1. line-height -> it use to provide the certain height of that font in webpage.
2. font-size -> it adjust the size of the font. 
3. font-weight -> it give the boldness as per your need. 
4. font-style - > it provide the style to the font like italic.

- Colors in CSS
In CSS there are 3 types are representation of colors.
1. eg; 
<style>p{color: red;}</style>

2. rgb color.
rgb means Red Green Blue (RGB)

syntax -> rgb(0,0,0,0)
       -> rgb(0-255, 0-255, 0-255, 0-1);
Red -> 0-255 range of colors     
Green -> 0-255 range of colors
Blue -> 0-255 range of colors
Transparency -> 0-1

3. Hex color: 
eg; <style>p{color: #ffffff}</style>
means, ff ff ff
ff, ff, ff every hex values has its individual color value, and after merge together it form one color.

- Background and border in CSS

In border we have some property: 
1. border-width
2. border-style
3. border-color

we can also merge them in single border property: 
like: 

border: 4px solid red;

4px is border-width;
solid is border-style;
red is border-color.

4. border-radius Property -> to curv the border corners/edges. 

like: border-radius: 4px;

5. border-top
6. border-bottom
7. border-left
8. border-right

- border-top: 4px solid black; -> property is provide the value to top border line only.
- border-bottom: 4px solid red; -> property is provide the value to bottom border line only.
- border-right: 4px solid green; -> property is provide the value to right border line only.
- border-left: 4px solid yellow; -> property is provide the value to left border line only.

9. border-top-radius
10. border-bottom-radius
11. border-right-bottom
12. border-left-bottom

- border-top-right-radius: 4px;  -> property is provide the curv to top-right of the corner of the box.
- border-top-left-radius: 4px;  -> property is provide the curv to top-left of the corner of the box.
- border-bottom-left-radius: 4px;  -> property is provide the curv to bottom-right of the corner of the box.
- border-bottom-right-radius: 4px;  -> property is provide the curv to bottom-left of the corner of the box.

- If we want to add the image in the background we can use below property: 
1. background-image: url("")

In url() -> we can also provide path image which is stored in our directory and external image as well. 

For internal image -> url("/path/of/the/image")
For external Image -> utl("/https:google.com/images")

- When we insert the image we will see the repeatness in the background we handle this repeatness with some css property: 

1. background-repeat: repeat-x;
2. background-repeat: repeat-y;
3. background-repeat: no-repeat;

- With background-repeat: repeat-x; -> it will repeat only from x-axis not from y-axis. 
- With background-repeat: repeat-y; -> it will repeat only from y-axis not from x-axis. 
- With background-repeat: no-repeat; -> it will not repeat from both the axis.

- We can also adjust the position of the image as well with some CSS property. 

1. background-position: center center;
2. background-position: top center;
3. background-position: top left;
4. background-position: top right;
5. background-position: bottom center;
6. background-position: bottom left;
7. background-position: bottom right;

- background-position: center center; -> property adjust the image at the center of the box means it will divide the same same from the top, bottom, left and right.
- background-position: top center; -> property adjust image at the top center of the box.
- background-position: top right; -> property adjust image at the top right of the box.
- background-position: top left; -> property adjust image at the top left of the box.
- background-position: bottom center; -> property adjust image at the bottom center of the box.
- background-position: bottom left; -> property adjust image at the bottom left of the box.
- background-position: bottom right; -> property adjust image at the bottom right of the box.

- Box model -> content, padding, border and margin. 

Css box model define how an element size is calculated with the content, padding, border and margin. 

So we have CSS BOX MODEL: 

First layer is MARGIN, 
Second layer is BORDER, 
Third layer is PADDING, and 
at the end there is CONTENT.

eg: 
padding, margin and border
<style>
    p{
        border: 4px solid lightgray;
        padding: 10px;
        margin: 10px;
    }
</style>

where, 
border: 4px solid lightgray; -> 4px is border-width, solid is border-style and lightgray is border-color.
padding: 10px; -> means from left, right, top and bottom all the side are 10px value. 
margin: 10px; -> means from left, right, top and bottom all the side are 10px value.

We can also provide with individual values of individual side in padding and margin as well. 

eg; 
padding-left: 10px;
padding-right: 30px;
padding-top: 5px;
padding-bottom: 50px;

margin-left: 10px;
margin-right: 30px;
margin-top: 5px;
margin-bottom: 50px;

- We also provide the all these in one property as well. 

syntax: 
padding: top right bottom left;
margin: top right bottom left;

eg; 

padding: 10px 30px 10px 30px;
margin: 10px 30px 10px 30px;

- If we want to provide same top/bottom and left/right values in a single property we can use like below: 

syntax: 

padding: x(top/bottom) y(left/right);
margin: x(top/bottom) y(left/right);

eg; 

padding: 10px 30px;
margin: 10px 30px;

- Sometimes when we  adjusts the padding and margin but somehow the box width and size gets changed it get unstable and not fixed. So in this case we can use box-sizing property to fix the current width and height of the box. 

eg; 

box-sizing: border-box;

- We have the universal selector which we can make some porperty universally applicable for other selectors and properties. 

We can use like below: 

<style>
    /* UNIVERSAL SELECTOR */
    *{
        box-sizing: border-box;
    }
</style>

- We have body selector as well to change anything inside the body. 

eg: 
<style>
    *{
        box-sizing: border-box;
    }
    /* BODY SELECTOR */
    body{
        background-color: blue;
    }
</style>

-CSS Float and Clear property.

- Float is the CSS property which adjusts the box or any content of the web page. Like;

- float: left -> it shifted the box towards the left side. 
- float: right ->it shifted the box towards the rigth side.

- overlapping of content/ boxes, to resolve this we can use clear property in CSS. 

- If we want to clear the content from the left we can use: 

<style>
    p{
        clear: left;
    }
</style>
- If we want to clear the content from the right we can use: 

<style>
    p{
        clear: right;
    }
</style>

- If we want to remove the overlapping/clear the content from the both the sides we can use below property in clear. 

<style>
    p{
        clear: both
    }
</style>

- We can also align the text as well inside the box. 
Like: 
<style>
    p{
        text-align: left;
    }
</style>
<style>
    p{
        text-align: right;
    }
</style>
<style>
    p{
        text-align: center;
    }
</style>
<style>
    p{
        text-align: justify;
    }
</style>

Where, 

text-align: left; -> This  align the text of the box towards the left side. 
text-align: right; -> This  align the text of the box towards the right side. 
text-align: center; -> This  align the text of the box towards the center side. 
text-align: justify; -> This property distribute left and right sides in equal space. 


