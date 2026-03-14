
# 1. What is CSS?

**CSS (Cascading Style Sheets)** is the language used to style and
design web pages.

### Purpose of CSS

CSS controls the **visual appearance** of HTML elements such as:

-   Colors
-   Fonts
-   Spacing
-   Alignment
-   Borders
-   Layout
-   Positioning

### Simple Understanding

-   **HTML** → Creates the structure of a webpage\
-   **CSS** → Makes the webpage look attractive

Example:

``` html
<p style="color:red;">Hello World</p>
```

------------------------------------------------------------------------

# 2. Types of CSS

There are **three types of CSS** used in web development.

1.  Inline CSS
2.  Internal CSS
3.  External CSS

------------------------------------------------------------------------

## 2.1 Inline CSS

Inline CSS is written **directly inside an HTML element** using the
`style` attribute.

### Example

``` html
<p style="color:red; font-size:20px;">
This is a paragraph using inline CSS
</p>
```

### When to Use

-   Small styling changes
-   Quick testing

### Not Recommended For

Large projects because it makes the code difficult to maintain.

------------------------------------------------------------------------

## 2.2 Internal CSS

Internal CSS is written inside the **`<style>` tag** within the
**`<head>` section** of an HTML file.

### Example

``` html
<head>
<style>
p {
  color: blue;
  font-size: 18px;
}
</style>
</head>
```

### When to Use

-   Styling a **single webpage**

------------------------------------------------------------------------

## 2.3 External CSS

External CSS is written in a **separate file** with the extension
`.css`.

Example file:

    style.css

### Linking CSS to HTML

``` html
<link rel="stylesheet" href="style.css">
```

### Advantages

-   Clean code
-   Reusable styles
-   Easy maintenance
-   Best practice for large projects

------------------------------------------------------------------------

# 3. CSS Selectors

CSS selectors are used to **select HTML elements** and apply styles to
them.

------------------------------------------------------------------------

## 3.1 Element Selector

Targets all elements with a specific HTML tag.

Example:

``` css
p {
  color: blue;
}
```

This will style **all paragraph elements**.

------------------------------------------------------------------------

## 3.2 ID Selector

Selects a **single unique element** using an `id`.

Symbol used: `#`

Example:

``` css
#title {
  color: red;
}
```

HTML:

``` html
<h1 id="title">Hello</h1>
```

------------------------------------------------------------------------

## 3.3 Class Selector

Selects **multiple elements** with the same class name.

Symbol used: `.`

Example:

``` css
.box {
  background-color: yellow;
}
```

HTML:

``` html
<div class="box">Content</div>
```

------------------------------------------------------------------------

## 3.4 Group Selector

Used to apply the **same style to multiple elements**.

Example:

``` css
h1, p {
  color: green;
}
```

HTML:

``` html
<h1>Heading</h1>
<p>Paragraph</p>
```

------------------------------------------------------------------------

# 4. CSS Box Model

Every HTML element is treated as a **box** in CSS.

The box model consists of four parts:

    Margin
    Border
    Padding
    Content

### Explanation

**Content**\
The actual text or image inside the element.

**Padding**\
Space between the content and the border.

**Border**\
The line surrounding the padding and content.

**Margin**\
Space outside the border separating elements.

Example:

``` css
div {
  margin: 10px;
  padding: 20px;
  border: 2px solid black;
}
```

------------------------------------------------------------------------

# 5. CSS Display Property

The `display` property defines **how an element appears on a webpage**.

------------------------------------------------------------------------

## Block

-   Takes full available width
-   Starts on a new line

Examples:

    div
    p
    h1

------------------------------------------------------------------------

## Inline

-   Takes only the required width
-   Does not start on a new line

Examples:

    span
    a

------------------------------------------------------------------------

## Inline‑Block

-   Appears inline
-   Allows width and height to be set

Example:

``` css
display: inline-block;
```

------------------------------------------------------------------------

## None

Hides the element completely.

``` css
display: none;
```

The element **will not take space on the page**.

------------------------------------------------------------------------

# Summary

CSS is used to **style and design webpages**.\
Key concepts include:

-   Types of CSS
-   CSS Selectors
-   Box Model
-   Display Property

Understanding these basics is essential for **front‑end web
development**.

------------------------------------------------------------------------