[MDN Web Docs](https://developer.mozilla.org/en-US/docs/Web/CSS)

## Basic Styles:
- font-family: Specifies the font for an element.
- margin: Sets the margin (space outside) of an element.
- background-color: Sets the background color of an element.
- color: Sets the text color.

## Additional Heading Styles:
- color: Sets the text color.

## Link Styles:
- color: Sets the text color of links.
- text-decoration: Specifies the decoration added to text, such as underlining.

## Form Styles:
- background-color: Sets the background color of the form.
- padding: Sets the padding (space inside) of the form.
- border: Sets the border of the form.
- border-radius: Rounds the corners of the form.
- margin-bottom: Sets the margin at the bottom of the form.
- display: Specifies the display behavior.
- width: Sets the width of form elements.
- box-sizing: Defines the box model for sizing elements.
- margin-right: Sets the margin on the right side.
- cursor: Specifies the mouse cursor to be displayed.

## Table Styles:
- width: Sets the width of the table.
- border-collapse: Specifies whether table borders should be collapsed into a single border.
- margin-bottom: Sets the margin at the bottom of the table.
- border: Sets the border of table cells.
- padding: Sets the padding inside table cells.
- text-align: Aligns the text inside table cells.
- background-color: Sets the background color of table headers.

## Media Element Styles:
- margin-top: Sets the margin at the top of media elements.
- max-width: Sets the maximum width of media elements.

## Miscellaneous Styles:
- border-bottom: Adds a bottom border to an element.
- cursor: Specifies the type of cursor to be displayed.
- font-style: Specifies the font style for text.

## Footer Styles:
- text-align: Aligns the text inside the footer.

### 1. **Selectors:**
   - **Description:** Selectors target HTML elements to apply styles.
   - **Example:** 
     ```css
     body {
         color: #333;
     }
     ```

### 2. **Colors:**
   - **Attribute:** `color`
   - **Options:** Color names (e.g., `red`), hex codes (e.g., `#FF5733`), RGB values (e.g., `rgb(255, 87, 51)`).
   - **Description:** Sets the text color.
   - **Example:** 
     ```css
     p {
         color: blue;
     }
     ```

### 3. **Background Color:**
   - **Attribute:** `background-color`
   - **Options:** Same as color options.
   - **Description:** Sets the background color.
   - **Example:** 
     ```css
     body {
         background-color: #f0f0f0;
     }
     ```

### 4. **Fonts:**
   - **Attribute:** `font-family`
   - **Options:** Font names (e.g., `Arial`), generic font families (e.g., `sans-serif`).
   - **Description:** Sets the font for an element.
   - **Example:** 
     ```css
     h1 {
         font-family: 'Helvetica', sans-serif;
     }
     ```

### 5. **Font Size:**
   - **Attribute:** `font-size`
   - **Options:** Absolute values (e.g., `16px`), relative values (e.g., `1.2em`).
   - **Description:** Sets the font size.
   - **Example:** 
     ```css
     p {
         font-size: 18px;
     }
     ```

### 6. **Font Weight:**
   - **Attribute:** `font-weight`
   - **Options:** `normal`, `bold`, `bolder`, `lighter`, numeric values.
   - **Description:** Sets the thickness of the font.
   - **Example:** 
     ```css
     strong {
         font-weight: bold;
     }
     ```

### 7. **Text Decoration:**
   - **Attribute:** `text-decoration`
   - **Options:** `none`, `underline`, `overline`, `line-through`.
   - **Description:** Sets the text decoration.
   - **Example:** 
     ```css
     a {
         text-decoration: underline;
     }
     ```

### 8. **Text Alignment:**
   - **Attribute:** `text-align`
   - **Options:** `left`, `center`, `right`, `justify`.
   - **Description:** Sets the horizontal alignment of text.
   - **Example:** 
     ```css
     p {
         text-align: center;
     }
     ```

### 9. **Margin and Padding:**
   - **Attribute:** `margin`, `padding`
   - **Options:** Length values (e.g., `10px`), percentage values, `auto`.
   - **Description:** Sets the margin or padding around an element.
   - **Example:** 
     ```css
     div {
         margin: 10px;
         padding: 20px;
     }
     ```

### 10. **Border:**
   - **Attribute:** `border`
   - **Options:** Border width, style, and color.
   - **Description:** Sets the border of an element.
   - **Example:** 
     ```css
     img {
         border: 1px solid #ccc;
     }
     ```

### 11. **Width and Height:**
   - **Attribute:** `width`, `height`
   - **Options:** Length values, percentage values.
   - **Description:** Sets the width and height of an element.
   - **Example:** 
     ```css
     img {
         width: 100%;
         height: auto;
     }
     ```

### 12. **Display:**
   - **Attribute:** `display`
   - **Options:** `block`, `inline`, `inline-block`, `none`, etc.
   - **Description:** Sets the display behavior of an element.
   - **Example:** 
     ```css
     span {
         display: inline-block;
     }
     ```
