Hyper Text Mark Up Language

### History

### 1.The Pre-Web Era & The Problem of Data Sharing

- **Floppy Disks:** Early users relied on physical floppy disks to transfer data between computers, but they had very limited storage capacity.
- **The Research Challenge:** Scientists and researchers could not  share large research papers and documents.
- **The Solution (1989–1991):** Tim Berners Lee created a development space and system to share files globally without storage limitations which led  to the development of **HTML** (Hyper Text Markup Language).


### Evolution of Word Wide Web 

-   Web 1.0: a**Viewer / Reader** (only consume  content).
- **Web 2.0:**  **Creator / Contributor** (generate and share content on platforms).
- **Web 3.0:**  **Owner / Controller** (own your data, digital identity, and assets).

### 2. Core Technologies Introduced
www (world wide web )
- **HTML (Hyper Text Markup Language):** Structured the content and allowed text to link to other pages.
- **URL (Uniform Resource Locator):** Provided a specific address to locate. 
- **HTTP (Hyper Text Transfer Protocol):** set of protocols to transfer data over the web.
 HTTP not secure
 HTTPS secure 

### 3. Client-Server Interaction

- **Client:** The user's device or browser (e.g when we search for something on Google , browser is the client sending the request).
- **Server:** The remote computer and database hosting the website's files and data.

  **How It Works:**
  
*  **Client** sends a request for a specific resource.
*  **Server** searches its system and database for that requested data.
* The **Server** sends the matching data back to the **Client**, displaying the results on your screen.

### 4.Webpage vs  Website

- **Webpage:** A single individual page on the internet.
- **Website:** A collection of multiple webpages linked together under a single domain name.
- **Web Browser:** A software application used to access and view websites and webpages on the internet.

**Example**
Website =  whole book.
Webpages =  individual pages inside that book.
Domain Name =  Title of the book.

### 5.Uses of HTML:
HTML is primarily used to build and structure webpages and websites
 
* ***Modern Uses (Beyond Websites):**
* ***Email Templates:** Formatting and designing professional emails.
* **App Interfaces:** Creating layouts for modern mobile app.

###  6. Three Pillars of Web Development:

* ***HTML (The Structure):** Defines  what content is on the page (headings, paragraphs, images).
 * ***CSS (The Design / Styling):** Defines how the page looks (colors, fonts, layouts).
 * ***JavaScript (The Interactivity ):** Defines  how the page behaves and responds to user actions (animations, buttons, logic) how the button will work.


### 7.Evolution of HTML :

**1991 (HTML 1.0):** Created by Tim Berners-Lee with just 18 basic text tags.
**1995 (HTML 2.0):**  introduced forms and tables.
**1997** **(HTML 3.2):** added colors and layouts.
**1999 (HTML 4.01):** A major version that separated structure from design using CSS.
**2000s (XHTML)**:Stricker syntax
**2014–Present (HTML5):** The modern standard added built in multimedia (`<video>`, `<audio>`) and mobile support.
 
 
### 8. Introduction to HTML:

**Stands for:** Hyper text markup language.
**Hyper text**: Text  with links that are Clickable  
**Mark up** : using special tag so that the browser know the meaning of the content
* Not a programming language use set of rules to make website.
* Describes the structure of a Web page.
* wide browser support(fire fox ,edge ,safari ,google)
* Easy to write Human Readable code


### 9.Structure of HTML:
<!DOCTYPE html>  
<html>  
<body>  
  
<h1>  Heading</h1>  
<p>paragraph.</p>  
  
  </body>  
</html>

