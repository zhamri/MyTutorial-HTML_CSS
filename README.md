## List

In HTML, a list is a way to organize and display a collection of related items — such as names, steps, or options — in a
structured format.

## List Tags

| **Tag**  | **Name / Purpose**                                          | **Example (Simplified)**                         |
|----------|-------------------------------------------------------------|--------------------------------------------------|
| `<ul>`   | **Unordered List** – creates a bulleted list.               | `<ul><li>Apple</li><li>Banana</li></ul>`         |
| `<ol>`   | **Ordered List** – creates a numbered list.                 | `<ol><li>Step 1</li><li>Step 2</li></ol>`        |
| `<li>`   | **List Item** – defines an item in `<ul>` or `<ol>`.        | `<li>Item</li>`                                  |
| `<dl>`   | **Description List** – defines terms and descriptions.      | `<dl><dt>HTML</dt><dd>Markup language</dd></dl>` |
| `<dt>`   | **Definition Term** – specifies the term in `<dl>`.         | `<dt>CSS</dt>`                                   |
| `<dd>`   | **Definition Description** – describes the term in `<dt>`.  | `<dd>Style sheet language</dd>`                  |
| `<menu>` | **Menu List** – defines a list of commands or menu options. | `<menu><li>Save</li><li>Exit</li></menu>`        |

## References:

1. https://developer.mozilla.org/en-US/docs/Learn_web_development/Core/Structuring_content/Lists
2. https://www.w3schools.com/html/html_lists.asp

## Try this:

| **Symbol / Part**   | **Meaning**             | **Description / Example**                                                                      |
|---------------------|-------------------------|------------------------------------------------------------------------------------------------|
| `ul`                | Element                 | Creates an unordered list (`<ul>`).                                                            |
| `>`                 | Child operator          | Nests the next element **inside** the previous one.<br>Example: `ul>li` → `<ul><li></li></ul>` |
| `li`                | Element                 | Creates a list item (`<li>`).                                                                  |
| `{ }`               | Text content            | Inserts text inside the element.<br>`li{Item}` → `<li>Item</li>`                               |
| `$`                 | Numbering placeholder   | Auto-increments with each repetition.<br>`li{Item $}` → `<li>Item 1</li>`, `<li>Item 2</li>`   |
| `*3`                | Multiplication operator | Repeats the previous element 3 times.                                                          |
| **Full Expression** | `ul>li{Item $}*3`       | Generates: <br>`<ul><li>Item 1</li><li>Item 2</li><li>Item 3</li></ul>`                        |

### Example 1: Unordered List

```
ul>li*3
```

Output:

```html

<ul>
    <li></li>
    <li></li>
    <li></li>
</ul>
```

### Example 2: Ordered List

```
ol>li*5
```

Output:

```html

<ol>
    <li></li>
    <li></li>
    <li></li>
    <li></li>
    <li></li>
</ol>
```

### Example 3: With Text and Numbering

```
ul>li{Item $}*3
```

Output:

```html

<ul>
    <li>Item 1</li>
    <li>Item 2</li>
    <li>Item 3</li>
</ul>
```

### Example 4: Nested List

```
ul>li{Main Item $}>ul>li{Sub Item $}*2
```

Output:

```html

<ul>
    <li>Main Item 1
        <ul>
            <li>Sub Item 1</li>
            <li>Sub Item 2</li>
        </ul>
    </li>
</ul>
```

## Edit List
- CTRL + CMD + G


