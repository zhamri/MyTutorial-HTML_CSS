## What is HTML
- HTML stands for HyperText Markup Language.
- It is the standard language used to create and structure web pages on the Internet.
- In short: HTML tells the browser what content to show — such as text, images, links, buttons, tables, and videos.

### 1. Basic Structure of an HTML Page
```html
<!DOCTYPE html>
<html>
<head>
    <title>My First Web Page</title>
</head>
<body>
<h1>Welcome!</h1>
<p>This is an example of a simple HTML document.</p>
</body>
</html>
```
| Section           | Purpose                                 |
| ----------------- | --------------------------------------- |
| `<!DOCTYPE html>` | Tells the browser to use HTML5          |
| `<html>`          | Root element of the page                |
| `<head>`          | Contains metadata (title, CSS, scripts) |
| `<body>`          | Contains visible content for users      |


### 2. Common HTML Tags
| Tag                    | Description          |
| ---------------------- | -------------------- |
| `<h1>` – `<h6>`        | Headings             |
| `<p>`                  | Paragraph            |
| `<a href="">`          | Hyperlink            |
| `<img src="">`         | Image                |
| `<ul>`, `<ol>`, `<li>` | Lists                |
| `<table>`              | Table                |
| `<div>`                | Division / container |
| `<span>`               | Inline container     |
| `<form>`               | Input form           |


## What is CSS
- CSS stands for Cascading Style Sheets.
- It is the language used to style and design web pages — controlling how HTML elements look (color, size, layout, fonts, spacing, animations, etc.).
- In short: HTML builds the structure, and CSS makes it beautiful.

### 1. What Does “Cascading” Mean?
- “Cascading” means if multiple styles apply to the same element, the browser decides which one wins — based on priority (specificity and order).
- Example:
```css
p { color: blue; }
p { color: red; } /* this one wins */
```

### 2. CSS Syntax
```css
selector {
  property: value;
}
```
Example
```css
p {
  color: red;
  font-size: 16px;
}
```

### 3. Basic Example
```html
<!DOCTYPE html>
<html>
<head>
  <style>
    h1 {
      color: blue;
      font-size: 40px;
    }
    p {
      color: gray;
      font-family: Arial, sans-serif;
    }
  </style>
</head>
<body>
  <h1>Hello, World!</h1>
  <p>This is my first styled web page.</p>
</body>
</html>
```
### 4. Three (3) Ways to Add CSS
| Method       | Where                        | Example                                    |
| ------------ | ---------------------------- | ------------------------------------------ |
| **Inline**   | Inside HTML tag              | `<p style="color:red;">Hello</p>`          |
| **Internal** | Inside `<style>` in `<head>` | `<style>p{color:red;}</style>`             |
| **External** | In separate `.css` file      | `<link rel="stylesheet" href="style.css">` |



## Summary
| Concept  | Description                 |
| -------- | --------------------------- |
| **HTML** | Structure — the content     |
| **CSS**  | Presentation — how it looks |
| **JS**   | Behavior — how it interacts |


## Try this:
1. type `lorem10`
2. the press `tab`

### Lorem Emmet Shorthands
| You Type      | Then Press `Tab` | What It Does                            |
| ------------- | ---------------- | --------------------------------------- |
| `lorem`       | →                | Generates ~30 words of dummy text       |
| `lorem10`     | →                | Generates 10 words                      |
| `lorem50`     | →                | Generates 50 words                      |
| `lorem*3`     | →                | Generates 3 paragraphs                  |
| `p*3>lorem10` | →                | Creates 3 `<p>` tags each with 10 words |


## References:
1. https://en.wikipedia.org/wiki/HTML
2. https://www.w3schools.com/html/html_intro.asp
3. https://developer.mozilla.org/en-US/docs/Web/HTML
4. https://en.wikipedia.org/wiki/CSS
5. https://www.w3schools.com/css/css_intro.asp
6. https://developer.mozilla.org/en-US/docs/Learn_web_development/Core/Styling_basics/What_is_CSS
