
### **The CSS Era: Solving the Web Design Crisis**

- **Inline Styling (The Old Way):** In the early days, developers had to apply styling by adding attributes or tags within each HTML element, which made the code very messy and complex.

- **The Scalability Challenge:** If a website had 100 pages, making even a small design change (like updating a color or font) was a nightmare because every single page had to be edited manually.

- **The Solution (1996):** Web developers introduced **CSS (Cascading Style Sheets)**. Its main purpose was to separate "Content" (HTML) from "Design" (CSS), making it possible to control and maintain the entire website's look and feel from a single file.
### **Who created CSS?**

CSS was first proposed by **Håkon Wium Lie** in 1994 while he was working at CERN with Tim Berners-Lee (the creator of HTML). Later, he teamed up with **Bert Bos** the first official standard (**CSS1**), which was officially release  in  1996. working on  SSP (Streamlined Style Sheets

### Types of CSS:

**Inline CSS :**
-  Styles written directly inside an HTML tag using the `style` attribute
- Quick, one-off fixes or testing.
- `<p style="color: blue; font-size: 16px;">This is blue text.</p>`

**Internal (Embedded) CSS:**
-  Styles written inside a `<style>` tag in the `<head>` section of  HTML document.
- Styling a single web page uniquely.
- `<head><style> p { color: red; font-size: 18px; } </style> </head>`

**External CSS**:
*  Styles written in a separate `.css` file and linked to your HTML using a `<link>` tag.
-  Styling **entire websites** (industry standard because it keeps code clean and reusable).
* ***HTML (`<head>`)**:`<link rel="stylesheet" href="style.css">`
*  **style.css file** :`p { color: green; font-size: 20px; }`

### Linking HTML With CSS:

`<link rel="stylesheet" href="style.css">`

### CSS Stands For:

**Cascading**:

- It acts like a waterfall, determining which style wins when multiple rules target the same element.
- It follows a strict priority order based on code position, specificity, and rules like `!important`.(Debugging Difficult)

**Style Sheets**:

- It is a collection of styling rules that control the visual design of web pages.
- It manages properties like fonts, colors, sizes, spacing, and layouts

### **Inheritance**:
child Takes the properties of Parent 

**Automatic Inheritance (No `inherit` needed)**
 * Text properties automatically pass down from Parent to Child.
 `color`, `font-family`, `font-size`, `text-align`, `line-height`.

 **Non-Inherited Properties (Needs `inherit` keyword):**
 * Box model and layout properties do **NOT** pass down automatically.
-  `border`, `background`, `padding`, `margin`, `width`, `height`.

### Selectors:

 **Universal Selector (`*`)**:
-  Targets **EVERY SINGLE element** on the whole webpage
- **Symbol:** `*`
- `{ margin: 0; padding: 0; }`


**Element Selector (`tagname`)**:
-  Targets all elements by their HTML tag name.
- **Symbol:** Direct Tag Name (`p`, `h1`, `div`)
* `` p { color: blue; }`


**Class Selector (`.classname`)****:
 - **What it does:** Targets elements with a specific class name. **Reusable** on multiple elements.
- **Symbol:** Dot (`.`)
- .btn { background-color: green; }


 **ID Selector (`#idname`)**
-  Targets **ONE unique element** on the page. Cannot be reused.
- **Symbol:** Hash (`#`)
- #id { font-size: 24px; }


**Grouping Selector (Comma `,`)**
-  Applies the **same style** to multiple selectors at once.
- **Symbol:** Comma (`,`)

### **Combinator Selectors**
 Explains the relationship (parent, child, or sibling) between two or more selectors to target elements based on their position in the HTML structure.

 **Descendant Selector (`space`)**

-  Targets **ALL** matching elements inside a parent, no matter how deep they are nested (children, grandchildren, etc.).
- **Symbol:** A single space ( )
- `div p { color: red; }` _(Styles **every** `p` inside a `div`, even if it's inside another tag)._

 **Child Selector (`>`)**

-  Targets **ONLY direct children** (1st level down) of a parent element.
- **Symbol:** Greater than (`>`)
- `div > p { color: blue; }` _(Styles **only** `p` tags that are directly inside a `div`)._

 **Adjacent Sibling Selector (`+`)**

-  Targets **ONLY the very next element** immediately following another element at the same level.
- **Symbol:** Plus (`+`)
-  `h2 + p { font-weight: bold; }` _(Styles **only the first `p`** right after an `h2`)._

**General Sibling Selector (`~`)**

-  Targets **ALL sibling elements** following an element at the same level.
- **Symbol:** Tilde (`~`)
- :** `h2 ~ p { color: green; }` _(Styles **all `p` tags** that come after an `h2` under the same parent).
### Attribute Selector

 Targets HTML elements based on their attributes or attribute values, eliminating the need for extra classes or IDs.
-**Symbol / Syntax:** Square brackets `[ ]

- **`[disabled]`** : Targets elements that have the disabled attribute (e.g., disabled buttons).
- **`[type="text"]`** : Targets elements with an exact attribute value (e.g., text input fields).
- **`[href^="https"]`** : Targets elements whose attribute value starts with specific text (e.g., secure website links).
- **`[href$=".pdf"]`** : Targets elements whose attribute value ends with specific text (e.g., PDF download links)._
## **Pseudo-Classes**

- Targets an element based on its **state** (like when hovered, focused, or clicked).
- **Symbol:** Single colon `:`

 **:hover**

- Styles an element when the user moves their mouse over it.
- ** Example:** `button:hover { background-color: green; }`

 **:nth-child()**
 
-  Targets an element based on its position/order among siblings.
- **Example:** `li:nth-child(2) { color: red; }` _(Styles **only the 2nd item** in a list)._

**:focus** $\rightarrow$ Styles an element (like an input field or button) when it receives focus, such as when a user clicks inside a text box or navigates to it using the keyboard.
- _Example:_ `input:focus { border-color: blue; outline: none; }`

**:active** 
Styles an element at the exact moment it is being activated/pressed down by the user (the duration between the mouse click and release).
 * Example: `button:active { transform: scale(0.98); }`

### **Pseudo-Elements**

-  Targets a **specific part** of an element or inserts virtual content.
- **Symbol:** Double colon `::`

 **`::before`**

- Inserts content **before** the actual content of an element.
- ** Example:** `p::before { content: "★ "; color: gold; }`

**`::after`**

-  Inserts content **after** the actual content of an element.
- ** Example:** `a::after { content: " ↗"; }`

**`::selection`**  
Styles the text that is highlighted/selected by the user.
* _Example:_ `p::selection { background-color: yellow; }`


### Summary of CSS Selectors

- **Universal Selector (`*`)** Targets every element on the webpage; commonly used for resetting default margin and padding (`margin: 0; padding: 0;`).

- **Element Selector (`p`, `h1`)**  Targets all HTML elements with the specified tag name across the page.

- **Class Selector (`.classname`)**  Targets multiple elements with the same class attribute for reusable styling.

- **ID Selector (`#idname`)** Targets a single, unique element on the webpage (used only once per page).

- **Grouping Selector (`,`)** Applies the same style rules to multiple selectors at once 

- **Attribute Selector (`[attr]`)**  Targets elements based on the presence or specific value of an HTML attribute (e.g., `[type="text"]`).

- **Combinator Selector** Defines the structural relationship (parent, child, or sibling) between two or more selectors.

- **Descendant Selector (`space`)**  Targets all matching elements nested inside a parent element (children, grandchildren, etc.).

- **Direct Child Selector (`>`)** Targets only the immediate, 1st-level children directly inside a parent element.

- **Adjacent Sibling Selector (`+`)** Targets only the single matching element that comes immediately after a specified element at the same level.

- **General Sibling Selector (`~`)**  Targets all matching sibling elements that follow a specified element at the same level.

- **Pseudo-Class (`:`)**  Targets an element based on its dynamic state or user interaction (e.g., `:hover`, `:focus`, `:active`, `:nth-child()`).

- **`:hover`**  Styles an element when the user moves their mouse cursor over it.

- **`:focus`**  Styles an element when it receives user focus, such as clicking into an input field or tab-navigating to it.

- **`:active`** Styles an element at the exact moment it is being clicked or held down by the user.

- **`:nth-child()`** Targets an element based on its specific numerical position or order among its siblings under the same parent.

- **Pseudo-Element (`::`)** Targets a specific part of an element or inserts virtual content without changing HTML structure (requires `content: ""` for `::before` and `::after`).

- **`::before`** Inserts decorative or functional virtual content right before the actual content of an element.

- **`::after`**  Inserts decorative or functional virtual content right after the actual content of an element.

- **`::selection`**  Styles the portion of text that is currently highlighted/selected by the user.

### Rules of Specificity:

**Rule 1: The Point System (Hierarchy)**

The selector with the highest score wins the style conflict

- **Inline Style (`style=""`)** = 1000 points _(Strongest)_
- **ID (`#id`)** = 100 points
- **Class / Pseudo-Class / Attribute (`.class`, `:hover`, `[attr]`)** = 10 points
- **Element (`p`, `h1`)** = 1 point
- **Universal Selector (`*`)** = 0 points _(Weakest)_

*  **Rule 2: Add Up the Scores**
More specific combinations win. For example, `div .card` ($1 + 10 = 11$ points) beats a single `.card` ($10$ points).

- **Rule 3: Tie-Breaker (Last One Wins)**
If two selectors have the **same score**, the style written **lower down in the CSS file** wins. (Cascade Rule).

- **Rule 4: (`!important`)**
Adding `!important` to a property overrides all specificity scores, no matter how high they are.

# **CSS Box Model **

 Every element on a webpage is shaped like a rectangular box with four layers.
- **Content** : The inside part of the box that holds  text, images, or buttons.
- **Padding** : The space inside the box between the content and the border.
**Spacing**
- **Border** : The outline or line that goes around the padding and content.
- **Margin** : The empty space outside the border that pushes other elements away.


- **Clockwise Rule** : Four values always work in order: Top $\rightarrow$ Right $\rightarrow$ Bottom $\rightarrow$ Left.

**Box sizing**
It controls how the total width and height of an element are calculated.

- **`border-box` Behavior:** The total box size stays fixed. Adding padding or border adjusts the space inside the box, so the outer size does not grow. **best practice**

- **`content-box` Behavior:** Adding padding or border increases (expands) the total box size, which can break the layout.(inspect)

### **CSS Units (Sizing)**

- **`px` (Pixel):** A fixed unit that always stays the exact same size regardless of the screen.
- **`%` (Percentage):** A relative unit that changes its size based on the width of its parent container.
- **`rem` (Root EM):** A relative unit based on the root (`<html>`) font size, making it the best choice for responsive design.
- **`em`:** A relative unit based on the font size of its immediate parent element.
### Responsive 
Font Size = 1rem, 2.5rem 
Padding = 1rem, 2rem
Margin = 1rem, 0.5rem 
Width = 50%, 100% 
Height = 100%, 50%
 **Fixed**
Border = 1px, 2px 
Box-shadow = 2px 2px 8px
Border-radius = 4px, 8px

### **Colors**

- **HEX Code (`#ff0000`):** A 6-character code used for r picking exact colors in web design.
- **RGB / RGBA:** A color format using Red, Green, and Blue values, where the `a` (alpha) controls transparency.
- **HSL / HSLA** :  (Hue, Saturation, Lightness)

### **Fonts & Typography**
Typography (Text Specific) is the  style of arranging text on a webpage to make it clear, readable, and visually appealing.

- **`font-family`:** Sets the specific design or style of the text (like Arial or Roboto).
- **`font-weight`:** Controls the thickness or boldness of the text.
- **`line-height`:** Controls the vertical space between lines of text.
### CSS Display Property:
 
 **Display: block**
Takes up the full width of the line and pushes the next element to a new line below it. (section up /down)
- Example: `<div>`, `<p>`, `<h1>`

 **Display: inline**
Stays on the same line and takes only as much space as its text, but ignores width and height (Styles inside text)
- Example: `<span>`, `<a>`, `<b>`

**Display: inline-block**
Stays on the same line with other elements, but allows you to set custom width, height, and padding. (cards)
- Example: Buttons, Cards, Navigation 


### Margin: auto
We use `margin: auto` to center a block element horizontally on a webpage by balancing the left and right spacing equally.

## Margin: 0
We use `margin: 0` when we do not want any space outside the border. If vertical spacing is needed, we can specify top and bottom margins using units like `px` or `rem`, following the standard `(top, right, bottom, left)` clockwise order.

## Best Practice
The best practice for centering a block element is to use `auto` for the left and right margins, while using explicit units (like `px` or `rem`) for the top and bottom margins.
These auto-margin rules apply **only to block elements** (`display: block`). They do **not** work directly on `inline` or `inline-block` elements.

### Week 5

# Flexbox 

## 1. CSS Flexbox (One-Dimensional)

Flexbox is designed for **one-dimensional** layouts. it handles content either as a **row** or as a **column** at a time. It is ideal for aligning items within a container, distributing space, and adjusting sizes dynamically.

*   **When to use:** Use Flexbox when we need to align items in a single direction (e.g., a navbar, a horizontal list of cards, or centering an item inside a container).

 **Properties:**
*   **Container (Parent) Properties:** `display: flex`, `justify-content`, `align-items``flex wrap`, `flex-direction`.
*   **Items (Children) Properties:** `flex-grow`, `flex-shrink`, `flex-basis`, `order`.

### Flexbox Axes:

**Main Axes**:
* In Flexbox, we have two main axes: the **main axis** and the **cross axis**.
* If we have displayed blocks horizontally in a row, our main axis runs from **left to right**.
* If we have set it in a column vertically, our main axis runs from **top to bottom**.

**Cross Axes:**
* The cross axis is the opposite, like perpendicular, to the main axis. 
* If the main axis is left to right, then the cross axis is vertical. 
* If the main axis is top to bottom, then the cross axis is vertical.
**Flex Direction:** Rows ,Coloumn
### Container vs. Item Properties 

 **Container Properties (Parent):** 
* The container acts as the parent. 
* Changes applied here affect the entire box and all items inside it. If we apply a background or border to the container, it applies to the whole box as a single unit. 
* Container properties include: `justify-content`, `align-items`, `flex-wrap`, and `gap`. 

**Item Properties (Child):**
* The items act as children. If we apply a border to an item, it has its own separate box.
* Item properties include: `flex-grow`, `flex-shrink`, `order`  and  `flex-basis`.

### Justify content: ( works for Main Axes)

**Types / Values of `justify-content`:** (container)

* **`flex-start`:** Aligns items to the very start of the main axis (on the left side if the direction is row). 
   |ABC       |
   
* **`flex-end`:** Aligns items to the end of the main axis (on the right side if the direction is row).
   |     ABC|
   
* **`center`:** Centers all the elements/boxes together in the middle of the container.
   |    ABC   |
  
* **`space-between`:** Places the outer blocks stuck to the edges (no extra space on the outer edges), and distributes equal space only between the inner blocks.
   |A  B  C|
   
* **`space-around`:** Gives equal space around every box (so there is a little bit of space on the outer edges as well, and double the space between adjacent items). 
   |  A  B  C  |
   
* **`space-evenly`:** Distributes completely equal/even space around every box and between all items, including the outer edges.
   | A B C |
### Align Items: ( Works on Cross axes):

 * **`stretch` (Default):** Used to adjust and stretch the height of the boxes along the cross axis so they match.
 * **`flex-start`:** Moves and sticks the boxes to the top edge (cross axis start). 
 * **`flex-end`:** Shifts and sticks the boxes to the bottom edge (cross axis end).
 * **`center`:** Aligns the boxes right in the middle according to the cross axis.
 * **`baseline`:** Used when text inside boxes is uneven (one word higher, another lower). It aligns the text so that all words sit perfectly on a straight line.


### **`Flex-wrap`:
   
   Used when we have multiple boxes and they start overflowing or going outside the screen/container width. It keeps items contained by shifting them to the next line when space runs out. 
 **Main Values:** 
   * **`nowrap` (Default):** Keeps all items in a single line, even if they shrink or overflow the container. 
   * **`wrap`:** Automatically moves overflowing items to the next line.
   * **`wrap-reverse`:** Wraps the items, but in a reverse order (the wrapping behavior or row stacking is flipped).

### **` Flex Gap`:**

 Used to create a specific, equal space (gap) between flex items without needing to use margins manually.
 *  **`gap`:** Applies spacing equally to both rows and columns at the same time (e.g., `gap: 20px;`
 * **`row-gap`:** Applies spacing only between the rows. 
 * **`column-gap`:** Applies spacing only between the columns.

### **Flex Item Properties :** 

* **`flex-grow`:**  Used to adjust and fill the remaining/extra empty space inside the container by allowing the items to expand proportionally.
* **`flex-shrink`:** Decides how much the boxes can shrink and squeeze when the screen size gets smaller, preventing them from overflowing or breaking the layout. 
* **`flex-basis`:**  Sets the initial/base size (width or height) of a flex item *before* the `flex-grow` and `flex-shrink` properties are applied to it.
* **`order`:**  Used to change the visual sequence or arrangement of the items. By giving specific order numbers (e.g., setting a box to a higher or lower order number), you can control which box appears first or last regardless of HTML source order.
  
# CSS  Grid Layout :

 A **two-dimensional** layout system  because It handles both rows and columns at the same time  Easily manage and adjust multiple rows and columns together.
` display: grid`

### Columns & fr Unit 

**`grid-template-columns`**: Used to define the number and width of columns in a grid. 

- **`fr` (Fractional Unit)**: Distributes the available space evenly among columns. 
- *Example*: `grid-template-columns: 1fr 1fr 1fr;` creates 3 equal-width columns. 
- **`minmax()` Function**: Sets a minimum and maximum size for grid columns/rows, making layouts responsive 

# CSS Grid `fr`  Unit

## What is `fr`?
* **`fr`** stands for **Fraction**. 
* It is a special measuring tool made just for CSS Grid to share screen space nicely.

##  Use  of `fr`?
It makes website **responsive and flexible automatically**

* **No Fixed Headaches:** If you we use pixels (`px`),  boxes stay the exact same size, even if someone opens  site on a tiny phone screen. That breaks  layout.
* **Smart Adjusting:** `fr` looks at the screen size and shares the space fairly. If the screen shrinks, the boxes shrink with it.


# `grid-template-columns`

### How Columns are Counted
* The **number of columns** is decided by how many times you write the value or use `repeat()`.
* The **width of each column** is decided by units like `fr` (Fraction).

###  Use  Of`repeat()`
* Use `repeat()` when you want **multiple columns of the exact same width**.
* **Example:** `grid-template-columns: repeat(4, 1fr);` creates 4 equal columns.

### Use 0f  Custom Values (No `repeat`)

* Use individual values when **each column needs a different size**.
* **Example:** `grid-template-columns: 1fr 2fr 3fr;` creates 3 columns where each has a different custom width.
###  Mixing `repeat()`

* You can combine custom sizes and `repeat()` in one line
* **Example:** `grid-template-columns: 2fr repeat(4, 1fr) 7fr;`

### Columns vs Rows (The Core Difference)
* **`grid-template-columns`:** Controls the **Width** (left to right space).
* **`grid-template-rows`:** Controls the **Height** (top to bottom space).

## Setting Rows (`grid-template-rows`)
* Just like columns, we can define row heights using pixels, percentages, or `fr`.

# `fr` is Best for Columns, but Rarely for Rows

### `fr` works great for Columns (Width)
* Columns move **left to right** (Width).
* Screen widths vary across devices (mobile, laptop, desktop).
* Using `fr` makes columns **fully responsive**, automatically adjusting as the screen size changes.

### we don't always use `fr` for Rows (Height)

* Rows move **top to bottom** (Height).
* Web pages grow vertically based on **content** (text, images), and users scroll through them.
* **The Risk of `fr` on Rows:** If you force rows to use strict `fr` units, the layout tries to squeeze everything into a fixed screen height. If your content is too long, **it will overflow and spill out of the boxes**, ruining the design.

### Best Practice for Rows
* Let rows adjust automatically to their content (`auto`), or use minimum heights (`min-height`) rather than strict `fr` units, unless we  are building a single-screen dashboard or full-page layout that shouldn't scroll.

# CSS Grid: Container vs. Specific Box Rules

### Container Properties (`grid-template-*`)
* **Applied to:** The **Parent Container**.
* **Purpose:** Creates the overall layout blueprint (defines total columns and rows).

### Item Properties (`grid-column-*` / `grid-row-*`)
* **Applied to:** A **Specific Box (Item)**.
* **Purpose:** Controls where an individual box starts and ends across the grid lines.


# @ Media Queries
 
* **The Problem:** When we code a website on laptop, it looks great. But if someone opens it on  mobile phone or a huge desktop monitor, the layout can break.
* **The Solution:** **Media Queries*  
* They let us  apply different CSS styles depending on the device screen size. 

### Why do we use them?
* To build **Responsive Web Design** (RWD).
* To make sure  site looks neat, clean, and accurate whether it's opened on a mobile phone, tablet, laptop, or desktop
* we use it on parent container,
