## Specificity
- 4 numbers
  - important, #ids, #classes, #elements
  - the selector with the highest left most value is chosen
    - eg: 0, 1, 0, 1 has more specificity than 0, 0, 999, 100

## Pseudo classes
- focus-visible
- disabled
  - eg: button:disabled
- checked
  - eg: input:checked
- first-child
  - eg: body :first-child => all first children inside the body

## Box Model
- Margins collapse => between two elements only the largest margin is used
- box-sizing
  - border-box: then width and height will be such that the border + padding + content's width and height
  - content-box: only for the content's width and height
  - to use this for all elements in the page, we can do something like
    - <code>* {
        &nbsp;&nbsp;&nbsp;&nbsp;box-sizing: border-box;
    }</code>

## Font sizing
- Preferable to use **rem** to **em** as **rem** depends upon the root font size and if someone zooms in, then our font automatically scales accordingly if **rem** is used
- one use case for **em** is when we want to scale our padding based on the font size
- **%** are exactly equal to **em**
  - 1em <=> 100%
  - 2em <=> 200%