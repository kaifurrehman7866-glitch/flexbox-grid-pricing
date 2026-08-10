# Flexbox vs Grid — Pricing Section Playground

A responsive 3-column pricing section built in two different ways: **CSS Flexbox** and **CSS Grid**.

The project presents the same pricing layout twice so the two layout systems can be compared side by side. Both versions use a responsive breakpoint that changes the three-column layout into a single-column stack below 600px.

## Preview

The page includes:

- A **Flexbox** pricing section
- A **CSS Grid** pricing section
- Starter, Pro, and Enterprise pricing cards
- Responsive layouts for smaller screens
- A comparison table explaining the differences between Flexbox and Grid

## Technologies Used

- HTML5
- CSS3
- CSS Flexbox
- CSS Grid
- Responsive Design

## Project Structure

```text
flexbox-grid-pricing/
├── index.html
└── README.md
```

### `index.html`

Contains the complete project, including:

- Flexbox pricing layout
- CSS Grid pricing layout
- Pricing cards
- Responsive media queries
- Flexbox vs Grid comparison table

## Flexbox vs Grid

### Flexbox

The first version uses:

```css
display: flex;
gap: 20px;
```

The pricing cards use equal flexible widths, and below 600px they stack vertically using:

```css
flex-direction: column;
```

### CSS Grid

The second version uses:

```css
display: grid;
grid-template-columns: repeat(3, 1fr);
gap: 20px;
```

Below 600px, the layout changes to one column:

```css
grid-template-columns: 1fr;
```

## Comparison

| Aspect | Flexbox | CSS Grid |
|---|---|---|
| 3 equal columns | Uses flexible item sizing | Uses explicit grid columns |
| Responsive stack | `flex-direction: column` | `grid-template-columns: 1fr` |
| Gap between cards | `gap` | `gap` |
| Layout model | One-dimensional | Two-dimensional |
| Best suited for | Rows and linear layouts | Structured rows and columns |

## How to Run

1. Clone or download the repository.
2. Open `index.html` in a web browser.
3. Resize the browser window below **600px** to see the responsive single-column layouts.

You can also open the project in VS Code and use the **Live Server** extension.

## Key Takeaway

For a single row of equal-width pricing cards, Flexbox and Grid can produce very similar results. Flexbox feels natural for a one-dimensional row, while Grid provides explicit column definitions and can be more useful for layouts that need stronger two-dimensional structure.

## Author

**Kaif Ur Rehman**

---

*Created as a frontend HTML & CSS practice project.*
