# 📖 CSS Flexbox Cheatsheet

A complete **CSS Flexbox Cheatsheet** to master layouts quickly. Perfect for beginners and pros!

---

## 📦 Flex Container Properties

| Property            | Values                                                                                     | Description                                                  |
|---------------------|---------------------------------------------------------------------------------------------|--------------------------------------------------------------|
| **display**         | `flex` \| `inline-flex`                                                                     | Defines a flex container.                                    |
| **flex-direction**  | `row` \| `row-reverse` \| `column` \| `column-reverse`                                      | Direction of main axis.                                      |
| **flex-wrap**       | `nowrap` \| `wrap` \| `wrap-reverse`                                                        | Whether flex items wrap onto multiple lines.                 |
| **flex-flow**       | `<flex-direction> <flex-wrap>`                                                              | Shorthand for `flex-direction` and `flex-wrap`.              |
| **justify-content** | `flex-start` \| `flex-end` \| `center` \| `space-between` \| `space-around` \| `space-evenly`| Aligns items on the main axis.                               |
| **align-items**     | `flex-start` \| `flex-end` \| `center` \| `baseline` \| `stretch`                            | Aligns items on the cross axis.                              |
| **align-content**   | `flex-start` \| `flex-end` \| `center` \| `space-between` \| `space-around` \| `stretch`     | Aligns multiple lines (only if items wrap).                  |

---

## 📦 Flex Item Properties

| Property         | Values                                                                    | Description                                               |
|------------------|---------------------------------------------------------------------------|-----------------------------------------------------------|
| **order**        | `<number>`                                                                | Controls item order. Default: `0`.                        |
| **flex-grow**    | `<number>`                                                                | Defines how much the item grows relative to others.       |
| **flex-shrink**  | `<number>`                                                                | Defines how much the item shrinks relative to others.     |
| **flex-basis**   | `<length>` \| `auto`                                                      | Initial size before growing/shrinking.                    |
| **flex**         | `<flex-grow> <flex-shrink> <flex-basis>`                                  | Shorthand for the above 3 properties.                     |
| **align-self**   | `auto` \| `flex-start` \| `flex-end` \| `center` \| `baseline` \| `stretch`| Overrides `align-items` for a single item.                 |

---

## 🖼 Flexbox Diagram

```
Main Axis (row) → →
|────────────────────────────────────────|
|  Cross Axis ↑
|             |
|             ↓
```

---

## 💻 Example: Basic Flex Layout

```css
.container {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: center;
}
```

```html
<div class="container">
  <div>Item 1</div>
  <div>Item 2</div>
  <div>Item 3</div>
</div>
```

---

## 🎨 Example: Responsive Flexbox Grid

```css
.container {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  gap: 10px;
}

.item {
  flex: 1 1 200px; /* grow, shrink, basis */
  background: #f4f4f4;
  padding: 20px;
  text-align: center;
}
```

```html
<div class="container">
  <div class="item">1</div>
  <div class="item">2</div>
  <div class="item">3</div>
  <div class="item">4</div>
</div>
```

---

## 📝 Quick Tips

✅ Use `gap` for spacing between items (better than margins).  
✅ Combine `flex: 1` with `min-width` for responsive grids.  
✅ `align-items: stretch` makes items fill cross axis by default.  

---

## 📚 Resources

- [CSS-Tricks Flexbox Guide](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)
- [MDN Flexbox Docs](https://developer.mozilla.org/en-US/docs/Web/CSS/flex)
- [Flexbox Froggy Game](https://flexboxfroggy.com)

---

## 🏁 License

This cheatsheet is free to use under the [MIT License](LICENSE).