<!DOCTYPE html> Tells the browser its a latest version
<html>The big box that holds everything
<head> The hidden brain (browser tab title, style link ,users can't see this).
<body> The visible screen (everything users actually see and click: text, pictures, buttons).

### HTML Elements
 An HTML element is a piece of code used to tell the web browser how to display content like text, images, or buttons on a website. 
 **Basic Structure **:
 Most HTML elements have an opening tag, content, and a closing tag: ```html <tagname>Hello World</tagname>
 - `href`: Sets the link URL in `<a>`.
- `src`: Sets the image path in `<img>`.
- `width` & `height`: Sets image size in pixels.
- `alt`: Gives alternate text if an image fails to load.
- `style`: Adds inline styles like color or size.
- `lang`: Declares the webpage language in `<html>`.

 
**Types of HTML Elements**:
 * Empty HTML Elements: do not have a closing tag.
 * Nested HTML Elements: an element inside another HTML element
 
 **Example:**
The `<html>` element is the parent container for the whole page.
Inside it, the `<body>` element is nested.
Inside the body, the `<h1>` and `<p>` elements are nested.

### HTML Attribute:
They provide additional information about HTML elements.
- `href`: Sets the link URL in `<a>`.
- `src`: Sets the image path in `<img>`.
- `width` & `height`: Sets image size in pixels.
- `alt`: Gives alternate text if an image fails to load.
- `lang`: Declares the webpage language in `<html>`.

### HTML Headings:
-HTML headings are defined with the `<h1>` to `<h6>` tags and are used as titles or subtitles on a webpage.
-`<h1>` defines the most important heading, while `<h6>` defines the least important heading.

###  HTML Paragraphs
- Defined with the `<p>` tag.
- Using `<br>` tag  for line break without starting a new paragraph. 
- **`<b>` / `<strong>`**: Defines bold text (strong).
- **`<i>` / `<em>`**: Defines italic text (em).
- **`<mark>`**: Defines marked or highlighted text.
- **`<small>`**: Defines smaller text

### HTML Quotation and Citation Elements

Used for short quotes, long quotes, and abbreviations:

- **`<q>`**: Defines a short quotation (browsers automatically insert quotation marks around it).
- **`<blockquote>`**: Defines a section quoted from another source.
- **`<abbr>`**: Defines an abbreviation  with a full description.
- **`<address>`**: Defines contact information for the document or article author, usually shown in italic.
- **`<cite>`**: Defines the title of a creative work, usually displayed in italic.

### HTML Comments

- Used to explain code.
- Not displayed by the browser.
- **Syntax:** `<!-- Write your comments here -->`

## HTML Styles

-  The HTML `style` attribute is used to add styles to an element, such as color, font size, and more.
- `<tagname style="property:value;">`

### HTML Links

- Defined using the `<a>` tag.
- The `href` attribute specifies the destination URL of the link.
- Links can open in the same tab or a new window using `target="_blank"`.
- `_self`: Opens the document in the exact same window/tab where it was clicked.

###  HTML Images

- Embedded using the `<img>` tag.
- The `src` attribute specifies the path to the image, and the `alt` attribute provides alternative text.
- The `width` and `height` attributes define the size of the image in pixels.

###  HTML Favicon

- A small icon displayed next to the page title in the browser tab.
- Added inside the `<head>` section using a `<link>` tag with `rel="icon"`.

###  HTML Page Title

- Defined using the `<title>` element inside the `<head>` section.
- Specifies the title of the web page shown in the browser's title bar or tab.

###  HTML Tables

- Used to display data in rows and columns.
- Core tags include `<table>` (wrapper), `<tr>` (table row), `<th>` (table header), and `<td>` (table data/cell).

### HTML Lists

- Used to group related items together.
- **Unordered List (`<ul>`):** Creates bulleted lists using `<li>` items.
- **Ordered List (`<ol>`):** Creates numbered lists using `<li>` items.
- ** Description list`**`<dl>` tag defines the description list`<dt>` tag defines the term name, and the `<dd>` tag describes each term.

###  HTML Block & Inline

- **Block Elements:** Always start on a new line and take up the full available width (e.g., `<div>`, `<p>`, `<h1>`).
- **Inline Elements:** Do not start on a new line and only take up as much width as necessary (e.g., `<span>`, `<a>`, `<img>`).

###  HTML Div

- Defined with the `<div>` tag, which is a block-level container.
- Used primarily as a section  to group other HTML elements together for styling or layout purposes.


###  HTML Classes

Can be used on multiple elements. You use a class when you want to apply the same styling or behavior to several different elements on a page (targeted in CSS using a dot `.` like `.my-class`).


###  HTML Id

Must be completely **unique**. An ID is used for only **one single element** per page, and it cannot be shared with any other element (targeted in CSS using a hash `#` like `#my-id`).

###  HTML Buttons
 Created using the `<button>` tag.
Used for clickable buttons inside forms or anywhere.

- `type="button"`  A normal clickable button (does nothing by default)
- `type="submit"` Submits a form
- `type="reset"`  Resets all form fields

### HTML Iframe 

- **Syntax:** Written as `<iframe src="url" title="description"></iframe>` to embed another document inside  a webpage.
- Embedding **Google Maps**.
- Embedding **YouTube or  videos**.
- **Height & Width:** Set using attributes (e.g., `height="200"` and `width="300"`) or via CSS.
 - **Syntax:** `<iframe src="URL" title="description"></iframe>`
- **Dimensions:** Controlled via `width` and `height` attributes or CSS.
- **Styling:** Borders can be removed using CSS (`style="border:none;"`).
- **Performance/Security:** Attributes like `loading="lazy"` (for faster page loads) and `sandbox` (for extra security)  `allow="fullscreen"`  `allow="autoplay"`are often included.


### HTML File Paths:
It tells the browser where to find a file (image, stylesheet ) in website's folders.
### **Types of File Path**
**Relative File Paths (Best Practice)**
Points to a file based on your **current page location**.
- **Same Folder:** `<img src="picture.jpg">` — File is right here in the same folder.
- **Subfolder:** `<img src="images/picture.jpg">` — File is inside an `images` folder.\

** Absolute File Path**
Uses the **full web address (URL)** to link to a file.
- **Example:** `<img src="[https://www.website.com/images/picture.jpg](https://www.website.com/images/...)">

 ### Metadata  of an HTML document:
 Meta tags are used to provide background information about the webpage to browsers and search engines.
<meta charset="UTF-8">  * UTF-8 Character Set
<meta name="description" content="Free Web tutorials">* Description Tag
<meta name="keywords" content="HTML, CSS, JavaScript">  * Keywords Tag
<meta name="author" content="John Doe">*  Author Tag
<meta name="viewport" content="width=device-width, initial-scale=1.0">* Viewport Tag


###HTML Layout Elements:
- `<header>` - Defines a header for a document or a section
- `<nav>` - Defines a set of navigation links
- `<section>` - Defines a section in a document
- `<article>` - Defines independent, self-contained content
- `<aside>` - Defines content aside from the content (like a sidebar)
- `<footer>` - Defines a footer for a document or a section

## Semantic Elements

 **Accessibility:** Screen readers use these tags to help visually impaired users navigate.
  **SEO:** Search engines (like Google) better understand the structure and hierarchy of your content.
 **Developer Experience:** It makes the code much easier for other developers to read and maintain.
 
**Semantic Elements (Meaningful):** Elements like `<header>`, `<nav>`, `<article>`, and `<section>` clearly describe their meaning to both the **browser** and the **user**

**Non-Semantic Elements (No Meaning):** Elements like `<div>` and `<span>` tell nothing about their content. They are just generic containers used purely for styling or layout structuring without giving any hints to the browser or search engines about what is inside them.

### HTML Entities
It is a code used to display reserved characters (like `<` or `>`) or special symbols (like `©`) that cannot be easily typed or used directly in HTML code.
**Structure**
- Always starts with an ampersand (`&`) and ends with a semicolon (`;`)
- **Copyright symbol:** `&copy;`
- **Ampersand:** `&amp;`
- **Greater than:** `&gt;`
- **Less than:** `&lt;`

### HTML vs XHTML
 XHTML(Extensible Hyper Text Mark up Language) is a stricter, more formal version of HTML that follows XML rules.
 **Main Differences:**

 **Strictness:**
- HTML: Is flexible .it doesn't break if there  minor coding mistakes.
- XHTML: Is very strict; even a small error will cause the page to show an error and fail to load.
**Closing Tags:**
- HTML: Some tags don't need to be closed (e.g., `<br>`, `<img>`).
- XHTML Every single tag **must** be closed. Self-closing tags need a slash at the end (e.g., `<br />`, `<img src="..." />`).
 **Lowercase Rule:**
- HTML: Tags can be written in uppercase or lowercase (e.g., `<P>` or `<p>`).
- XHTML: All tags and attributes **must** be in lowercase.

### HTML Forms
- Used to collect user input (like login, signup, or feedback).
** Form Attributes**
- **`action`**: Decides where the form data goes for processing (e.g., a server file).
- **`method`**: How data is sent._GET_: Shows data in the URL (not secure).POST_: Hides data (secure).
- **`target`**: Where to open the response 

**HTML Form Elements**
- **`<input>`**: The main element for text fields, buttons, etc.
- **`<label>`**: Text title for an input (helps accessibility).
- **`<select>` & `<option>`**: Creates a drop-down list.
- **`<textarea>`**: A big box for long text paragraphs.
- **`<button>`**: A clickable button.

**  Input Types**

- `type="password"`: Hides entered characters (dots/stars).
- `type="submit"`: Sends the form.
- `type="reset"`: Clears form fields.
- `type="radio"`: Select **only one** option from a group.
- `type="checkbox"`: Select **multiple** options.

 **Input Attributes**

- **`value`**: Sets a default text inside the input.
- **`readonly`**: Can read text, but cannot change it.
- **`disabled`**: Locks the input completely (data is not sent).
- **`maxlength`**: Limits the number of characters.
- **`placeholder`**: Shows light hint text inside an empty field.
- **`required`**: Makes filling the field mandatory before submit.

### HTML Graphics
HTML allows you to draw graphics on a web page using elements like `<canvas>` or `<svg>`.

- **HTML Canvas (`<canvas>`):** A container used to draw graphics using **JavaScript**. It works with pixels and is great for games and animations.
- **HTML SVG (`<svg>릭터`):** Used to draw vector graphics using **XML tags** (like circles and rectangles). It never loses quality when zoomed in or resized.

### HTML Media 

- ** Media:** Refers to things like video and audio added to a web page.
- ** Video (`<video>`):** Used to embed video files on a web page. (Supports controls like play, pause, and volume).
- ** Audio (`<audio>`):** Used to embed sound or music files on a web page.
- **HTML YouTube:** Methods to embed YouTube videos directly into a web page using an `<iframe>`


- ### Accessibility: 
- Making websites usable for everyone, including people with disabilities (e.g., using screen readers or keyboard navigation).

- ### SEO (Search Engine Optimization):
- Optimizing a website so it ranks higher in search engine results (like Google)
