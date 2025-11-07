## `px` vs `em` vs `rem`
| Unit  | Relative To               | Responsive? | Example (if base = 16px)       |
| ----- | ------------------------- | ----------- | ------------------------------ |
| `px`  | Fixed pixel               | ❌ No        | 16px = 16px                    |
| `em`  | Parent font size          | ✅ Yes       | 1.5em = 24px if parent is 16px |
| `rem` | Root (`<html>`) font size | ✅ Yes       | 1.5rem = 24px always           |

### 1. `px` — Pixels (Fixed Unit)
- px stands for pixels, the smallest display unit on a screen.
- It’s an absolute unit — meaning it does not scale relative to anything else.
- 1px is roughly one dot on your screen (though high-DPI screens scale it).
- Example:
```css
p {
  font-size: 16px;
}
```
This means the text is exactly 16 pixels high — no matter the parent element or screen size.

#### ✅ Advantages
- Consistent across browsers.
- Predictable and precise.

#### ❌ Disadvantages
- Not responsive — doesn’t scale automatically with user zoom or accessibility settings.

### 2. `em` — Relative to Parent’s Font Size
- em is a relative unit.
- It scales based on the font size of its parent element.
- Example: If the parent has:
```css
body {
  font-size: 16px;
}
p {
  font-size: 1.5em;
}
```
Then 1.5em = 1.5 × 16px = 24px

#### ✅ Advantages
- Scales naturally — great for accessibility and responsive design.
- Allows nested scaling (children inherit and multiply parent sizes).

#### ❌ Disadvantages
- Can “compound” (stack up) if nested, making values unpredictable sometimes.


### Comparison Example
```css
<div style="font-size: 16px;">
  <p style="font-size: 1em;">This is 16px</p>
  <p style="font-size: 2em;">This is 32px</p>
</div>

<div style="font-size: 20px;">
  <p style="font-size: 1em;">This is 20px</p>
  <p style="font-size: 2em;">This is 40px</p>
</div>
```
>Notice how the second block’s text becomes bigger — because em depends on the parent’s font size.

### `rem` — Root em
- rem = root em (relative to the root <html> font size, not the parent).
- Most browsers default to 16px at the root.
- Example:
```css
html {
  font-size: 16px;
}
h1 {
  font-size: 2rem; /* = 32px everywhere */
}
```
>More predictable than em, because it doesn’t multiply in nested elements.


## References:
1. https://developer.mozilla.org/en-US/docs/Web/HTML/Reference/Elements/Heading_Elements
2. https://developer.mozilla.org/en-US/docs/Web/HTML/Reference/Elements/style
2. https://www.w3schools.com/html/html_headings.asp
3. https://www.w3schools.com/html/html_styles.asp
