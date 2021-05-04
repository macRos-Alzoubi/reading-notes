# CSS
CSS (Cascading Style Sheets) is a language for specifying how documents are presented to users — how they are styled, laid out, etc.

- **CSS syntax**:
CSS is a rule-based language, You define rules specifying groups of styles that should be applied to particular elements or groups of elements on your web page.
  - i.g: ``` selector { role: value } , header idv{ color: #fff}```

- **How To Add CSS**:
  Three Ways to Insert CSS
    1. External CSS
      With an external style sheet, you can change the look of an entire website by changing just one file!
      Each HTML page must include a reference to the external style sheet file inside the 
      - ```<link>``` element, inside the head section.
      ``` <head><link rel="stylesheet" href="mystyle.css"></head>```
    2. **Internal CSS**:
      An internal style sheet may be used if one single HTML page has a unique style.
      The internal style is defined inside the 
       -
        ``` 
       <head>
        <style>
          body {
            background-color: linen;
          }
          h1 {
          color: maroon;
          margin-left: 40px;
          }
          </style>
        </head>
         ```
    3. **Inline CSS**:
      An inline style may be used to apply a unique style for a single element.
      To use inline styles, add the style attribute to the relevant element. The style attribute can contain any CSS property.
        - 
        ``` 
        <h1 style="color:blue;text-align:center;">This is a heading</h1>
        <p style="color:red;">This is a paragraph.</p>
         ```
- **CSS color Property**:
  The color property can be applied by a different Ways
  1. Name value: i.g ``` body { color: red;} ```
  2. Hexadecimal value: i.g ``` body { color: #ff0000;} ```
  3. RGB value: i.g ``` body { color: rgb(255, 0, 0);} ```
  4. RGBA value: i.g ``` body { color: rgba(255, 0, 0, 0);} ```
  5. HSL value: i.g ``` body { color: hsl(89, 43%, 51%);} ``` 
  6. HSLA value: i.g ``` body {color: hsla(89, 43%, 51%, 0.6);} ``` 
