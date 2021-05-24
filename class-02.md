# HTML Text

- ## Structural markup & Semantic markup:

  - ### **Structural markup**:

    he elements that you can use to
    describe both headings and paragraphs.

  - ### **Semantic markup**:

    which provides extra information; such
    as where emphasis is placed in a sentence, that something
    you have written is a quotation (and who said it), the
    meaning of acronyms, and so on.

- ## Headings:

  HTML has six "levels" of headings.

  Browsers display the contents of
  headings at different sizes. The
  contents of an `<h1>` element is
  the largest, and the contents of
  an `<h6>` element is the smallest.

- ## Paragraphs:

  To create a paragraph, surround
  the words that make up the
  paragraph with an opening `<p>`
  tag and closing `</p>` tag.
  By default, a browser will show
  each paragraph on a new line
  with some space between it and
  any subsequent paragraphs.

- ## Bold & Italic:

  - ### Bold:

    By enclosing words in the tags
    `<b>` and `</b>` we can make
    characters appear bold.

    The `<b>` element also represents
    a section of text that would be
    presented in a visually different
    way (for example key words in a
    paragraph) although the use of
    the `<b>` element does not imply
    any additional meaning.

  - ### Italic:

    By enclosing words in the tags
    `<i>` and `</i>` we can make
    characters appear italic.
    The `<i>` element also represents
    a section of text that would be
    said in a different way from
    surrounding content — such as
    technical terms, names of ships,
    foreign words, thoughts, or other
    terms that would usually be
    italicized.

- ## Line Break & Horizantal Rules:

  - ### Line Break:

    As you have already seen, the
    browser will automatically show
    each new paragraph or heading
    on a new line. But if you wanted
    to add a line break inside the
    middle of a paragraph you can
    use the line break tag `<br/>`.

  - ### Horizantal Rules:

    To create a break between
    themes — such as a change of
    topic in a book or a new scene
    in a play — you can add a
    horizontal rule between sections
    using the `<hr/>` tag.

# CSS

**CSS** allows you to create rules that specify how the content of
an element should appear in a web document.

- ## External CSS

  The `<link>` element can be used
  in an HTML document to tell the
  browser where to find the CSS
  file used to style the page. It is an
  empty element (meaning it does
  not need a closing tag), and it
  lives inside the `<head>` element.
  It should use three attributes:

  - ### **href**:

    This specifies the path to the
    CSS file (which is often placed in
    a folder called css or styles).

  - ### **type**:

    This attribute specifies the type
    of document being linked to. The
    value should be text/css.

  - ### **rel**:

    This specifies the relationship
    between the HTML page and
    the file it is linked to. The value
    should be stylesheet when
    linking to a CSS file.

- ## Internal CSS

  You can also include CSS rules
  within an HTML page by placing
  them inside a `<style> element`,
  which usually sits inside the
  `<head>` element of the page.

  - i.g:

    ```
    <head>
    <title>Using Internal CSS</title>
        <style type="text/css">
            body {
                font-family: arial;
                background-color: rgb(185,179,175);
            }

            h1 {
                color: rgb(255,255,255);
            }
        </style>
    </head>
    ```

- ## CSS Selector

  1. **Universal Selector** `* {}`

     - Applies to all elements in the document.

  2. **Type selector** `h1, h2, h3, div{}`

     - Matches element names.

  3. **class selsector** `.plane {}`

     - Matches an element whose
       class attribute has a value that
       matches the one specified after
       the period (or full stop) symbol.

  4. **ID Selector** `#main-footer {}`

     - Matches an element whose
       id attribute has a value that
       matches the one specified after
       the pound or hash symbol

  5. **Child Selector** `li>a {}`

     - Matches an element that is a
       descendent of another specified
       element (not just a direct child of
       that element).

  6. **Descendant Selector** `p a {}`

     - Matches an element that is a
       descendent of another specified
       element (not just a direct child of
       that element).

  7. **Adjacent Sebling Selector** `h1+p {}`

     - Matches an element that is the
       next sibling of another.

  8. **General Sebling Selector** `h1~p {}`

     - Matches an element that is a
       sibling of another, although it
       does not have to be the directly
       preceding element.

# Javascript

- ## Statments

  A script is a series of instructions that a computer can follow one-by-one.
  Each individual instruction or step is known as a **statement**.
  Statements should end with a semicolon.

  - STATEMENTS ARE INSTRUCTIONS AND
    EACH ONE STARTS ON A NEW LINE.

  - STATEMENTS CAN BE ORGANIZED
    INTO CODE BLOCKS.

- ## Comments

  You should write comments to explain what your code does.
  They help make your code easier to read and understand.
  This can help you and others who read your code.

  - Single line Comment `// comment gose here`.
  - Multi line Comment `/* comment gose here */`

- ## What is variable?

  JavaScript variables are containers for storing data values.

  - i.g `let salary = '3000$'`

- ## How to declare a variable

  - We use first the keyword `var` , `let` or `const`.

    - The variable declared with `var` or `let` can be mutated (Changed).
    - The variable declared with `const` it can't be mutated (Changed).

  - The we give the variable a name, There is some rolse
    we have to follow:

    - Can't start with **nubers** or **special symbols** except the `_`.

- ## How to Assign a value to the variable

  We use the `=` symbol to give the variable a value

  -i.g `let name = 'Ali'`

- ## Data Types

  - Numeric data type

    The numeric data type handles
    numbers. `0.9`

  - String data type

    The strings data type consists of
    letters and other characters. `'hj_='`

  - Boolean data type

    Boolean data types can have one
    of two va lues: true or false. `false, true`

- ## Using comparison oprator

  - `>` greater than retun `true` if the left side is greater
    than right side otherwise it return `false`.

  - `<` less than retun `true` if the left side is less
    than right side otherwise it return `false`.

  - `>=` greater than or equal retun `true` if the left side is
    greater than right side otherwise it return `false`.

  - `<=` less than or equal retun `true` if the left side is
    greater than right side otherwise it return `false`.

  - `==` check the equalty of two variables if are equal
    it will return `true` otherwise `false`.

  - `!=` check the inequalty of two variables if are equal
    it will return `true` otherwise `false`.
