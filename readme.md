# Basic HTML Tags and Their Definitions

HTML (HyperText Markup Language) is the standard language for creating web pages. Here are some basic HTML tags and their definitions:

## Basic Tags

- `<!DOCTYPE html>`: Defines the document type and version of HTML.
- `<html>`: The root element of an HTML page.
- `<head>`: Contains meta-information about the HTML document.
- `<title>`: Sets the title of the HTML document (shown in the browser's title bar or tab).
- `<body>`: Contains the content of the HTML document.

## Text Formatting Tags

- `<h1>` to `<h6>`: Define HTML headings, `<h1>` being the highest (or most important) level and `<h6>` the lowest.
- `<p>`: Defines a paragraph.
- `<br>`: Inserts a single line break.
- `<hr>`: Defines a thematic change in the content (horizontal rule).
- `<strong>`: Defines important text (usually displayed in bold).
- `<em>`: Defines emphasized text (usually displayed in italics).

## List Tags

- `<ul>`: Defines an unordered list.
- `<ol>`: Defines an ordered list.
- `<li>`: Defines a list item.

## Link and Media Tags

- `<a>`: Defines a hyperlink.
- `<img>`: Embeds an image.
- `<video>`: Embeds a video.
- `<audio>`: Embeds an audio file.

## Table Tags

- `<table>`: Defines a table.
- `<tr>`: Defines a table row.
- `<td>`: Defines a table cell.
- `<th>`: Defines a table header cell.

## Form Tags

- `<form>`: Defines an HTML form for user input.
- `<input>`: Defines an input control.
- `<label>`: Defines a label for an `<input>` element.
- `<button>`: Defines a clickable button.

These are some of the fundamental HTML tags used to structure and format web content.
## Metadata Tags

Metadata is data that provides information about other data. In HTML, metadata is defined in the `<head>` section of the document. Here are some common metadata tags:

- `<meta>`: Defines metadata about an HTML document. It is used to specify the character set, page description, keywords, author of the document, and viewport settings.
- `<link>`: Defines the relationship between the current document and an external resource. It is commonly used to link to stylesheets.
- `<style>`: Contains internal CSS styles for the document.
- `<script>`: Embeds or references JavaScript code.

## Semantic and Non-Semantic Tags

Semantic HTML tags provide meaning to the content they enclose, making it easier for browsers and search engines to understand the structure and content of a webpage. Non-semantic tags, on the other hand, do not provide any information about the content they contain.

### Semantic Tags

- `<header>`: Defines a header for a document or section.
- `<nav>`: Defines a container for navigation links.
- `<section>`: Defines a section in a document.
- `<article>`: Defines an independent, self-contained piece of content.
- `<aside>`: Defines content aside from the main content (like a sidebar).
- `<footer>`: Defines a footer for a document or section.
- `<main>`: Defines the main content of a document.
- `<figure>`: Specifies self-contained content, like illustrations, diagrams, or photos.
- `<figcaption>`: Defines a caption for a `<figure>` element.

### Non-Semantic Tags

- `<div>`: Defines a division or section in an HTML document. It is often used as a container for other elements.
- `<span>`: Defines a section in a document. It is used to group inline elements.

Using semantic tags improves the accessibility and SEO of a webpage, while non-semantic tags are useful for styling and layout purposes.


## CSS Selectors and Basics of CSS

CSS (Cascading Style Sheets) is used to style and layout web pages. It allows you to apply styles to HTML elements and control their appearance.

### CSS Selectors

CSS selectors are used to select the HTML elements you want to style. Here are some basic types of selectors:

- **Element Selector**: Selects all elements of a given type.
    ```css
    p {
        color: blue;
    }
    ```
    This will make all `<p>` elements blue.

- **Class Selector**: Selects all elements with a specific class attribute.
    ```css
    .example {
        font-size: 20px;
    }
    ```
    This will apply a font size of 20px to all elements with the class `example`.

- **ID Selector**: Selects a single element with a specific id attribute.
    ```css
    #unique {
        background-color: yellow;
    }
    ```
    This will apply a yellow background to the element with the id `unique`.

- **Attribute Selector**: Selects elements based on an attribute or attribute value.
    ```css
    [type="text"] {
        border: 1px solid black;
    }
    ```
    This will apply a border to all input elements with the type attribute set to "text".

- **Descendant Selector**: Selects elements that are descendants of another element.
    ```css
    div p {
        margin: 10px;
    }
    ```
    This will apply a margin to all `<p>` elements that are inside a `<div>`.

### Basics of CSS

CSS is composed of rules that specify how HTML elements should be styled. Each rule consists of a selector and a declaration block.

- **Selector**: Indicates which HTML elements the rule applies to.
- **Declaration Block**: Contains one or more declarations separated by semicolons. Each declaration includes a property and a value.

Example:
```css
h1 {
    color: red;
    text-align: center;
}
```
In this example, the `h1` selector targets all `<h1>` elements, and the declaration block sets the text color to red and centers the text.

### Common CSS Properties

- **Color**: Sets the color of the text.
    ```css
    color: blue;
    ```

- **Background**: Sets the background color or image.
    ```css
    background-color: lightgrey;
    ```

- **Font**: Sets the font family, size, weight, and style.
    ```css
    font-family: Arial, sans-serif;
    font-size: 16px;
    font-weight: bold;
    font-style: italic;
    ```

- **Margin**: Sets the space outside an element.
    ```css
    margin: 20px;
    ```

- **Padding**: Sets the space inside an element.
    ```css
    padding: 10px;
    ```

- **Border**: Sets the border around an element.
    ```css
    border: 1px solid black;
    ```

These are some of the fundamental concepts of CSS that help in styling and designing web pages effectively.

### Adjacent Sibling Selector

The adjacent sibling selector selects an element that is directly after another specific element. It is represented by the `+` symbol.

Example:
```css
h1 + p {
    color: green;
}
```
In this example, the adjacent sibling selector targets any `<p>` element that immediately follows an `<h1>` element and sets its text color to green.

### General Sibling Selector

The general sibling selector selects all elements that are siblings of a specified element. It is represented by the `~` symbol.

Example:
```css
h1 ~ p {
    color: orange;
}
```
In this example, the general sibling selector targets all `<p>` elements that are siblings of an `<h1>` element and sets their text color to orange.


### Pseudo-Classes

Pseudo-classes are keywords added to selectors that specify a special state of the selected elements. They are used to define the styling of an element when it is in a particular state.

#### Common Pseudo-Classes

- **`:hover`**: Applies when the user designates an element (usually with a pointing device), but does not activate it.
    ```css
    a:hover {
        color: red;
    }
    ```
    This will change the color of a link to red when the user hovers over it.

- **`:visited`**: Applies once the link has been visited by the user.
    ```css
    a:visited {
        color: purple;
    }
    ```
    This will change the color of a link to purple if it has been visited.

- **`:active`**: Applies when an element is being activated by the user (e.g., when a link is being clicked).
    ```css
    a:active {
        color: blue;
    }
    ```
    This will change the color of a link to blue when it is being clicked.

- **`:focus`**: Applies when an element has received focus (e.g., when a user clicks on an input field).
    ```css
    input:focus {
        border-color: green;
    }
    ```
    This will change the border color of an input field to green when it is focused.

Pseudo-classes enhance the interactivity and user experience of a webpage by allowing different styles to be applied based on user actions.
## Summary of CSS Attributes

CSS attributes are used to style and layout HTML elements. Here are some common CSS attributes:

- **Color**: Sets the color of the text.
    ```css
    color: blue;
    ```

- **Background**: Sets the background color or image.
    ```css
    background-color: lightgrey;
    ```

- **Font**: Sets the font family, size, weight, and style.
```css
font-family: Arial, sans-serif;
font-size: 16px;
font-weight: bold;
font-style: italic;
```

- **Margin**: Sets the space outside an element.
```css
margin: 20px;
```

- **Padding**: Sets the space inside an element.
```css
padding: 10px;
```

- **Border**: Sets the border around an element.
```css
border: 1px solid black;
```

- **Width**: Sets the width of an element.
```css
width: 100px;
```

- **Height**: Sets the height of an element.
```css
height: 100px;
```

- **Display**: Specifies the display behavior of an element.
```css
display: block;
```

- **Position**: Specifies the positioning method of an element.
```css
position: absolute;
```

- **Top, Right, Bottom, Left**: Specifies the offset of an element from its positioned container.
```css
top: 10px;
right: 10px;
bottom: 10px;
left: 10px;
```

- **Float**: Specifies whether an element should float to the left, right, or not at all.
```css
float: left;
```

- **Clear**: Specifies what elements can float beside the cleared element and on which side.
```css
clear: both;
```

- **Overflow**: Specifies what happens if content overflows an element's box.
```css
overflow: hidden;
```

- **Visibility**: Specifies whether an element is visible or hidden.
```css
visibility: hidden;
```

- **Z-index**: Specifies the stack order of an element.
```css
z-index: 10;
```

These attributes are fundamental in controlling the layout and appearance of HTML elements using CSS.



### Pseudo-Elements

Pseudo-elements are keywords added to selectors that allow you to style specific parts of an element. They are used to apply styles to a portion of an element's content.

#### Common Pseudo-Elements

- **`::before`**: Inserts content before the content of an element.
    ```css
    p::before {
        content: "Note: ";
        font-weight: bold;
    }
    ```
    This will insert the text "Note: " before the content of all `<p>` elements.

- **`::after`**: Inserts content after the content of an element.
    ```css
    p::after {
        content: " End of paragraph.";
        font-style: italic;
    }
    ```
    This will insert the text " End of paragraph." after the content of all `<p>` elements.

- **`::first-line`**: Applies styles to the first line of a block-level element.
    ```css
    p::first-line {
        color: blue;
        font-weight: bold;
    }
    ```
    This will make the first line of all `<p>` elements blue and bold.

- **`::first-letter`**: Applies styles to the first letter of a block-level element.
    ```css
    p::first-letter {
        font-size: 200%;
        color: red;
    }
    ```
    This will make the first letter of all `<p>` elements twice as large and red.

Pseudo-elements enhance the ability to style specific parts of an element's content, providing more control over the presentation of web pages.

### Attribute Selector

The attribute selector in CSS is used to select elements based on the presence or value of a given attribute. It allows you to apply styles to elements that have specific attributes or attribute values.

#### Syntax

The basic syntax of an attribute selector is:
```css
[attribute] {
    /* CSS properties */
}
```
This selects all elements that have the specified attribute, regardless of its value.

#### Examples

- **Select elements with a specific attribute:**
    ```css
    [title] {
        color: blue;
    }
    ```
    This will apply the color blue to all elements that have a `title` attribute.

- **Select elements with a specific attribute value:**
    ```css
    [type="text"] {
        border: 1px solid black;
    }
    ```
    This will apply a border to all input elements with the `type` attribute set to "text".

- **Select elements with an attribute value containing a specific word:**
    ```css
    [class~="example"] {
        font-size: 20px;
    }
    ```
    This will apply a font size of 20px to all elements with a `class` attribute that contains the word "example".

- **Select elements with an attribute value starting with a specific value:**
    ```css
    [href^="https"] {
        color: green;
    }
    ```
    This will apply the color green to all links (`<a>` elements) where the `href` attribute value starts with "https".

- **Select elements with an attribute value ending with a specific value:**
    ```css
    [src$=".jpg"] {
        border: 2px solid red;
    }
    ```
    This will apply a red border to all images (`<img>` elements) where the `src` attribute value ends with ".jpg".

- **Select elements with an attribute value containing a specific substring:**
    ```css
    [data-info*="part"] {
        background-color: yellow;
    }
    ```
    This will apply a yellow background to all elements with a `data-info` attribute that contains the substring "part".

Attribute selectors provide a powerful way to target elements based on their attributes, allowing for more precise and flexible styling.


CSS fonts 

### CSS Fonts

CSS provides various properties to control the appearance of text on a webpage. Here are some common CSS font properties:

- **`font-family`**: Specifies the font family for the text.
    ```css
    font-family: Arial, sans-serif;
    ```

- **`font-size`**: Specifies the size of the font.
    ```css
    font-size: 16px;
    ```

- **`font-weight`**: Specifies the weight (or boldness) of the font.
    ```css
    font-weight: bold;
    ```

- **`font-style`**: Specifies the style of the font (e.g., normal, italic, oblique).
    ```css
    font-style: italic;
    ```

- **`font-variant`**: Specifies whether the text should be displayed in small-caps.
    ```css
    font-variant: small-caps;
    ```

- **`line-height`**: Specifies the height of a line of text.
    ```css
    line-height: 1.5;
    ```

- **`letter-spacing`**: Specifies the space between characters.
    ```css
    letter-spacing: 2px;
    ```

- **`text-transform`**: Controls the capitalization of text.
    ```css
    text-transform: uppercase;
    ```

- **`text-align`**: Specifies the horizontal alignment of text.
    ```css
    text-align: center;
    ```

- **`text-decoration`**: Specifies the decoration added to text (e.g., underline, overline, line-through).
    ```css
    text-decoration: underline;
    ```

These properties allow you to customize the appearance of text on your webpage, making it more visually appealing and easier to read.



### CSS Units

CSS units are used to define the size of various elements, such as width, height, margin, padding, and font size. There are two main types of CSS units: absolute and relative.

#### Absolute Units

Absolute units are fixed and do not change based on other elements or the viewport. Common absolute units include:

- **`px` (pixels)**: Represents a single dot on the screen.
    ```css
    width: 100px;
    ```

- **`pt` (points)**: Commonly used in print media, where 1pt is 1/72 of an inch.
    ```css
    font-size: 12pt;
    ```

- **`cm` (centimeters)**: Represents a length in centimeters.
    ```css
    margin: 2cm;
    ```

- **`mm` (millimeters)**: Represents a length in millimeters.
    ```css
    padding: 10mm;
    ```

- **`in` (inches)**: Represents a length in inches.
    ```css
    height: 1in;
    ```

#### Relative Units

Relative units are based on the size of other elements or the viewport, making them more flexible and responsive. Common relative units include:

- **`%` (percentage)**: Represents a percentage of the parent element's size.
    ```css
    width: 50%;
    ```

- **`em`**: Relative to the font size of the element. If the font size of the element is 16px, 1em is 16px.
    ```css
    padding: 2em;
    ```

- **`rem`**: Relative to the font size of the root element (`<html>`). If the root font size is 16px, 1rem is 16px.
    ```css
    margin: 1.5rem;
    ```

- **`vw` (viewport width)**: Represents a percentage of the viewport's width. 1vw is 1% of the viewport's width.
    ```css
    width: 50vw;
    ```

- **`vh` (viewport height)**: Represents a percentage of the viewport's height. 1vh is 1% of the viewport's height.
    ```css
    height: 50vh;
    ```

- **`vmin`**: Represents the smaller value of `vw` and `vh`.
    ```css
    font-size: 2vmin;
    ```

- **`vmax`**: Represents the larger value of `vw` and `vh`.
    ```css
    font-size: 2vmax;
    ```

Using the appropriate CSS units helps create responsive and adaptable web designs that work well on various devices and screen sizes.

## CSS Colors

CSS provides various ways to specify colors for elements on a webpage. Here are some common methods to define colors in CSS:

### Named Colors

CSS supports 140 named colors, such as `red`, `blue`, `green`, etc.

```css
color: red;
background-color: blue;
```

### Hexadecimal Colors

Hexadecimal colors are defined using a `#` followed by six hexadecimal digits (0-9, A-F). The first two digits represent the red component, the next two represent the green component, and the last two represent the blue component.

```css
color: #ff0000; /* Red */
background-color: #0000ff; /* Blue */
```

### RGB Colors

RGB colors are defined using the `rgb()` function, which takes three comma-separated values representing the red, green, and blue components (0-255).

```css
color: rgb(255, 0, 0); /* Red */
background-color: rgb(0, 0, 255); /* Blue */
```

### RGBA Colors

RGBA colors are similar to RGB colors but include an alpha channel to specify the opacity (0.0 to 1.0).

```css
color: rgba(255, 0, 0, 0.5); /* Semi-transparent red */
background-color: rgba(0, 0, 255, 0.5); /* Semi-transparent blue */
```

### HSL Colors

HSL colors are defined using the `hsl()` function, which takes three values: hue (0-360), saturation (0%-100%), and lightness (0%-100%).

```css
color: hsl(0, 100%, 50%); /* Red */
background-color: hsl(240, 100%, 50%); /* Blue */
```

### HSLA Colors

HSLA colors are similar to HSL colors but include an alpha channel to specify the opacity (0.0 to 1.0).

```css
color: hsla(0, 100%, 50%, 0.5); /* Semi-transparent red */
background-color: hsla(240, 100%, 50%, 0.5); /* Semi-transparent blue */
```

Using these methods, you can define a wide range of colors to enhance the visual appeal of your web pages.

## CSS Background Colors

CSS background colors are used to set the background color of an element. You can use various methods to define background colors, similar to how you define text colors.

### Setting Background Colors

You can set the background color of an element using the `background-color` property.

#### Named Colors

```css
background-color: red;
```

#### Hexadecimal Colors

```css
background-color: #ff0000; /* Red */
```

#### RGB Colors

```css
background-color: rgb(255, 0, 0); /* Red */
```

#### RGBA Colors

```css
background-color: rgba(255, 0, 0, 0.5); /* Semi-transparent red */
```

#### HSL Colors

```css
background-color: hsl(0, 100%, 50%); /* Red */
```

#### HSLA Colors

```css
background-color: hsla(0, 100%, 50%, 0.5); /* Semi-transparent red */
```

### Applying Background Colors

You can apply background colors to various HTML elements, such as `<div>`, `<p>`, `<header>`, etc.

Example:
```html
<div style="background-color: lightblue;">
    This div has a light blue background.
</div>
```

Using background colors effectively can enhance the visual appeal and readability of your web pages.
## CSS Tables

CSS provides various properties to style HTML tables, making them more visually appealing and easier to read. Here are some common CSS properties used to style tables:

### Table Properties

- **`border`**: Sets the border for the table and its cells.
    ```css
    table, th, td {
        border: 1px solid black;
    }
    ```

- **`border-collapse`**: Specifies whether the table borders should be collapsed into a single border or separated.
    ```css
    table {
        border-collapse: collapse;
    }
    ```

- **`width`**: Sets the width of the table.
    ```css
    table {
        width: 100%;
    }
    ```

- **`padding`**: Sets the padding inside the table cells.
    ```css
    th, td {
        padding: 10px;
    }
    ```

- **`text-align`**: Sets the horizontal alignment of the text in the table cells.
    ```css
    th {
        text-align: left;
    }
    ```

- **`background-color`**: Sets the background color of the table cells.
    ```css
    th {
        background-color: #f2f2f2;
    }
    ```

### Example

Here is an example of a styled table using CSS:

```html
<table>
    <tr>
        <th>Header 1</th>
        <th>Header 2</th>
        <th>Header 3</th>
    </tr>
    <tr>
        <td>Data 1</td>
        <td>Data 2</td>
        <td>Data 3</td>
    </tr>
    <tr>
        <td>Data 4</td>
        <td>Data 5</td>
        <td>Data 6</td>
    </tr>
</table>
```

```css
table, th, td {
    border: 1px solid black;
    border-collapse: collapse;
}

th, td {
    padding: 10px;
    text-align: left;
}

th {
    background-color: #f2f2f2;
}
```

Using these CSS properties, you can create well-structured and visually appealing tables for your web pages.

## CSS Icons

CSS icons are used to add visual elements to your web pages, enhancing the user experience. You can use icon libraries like Font Awesome, Material Icons, or create custom icons using CSS.

### Using Font Awesome

Font Awesome is a popular icon library that provides a wide range of icons. To use Font Awesome, you need to include the Font Awesome CSS file in your HTML document.

#### Example

1. Include the Font Awesome CSS file in the `<head>` section of your HTML document:
    ```html
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.4/css/all.min.css">
    ```

2. Use the Font Awesome icons in your HTML:
    ```html
    <i class="fas fa-home"></i> Home
    <i class="fas fa-envelope"></i> Contact
    ```

### Creating Custom Icons with CSS

You can also create custom icons using CSS by styling HTML elements.

#### Example

1. Create an HTML element for the icon:
    ```html
    <div class="custom-icon"></div>
    ```

2. Style the icon using CSS:
    ```css
    .custom-icon {
        width: 50px;
        height: 50px;
        background-color: #000;
        mask: url('icon.svg') no-repeat center;
        -webkit-mask: url('icon.svg') no-repeat center;
    }
    ```

Using CSS icons can enhance the visual appeal of your web pages and provide a better user experience.

## CSS Forms

CSS forms are used to style HTML forms, making them more visually appealing and user-friendly. Here are some common CSS properties used to style forms:

### Form Properties

- **`width`**: Sets the width of the form elements.
    ```css
    input[type="text"], input[type="email"], input[type="password"], textarea {
        width: 100%;
        padding: 10px;
        margin: 5px 0;
        box-sizing: border-box;
    }
    ```

- **`padding`**: Sets the padding inside the form elements.
    ```css
    input[type="text"], input[type="email"], input[type="password"], textarea {
        padding: 10px;
    }
    ```

- **`border`**: Sets the border for the form elements.
    ```css
    input[type="text"], input[type="email"], input[type="password"], textarea {
        border: 1px solid #ccc;
        border-radius: 4px;
    }
    ```

- **`background-color`**: Sets the background color of the form elements.
    ```css
    input[type="text"], input[type="email"], input[type="password"], textarea {
        background-color: #f9f9f9;
    }
    ```

- **`focus`**: Sets the styles for the form elements when they are focused.
    ```css
    input[type="text"]:focus, input[type="email"]:focus, input[type="password"]:focus, textarea:focus {
        border-color: #4CAF50;
        outline: none;
    }
    ```

### Example

Here is an example of a styled form using CSS:

```html
<form>
    <label for="name">Name:</label>
    <input type="text" id="name" name="name">

    <label for="email">Email:</label>
    <input type="email" id="email" name="email">

    <label for="message">Message:</label>
    <textarea id="message" name="message"></textarea>

    <input type="submit" value="Submit">
</form>
```

```css
form {
    max-width: 600px;
    margin: 0 auto;
}

label {
    display: block;
    margin-bottom: 5px;
}

input[type="text"], input[type="email"], textarea {
    width: 100%;
    padding: 10px;
    margin: 5px 0 20px 0;
    border: 1px solid #ccc;
    border-radius: 4px;
    box-sizing: border-box;
}

input[type="text"]:focus, input[type="email"]:focus, textarea:focus {
    border-color: #4CAF50;
    outline: none;
}

input[type="submit"] {
    background-color: #4CAF50;
    color: white;
    padding: 10px 20px;
    border: none;
    border-radius: 4px;
    cursor: pointer;
}

input[type="submit"]:hover {
    background-color: #45a049;
}
```

Using these CSS properties, you can create well-structured and visually appealing forms for your web pages.
## CSS Text

CSS provides various properties to control the appearance and layout of text on a webpage. Here are some common CSS text properties:

### Text Properties

- **`color`**: Sets the color of the text.
    ```css
    color: blue;
    ```

- **`text-align`**: Specifies the horizontal alignment of text.
    ```css
    text-align: center;
    ```

- **`text-decoration`**: Specifies the decoration added to text (e.g., underline, overline, line-through).
    ```css
    text-decoration: underline;
    ```

- **`text-transform`**: Controls the capitalization of text.
    ```css
    text-transform: uppercase;
    ```

- **`text-indent`**: Specifies the indentation of the first line of text.
    ```css
    text-indent: 50px;
    ```

- **`line-height`**: Specifies the height of a line of text.
    ```css
    line-height: 1.5;
    ```

- **`letter-spacing`**: Specifies the space between characters.
    ```css
    letter-spacing: 2px;
    ```

- **`word-spacing`**: Specifies the space between words.
    ```css
    word-spacing: 5px;
    ```

- **`text-shadow`**: Adds shadow to text.
    ```css
    text-shadow: 2px 2px 5px grey;
    ```

These properties allow you to customize the appearance and layout of text on your webpage, making it more visually appealing and easier to read.
## CSS Nesting

CSS Nesting allows you to nest your CSS selectors in a way that follows the same visual hierarchy of your HTML. This makes your CSS more readable and maintainable.

### Example

Without nesting:
```css
nav ul {
    list-style: none;
}

nav ul li {
    display: inline-block;
}

nav ul li a {
    text-decoration: none;
}
```

With nesting:
```css
nav {
    ul {
        list-style: none;

        li {
            display: inline-block;

            a {
                text-decoration: none;
            }
        }
    }
}
```

CSS Nesting is not yet fully supported in all browsers, but it can be used with preprocessors like Sass.

## CSS Container Queries

CSS Container Queries allow you to apply styles to an element based on the size of its container, rather than the size of the viewport. This is useful for creating responsive components that adapt to their container's size.

### Example

```css
.container {
    container-type: inline-size;
}

@container (min-width: 500px) {
    .item {
        font-size: 1.5rem;
    }
}

@container (max-width: 499px) {
    .item {
        font-size: 1rem;
    }
}
```

In this example, the `.item` element's font size changes based on the width of its container. Container Queries are a powerful tool for creating flexible, responsive designs.