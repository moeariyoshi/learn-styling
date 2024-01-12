# CSS vs. SCSS (Sass: Syntactically Awesome Stylesheets)

### 1. **Syntax:**
   - **CSS:** Uses a simple syntax.
   - **SCSS:** Uses a more advanced and nested syntax.

### 2. **Variables:**
   - **CSS:** No native variable support.
   - **SCSS:** Supports variables using the `$` symbol.
     ```scss
     // SCSS
     $primary-color: #007bff;
     body {
         color: $primary-color;
     }
     ```

### 3. **Nesting:**
   - **CSS:** Selectors are not nested.
   - **SCSS:** Allows nesting of selectors.
     ```scss
     // SCSS
        nav {
            ul {
                margin: 0;
                padding: 0;
                list-style: none;

                li {
                    display: inline-block;
                    a {
                        text-decoration: none;
                        &:hover {
                            color: #007bff;
                        }
                    }
                }
            }
        }
     // CSS
        /* Compiled CSS */
        nav {
            ul {
                margin: 0;
                padding: 0;
                list-style: none;
            }

            nav ul li {
                display: inline-block;
            }

            nav ul li a {
                text-decoration: none;
            }

            nav ul li a:hover {
                color: #007bff;
            }
        }

     ```

### 4. **Partials and Importing:**
   - **CSS:** No concept of partials or importing.
   - **SCSS:** Supports partials and importing.
     ```scss
     // SCSS - _variables.scss
     $primary-color: #007bff;

     // SCSS - main.scss
     @import 'variables';
     body {
         color: $primary-color;
     }
     ```

### 5. **Mixins:**
   - **CSS:** No native mixin support.
   - **SCSS:** Supports mixins for reusable blocks of styles.
     ```scss
     // SCSS
     @mixin border-radius($radius) {
         -webkit-border-radius: $radius;
         -moz-border-radius: $radius;
         border-radius: $radius;
     }

     button {
         @include border-radius(5px);
     }
     ```

### 6. **Inheritance:**
   - **CSS:** No native inheritance support.
   - **SCSS:** Supports inheritance with `@extend`.
     ```scss
     // SCSS
     .error {
         border: 1px solid #ff0000;
         color: #ff0000;
     }

     .critical-error {
         @extend .error;
         font-weight: bold;
     }
     ```

### 7. **Operators:**
   - **CSS:** No native mathematical operators.
   - **SCSS:** Supports mathematical operators.
     ```scss
     // SCSS
     $base-font-size: 16px;
     p {
         font-size: $base-font-size * 1.5;
     }
     ```

### 8. **Comments:**
   - **CSS:** Uses `/* */` for comments.
   - **SCSS:** Supports both `//` and `/* */` for comments.
     ```scss
     // This is a single-line comment in SCSS
     /* This is a multi-line comment in SCSS */
     ```

### 9. **Conditional Statements:**
   - **CSS:** No native support for conditionals.
   - **SCSS:** Supports `@if`, `@else if`, and `@else` for conditionals.
     ```scss
     // SCSS
     $theme: light;

     button {
         @if $theme == light {
             background-color: #fff;
             color: #333;
         } @else {
             background-color: #333;
             color: #fff;
         }
     }
     ```

### 10. **Loops:**
   - **CSS:** No native support for loops.
   - **SCSS:** Supports `@for` and `@each` for loops.
     ```scss
     // SCSS
     @for $i from 1 through 3 {
         .item-#{$i} {
             width: 100px * $i;
         }
     }
     ```

### 11. **Importance of Semicolons:**
   - **CSS:** Requires semicolons at the end of each statement.
   - **SCSS:** Semicolons are optional in SCSS.
     ```scss
     // SCSS
     body {
         color: #333
     }
     ```

### 12. **Browser Compatibility:**
   - **CSS:** Widely supported.
   - **SCSS:** Requires a preprocessor (sass) for browser compatibility.
