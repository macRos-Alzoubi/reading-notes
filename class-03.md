# HTML CSS & JS

- ## Ordered lists

  are lists where each item in the list is
  numbered. For example, the list might be a set of steps for
  a recipe that must be performed in order, or a legal contract
  where each point needs to be identified by a section
  number.

  - The ordered list is created with
    the `<ol>` element.

  - Each item in the list is placed
    between an opening `<li>` tag
    and a closing `</li>` tag. (The li
    stands for list item.)

- ## Unordered lists

  are lists that begin with a bullet point
  (rather than characters that indicate order).

  - The unordered list is created
    with the `<ul>` element.

  - Each item in the list is placed
    between an opening `<li>` tag
    and a closing `</li>` tag. (The li
    stands for list item.)

- ## Definition lists

  are made up of a set of terms along with the
  definitions for each of those terms.

  - The definition list is created with
    the `<dl>` element and usually
    consists of a series of terms and
    their definitions.

  - `<dt>` This is used to contain the term
    being defined (the definition
    term).

  - `<dd>` This is used to contain the
    definition.

- ## Nested Lists

  You can put a second list inside
  an `<li>` element to create a sublist
  or nested list.

  - i.g

  ```HTML
    <ul>
        <li>
            <ul>
                <li>
                    text
                </li>
            </ul>
        </li>
    </ul>
  ```

## HTML BOX

By default a box is sized just big
enough to hold its contents. To
set your own dimensions for a
box you can use the `height` and
`width` properties.

- ### Limting Width

  Some page designs expand and
  shrink to fit the size of the user's
  screen. In such designs, the
  `min-width` property specifies
  the smallest size a box can be
  displayed at when the browser
  window is narrow, and the
  `max-width` property indicates
  the maximum width a box can
  stretch to when the browser
  window is wide.

- ### Limting Height

  In the same way that you might
  want to limit the width of a box
  on a page, you may also want
  to limit the height of it. This is
  achieved using the `min-height`
  and `max-height` properties.

- ### Overflowing Content

  The overflow property tells the
  browser what to do if the content
  contained within a box is larger
  than the box itself. It can have
  one of two values:

  - #### `hidden`

  This property simply hides any
  extra content that does not fit in
  the box.

  - #### `scroll`

  This property adds a scrollbar to
  the box so that users can scroll
  to see the missing content.

- ### Border, Padding and Border

  - #### Border

    Every box has a border (even if
    it is not visible or is specified to
    be 0 pixels wide). The border
    separates the edge of one box
    from another.

  - #### Margin

    Margins sit outside the edge
    of the border. You can set the
    width of a margin to create a
    gap between the borders of two
    adjacent boxes.

  - #### Padding

    Padding is the space between
    the border of a box and any
    content contained within it.
    Adding padding can increase the
    readability of its contents.

- ### Centering Content

  If you want to center a box on
  the page (or center it inside
  the element that it sits in), you
  can set the `left-margin` and
  `right-margin` to auto.

  The `text-align` property is
  inherited by child elements. You
  therefore also need to specify
  the `text-align` property on the
  centered box if you do not want
  the text inside it to be centered.

- ### Display Propety

  The display property allows
  you to turn an inline element
  into a block-level element or vice
  versa, and can also be used to
  hide an element from the page.
  The values this property can
  take are:

  - #### inline

    This causes a block-level
    element to act like an `inline`
    element.

  - #### block

    This causes an inline element to
    act like a `block-level` element.

  - #### inline-block

    This causes a `block-level`
    element to flow like an inline
    element, while retaining other
    features of a `block-level` element.

  - #### none

    This hides an element from the
    page. In this case, the element
    acts as though it is not on the
    page at all (although a user could
    still see the content of the box if
    they used the view source option
    in their browser).

- ### Visibilty

  The visibility property allows
  you to hide boxes from users
  but It leaves a space where the
  element would have been.
  This property can take two
  values:

  - #### hidden

    This hides the element.

  - #### visible

    This shows the element.

## Javascript

- ### Logical Operators

  - #### Logical AND `&&`

    This oprator tests more than one condition.

    Both of the condition must be true in order evaluate to `True`

    - i.g `((10 < 2) && (2 <= 2))`

  - #### Logical OR `||`

    This oprator tests at least one condetion.

    In order to Evaluate to `True` at least one of the condetions must be `True`.

    - i.g `((10 < 2) || (2 <= 2))`

  - #### Logical NOT `!`

    This operator tacks a single Boolean value and inverts it.

    - i.g `!(5 > 2)`

- ### If Statment

  If statment evaaluates a condition, If the condition evaluates to `true`, any statment in the subsequent code block are executed.

  - **Structure**

    ```js
    if (condition1) {
      //  block of code to be executed if condition1 is true
    } else if (condition2) {
      //  block of code to be executed if the condition1 is false and condition2 is true
    } else {
      //  block of code to be executed if the condition1 is false and condition2 is false
    }
    ```

- ### Switch Statment

  The `switch` statement is used to perform different actions based on different conditions.

  Use the `switch` statement to select one of many code blocks to be executed.

  - **Structure**

    ```js
    switch (expression) {
      case x:
        // code block
        break;
      case y:
        // code block
        break;
      default:
      // code block
    }
    ```

- ### Loops

  Loop check condition. If it returns`true`, A code block will run.Then the condition will be checked agine if it still returns `true`, The code will run agine.

  There are three types of loops:

  - **For**

    If you need to run code a specific nuber of time, User `for` loop.

  - **While**

    If you don't know how many time you wante to run the code, Use `while` loop.

  - **do while**

    The `do/while` loop is a variant of the `while` loop. This loop will execute the code block once, before checking if the condition is true, then it will repeat the loop as long as the condition is true.
