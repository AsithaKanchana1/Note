### Study Note: CSS Concepts and Practical Examples

---

#### **Color Representation in CSS**

- **Hexadecimal Method**:
  - Colors are represented as `#RRGGBB` where `RR`, `GG`, and `BB` are two-digit hexadecimal numbers.
  - Example: `#FF5733` represents a color with full red, moderate green, and low blue.

- **RGBA Method**:
  - Colors are represented as `rgba(R, G, B, A)` where `R`, `G`, and `B` range from 0 to 255, and `A` (alpha) ranges from 0 (completely transparent) to 1 (completely opaque).
  - Example: `rgba(255, 87, 51, 0.5)` represents a semi-transparent color.

#### **Creating and Using External CSS**

- **External CSS**:
  - Store styles in a separate `.css` file and link it to the HTML file.
  - Example:
    ```css
    /* external.css */
    p {
      color: red;
      text-align: center;
    }
    ```
    ```html
    <!-- external.html -->
    <link rel="stylesheet" href="external.css">
    <p>This is a paragraph.</p>
    ```

#### **Box Model in CSS**

- **Box Model Components**:
  - Content
  - Padding: Space inside the element, around the content.
  - Border: The edge surrounding the padding.
  - Margin: Space outside the border.

- **Example**:
  ```css
  .box {
    width: 200px;
    height: 100px;
    padding: 20px;
    border: 5px solid black;
    margin: 15px;
    background-color: lightblue;
    text-align: center;
  }
  ```
  ```html
  <div class="box">This is a box.</div>
  ```

#### **CSS Selectors**

- **Class Selector**: Prefixed with `.` (dot).
  - Example:
    ```css
    .classname {
      color: blue;
    }
    ```
    ```html
    <p class="classname">This text is blue.</p>
    ```

#### **Styling HTML Tables**

- **Example**:
  ```css
  table {
    width: 100%;
    border-collapse: collapse;
  }
  th, td {
    border: 1px solid black;
    padding: 8px;
    text-align: center;
  }
  th {
    background-color: #f2f2f2;
  }
  ```
  ```html
  <table>
    <tr>
      <th>Header 1</th>
      <th>Header 2</th>
    </tr>
    <tr>
      <td>Data 1</td>
      <td>Data 2</td>
    </tr>
  </table>
  ```

#### **Opacity in CSS**

- **Setting Opacity**:
  - Ranges from `0` (completely transparent) to `1` (completely opaque).
  - Example:
    ```css
    .transparent-box {
      background-color: blue;
      opacity: 0.5;
    }
    ```
    ```html
    <div class="transparent-box">This box is semi-transparent.</div>
    ```

#### **Creating Dropdowns in CSS**

- **Example**:
  ```css
  .dropdown {
    position: relative;
    display: inline-block;
  }
  .dropdown-content {
    display: none;
    position: absolute;
    background-color: #f9f9f9;
    box-shadow: 0px 8px 16px 0px rgba(0,0,0,0.2);
    z-index: 1;
  }
  .dropdown:hover .dropdown-content {
    display: block;
  }
  ```
  ```html
  <div class="dropdown">
    <button class="dropbtn">Dropdown</button>
    <div class="dropdown-content">
      <a href="#">Link 1</a>
      <a href="#">Link 2</a>
      <a href="#">Link 3</a>
    </div>
  </div>
  ```

#### **Practical Tips**

- **External CSS**:
  - Use for large projects to maintain consistency across multiple HTML files.
  
- **Box Model**:
  - Essential for understanding and controlling layout and spacing.

- **Selectors**:
  - Use class selectors to apply styles to specific elements efficiently.

- **Tables**:
  - Apply consistent styling for better readability and structure.

- **Opacity**:
  - Use to create overlay effects and adjust the transparency of elements.

- **Dropdowns**:
  - Enhance user interface with interactive elements.

---

These notes provide a concise overview of various CSS techniques and practices, helping to structure your study sessions effectively.