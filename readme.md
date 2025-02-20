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



