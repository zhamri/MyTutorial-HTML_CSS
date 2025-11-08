## CSS Precedence / Cascade Order
When the browser decides which CSS rule to apply, it follows four main rules — in this order:

| **Priority**      | **Rule**                                       | **Meaning / Description**                                                           | **Example / Notes**                                                                              |
| ----------------- | ---------------------------------------------- | ----------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------ |
| **1️⃣ (Highest)** | **Inline Style**                               | Styles written directly inside an HTML element have the highest priority.           | `<p style="color: red;">Text</p>`                                                                |
| **2️⃣**           | **`!important` Declarations**                  | Overrides all other CSS rules, except another `!important` with higher specificity. | `p { color: blue !important; }`                                                                  |
| **3️⃣**           | **ID Selectors**                               | Targets elements by their unique ID — higher priority than classes or elements.     | `#title { color: green; }`                                                                       |
| **4️⃣**           | **Class / Pseudo-Class / Attribute Selectors** | Targets elements using class names, pseudo-classes (`:hover`), or attributes.       | `.note { color: orange; }`<br>`a:hover { color: pink; }`<br>`input[type=text] { color: black; }` |
| **5️⃣**           | **Element / Pseudo-Element Selectors**         | Targets HTML elements directly (lowest among author-defined styles).                | `p { color: gray; }`<br>`p::first-line { color: blue; }`                                         |
| **6️⃣ (Lowest)**  | **Browser Default Styles**                     | The built-in styles applied by the browser if no CSS rules are defined.             | For example, `<h1>` is bold and large by default.                                                |
