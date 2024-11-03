Advanced CSS selectors enable more precise and complex selections of elements within a document, allowing developers to apply styles based on specific conditions or structures. Here’s an overview of the various advanced CSS selector types:

### 1. Attribute Selectors
These selectors allow you to target elements based on their attributes or attribute values.

- **Starts with**: `[attribute^="value"]`
- **Ends with**: `[attribute$="value"]`
- **Contains**: `[attribute*="value"]`
- **Example**:
    ```css
    /* Selects links that start with "http" */
    a[href^="http"] {
      color: green;
    }
    
    /* Selects elements with titles that end with "-info" */
    [title$="-info"] {
      color: blue;
    }
    
    /* Selects elements with class names that contain "btn-" */
    [class*="btn-"] {
      background-color: orange;
    }
    ```

### 2. Pseudo-classes
Pseudo-classes are used to apply styles based on the dynamic states of elements or their position in the document structure.

- **Structural pseudo-classes**:
  - `:nth-child(n)`: Selects the nth child of a parent.
  - `:nth-of-type(n)`: Selects the nth element of a particular type.
  - `:first-child`, `:last-child`, `:only-child`, `:only-of-type`, `:empty`
- **Example**:
    ```css
    /* Selects every second paragraph */
    p:nth-child(2n) {
      background-color: lightgray;
    }

    /* Selects the last item in an unordered list */
    ul li:last-child {
      font-weight: bold;
    }
    ```

### 3. Pseudo-elements
Pseudo-elements style specific parts of an element, allowing for more granular control over styling.

- **Common pseudo-elements**:
  - `::before`: Inserts content before an element’s content.
  - `::after`: Inserts content after an element’s content.
  - `::first-letter`: Styles the first letter of an element.
  - `::first-line`: Styles the first line of an element.
- **Example**:
    ```css
    /* Adds a quotation mark before blockquote content */
    blockquote::before {
      content: '"';
    }
    
    /* Changes the first letter of a paragraph to uppercase */
    p::first-letter {
      font-size: 2em;
      font-weight: bold;
    }
    ```

### 4. Child and Sibling Combinators
These selectors enable you to target elements based on their relationship to other elements in the document hierarchy.

- **Child combinator**: `parent > child`
- **Adjacent sibling combinator**: `element1 + element2`
- **General sibling combinator**: `element1 ~ element2`
- **Example**:
    ```css
    /* Selects a direct child of a div */
    div > p {
      margin-top: 20px;
    }

    /* Selects the first <p> that immediately follows an <h2> header */
    h2 + p {
      color: darkblue;
    }

    /* Selects all <li> elements that are siblings of <h2> */
    h2 ~ li {
      color: green;
    }
    ```

### 5. Negation Pseudo-class
The `:not(selector)` pseudo-class selects elements that do not match the given selector.

- **Example**:
    ```css
    /* Selects all <div> elements that do not have the class `.special` */
    div:not(.special) {
      background-color: lightyellow;
    }
    ```

### 6. Functional Pseudo-classes
Functional pseudo-classes provide even more control over selections based on specific conditions.

- `:is(selector)`: Matches elements that match any of a list of selectors.
- `:where(selector)`: Similar to `:is()`, but has lower specificity.
- `:has(selector)`: Selects elements that contain a specified selector as a descendant.
- **Example**:
    ```css
    /* Applies to any element that matches either h1 or h2 */
    :is(h1, h2) {
      margin-bottom: 10px;
    }

    /* Selects any article that contains a p element */
    article:has(p) {
      border: 2px solid blue;
    }
    ```

### Summary
Advanced CSS selectors such as attribute selectors, pseudo-classes, pseudo-elements, combinators, and functional selectors greatly enhance your ability to target and style elements within a web page. By mastering these selectors, developers can create more efficient, maintainable, and responsive designs tailored to user interactions and page structures.
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTI1NTc1NjUxM119
-->