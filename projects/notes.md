# FreeCodeCamp Notes
## 2025-10-06
### CSS Specificity
The universal selector * is often used to apply a style to all elements on the page.  

`*  {
     margin: 0;
     padding: 0;
   }`    

This can help to remove default settings from browsers.  

**Type selectors** specificity value is `(0, 0, 0, 1)`. 

The `!important` keyword in CSS is used to give a style rule the highest priority, allowing it to override
any other declarations for a property.

## 2025-10-06

`.para {
    background-color: black !important;
    color: white !important;
}`  

The `!important` keyword is used after the CSS value and before the semicolon.  

#### Cascade Algorithm at a High Level
The process begins with **relevance**.
This process matches selectors and considering media queries that might be in effect.  
Next, the algorithm considers **origin and importance**.
Different sources: the browser's default styles(user-agent), styles set by the user, and styles written by the author(you).  
Then it evaluates the importance of each rule, giving priority to rules marked with `!important`, which override other rules regardless of their source.  
1. relevance
2. origin and importance
3. specificity
4. order of appearance

## 2025-10-11
### CSS Specificity (Continued)

`<div style="color:blue;">This is the parent element.<p>This is the child element inheriting the color.</p></div>`  

#### Different Types of CSS Combinators
- Descendant Combinator `ul li {background-color: yellow;}`
    - This example will target all `li` items inside `ul` elements.
- Child Combinator (`>`): is used to select elements that are direct children of a specified parent element.
    - This example will target all `p` elements that are direct children of the `container` class.
    - `.container > p {background-color: black;color:white;}` 


