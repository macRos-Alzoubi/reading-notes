# HTML Forms and JS Events

## Forms

  - ### Why Forms?

    The best known form on the web is probably
    the search box that sits right in the middle of
    Google's homepage.

  - ### Form Controls

    There are several types of form controls that
    you can use to collect information from visitors
    to your site.

    - ### ADDING TEXT

      - #### Text input

         Used for a single line of text such as email addresses and names.

      - #### Password input

        Like a single line text box but it masks the characters entered.

      - #### Text area

        For longer areas of text, such as messages and comments.

    - ### Making Choices

      - #### Radio buttons

        For use when a user must select one of a number of options.

      - #### Checkboxes

        When a user can select and unselect one or more options.

      - #### Drop-down boxes

        When a user must pick one of a number of options from a list.

    - ### Submitting Forms:

      - #### Submit buttons

        To submit data from your form to another web page.

      - #### Image buttons

        Similar to submit buttons but they allow you to use an image.

      - #### File upload

        Allows users to upload files (e.g. images) to a website.

  - ### How Forms Work?

    1. A user fills in a form and then presses a button
    to submit the information to the server.

    2. The name of each formcontrol is sent to the
    server along with thevalue the user enters or selects.

    3. The server processes the information using a
    programming language such as `PHP`, `C#`, `VB.net`, or `Java`. It may also store the information in a database.

    4. The server creates a new page to send back to the
    browser based on the information received.

  - ### Form Structure

    - `<form>`

      Form controls live inside a `<form>` element. This element
    should always carry the action
    attribute and will usually have a
    method and id attribute too.

    - `action`

      Every `<form>`element requires
    an action attribute. Its value
    is the URL for the page on the
    server that will receive the
    information in the form when it
    is submitted.

    - `method`

      Forms can be sent using one of two methods: `get` or `post`.

    - ### Text Input

      - `<input>`

        The `<input>` element is used
        to create several different form
        controls. The value of the type
        attribute determines what kind
        of input they will be creating.

      - `type="text"`

        When the type attribute has a
        value of text, it creates a singleline
        text input.

      - `name`

        When users enter information
        into a form, the server needs to
        know which form control each
        piece of data was entered into.
        (For example, in a login form, the
        server needs to know what has
        been entered as the username
        and what has been given as the
        password.) Therefore, each form
        control requires a name attribute.
        The value of this attribute
        identifies the form control and is
        sent along with the information
        they enter to the server.

      - `maxlength`

        You can use the maxlength
        attribute to limit the number
        of characters a user may enter
        into the text field. Its value is the
        number of characters they may
        enter. For example, if you were
        asking for a year, the maxlength
        attribute could have a value of 4.

    - ### Password Input

      - `<input type="password">`

        When the type attribute has
        a value of password it creates
        a text box that acts just like a
        single-line text input, except
        the characters are blocked out.
        They are hidden in this way so
        that if someone is looking over
        the user's shoulder, they cannot
        see sensitive data such as
        passwords.

      - `name`

        The name attribute indicates
        the name of the password input,
        which is sent to the server with
        the password the user enters.

      - `size, maxlength`

        It can also carry the size and
        maxlength attributes like the
        the single-line text input.

    - ### TEXT AREA

      - `<textarea>`

        The `<textarea>` element
        is used to create a mutli-line
        text input. Unlike other input
        elements this is not an empty
        element. It should therefore have
        an opening and a closing tag.

        Any text that appears between
        the opening `<textarea>` and
        closing `</textarea>` tags will
        appear in the text box when the
        page loads.

    - ### Radio Button

      - `<input type="radio">`

        Radio buttons allow users to pick just one of a number of options.

      - `name`

        The name attribute is sent to
        the server with the value of the
        option the user selects. When
        a question provides users with
        options for answers in the form
        of radio buttons, the value of
        the name attribute should be the
        same for all of the radio buttons
        used to answer that question.

      - `value`

        The value attribute indicates
        the value that is sent to the
        server for the selected option.
        The value of each of the buttons
        in a group should be different
        (so that the server knows which
        option the user has selected).

      - `checked`

        The checked attribute can be
        used to indicate which value (if
        any) should be selected when
        the page loads. The value of this
        attribute is checked. Only one
        radio button in a group should
        use this attribute.

## Lists, Tables and Forms

  - ### Bullet Point Styles

    - `list-style-type`

      The list-style-type property
    allows you to control the shape
    or style of a bullet point (also
    known as a marker).
    It can be used on rules that
    apply to the `<ol>`, `<ul>`, and `<li>`
    elements.

    - ### Unordered Lists

        For an unordered list you can use
        the following values:
        - none
        - disc
        - circle
        - square

    - ### Ordered Lists

      For an ordered (numbered) list
      you can use the following values:

        - #### decimal `1 2 3`.

        - #### decimal-leading-zero `01 02 03`

        - #### lower-alpha `a b c`

        - #### upper-alpha `A B C`

        - #### lower-roman `i. ii. iii`

        - #### upper-roman `I II III`

  - ### Table Properties

    You have already met several
    properties that are commonly
    used with tables. Here we will
    put them together in a single
    example using the following:

    - `width`

      to set the width of the table

    - `padding`

      to set the space between the border of each table
    cell and its content

    - `text-transform`

      to convert the content of the table headers to
    uppercase

    - `letter-spacing, font-size`

      to add additional styling to the content of the table headers

    - `border-top, border-bottom`

      to set borders above and below
    the table headers

    - `text-align`

      to align the writing to the left of some table cells and
    to the right of the others

    - `background-color`

      to change the background color of the alternating table rows

    - `:hover`

      to highlight a table row when a user's mouse goes over it

  - ### Border on Empty Cells

    - `empty-cells`

      If you have empty cells in
    your table, then you can use
    the `empty-cells` property to
    specify whether or not their
    borders should be shown.

    - `show`

      This shows the borders of any empty cells.

    - `hide`

      This hides the borders of any empty cells.

    - `inherit`

      If you have one table nested
    inside another, the inherit
    value instructs the table cells to
    obey the rules of the containing
    table.

  - ### Gaps Between Cells

    The `border-spacing` property
    allows you to control the
    distance between adjacent cells.
    By default, browsers often leave
    a small gap between each table
    cell, so if you want to increase
    or decrease this space then
    the `border-spacing` property
    allows you to control the gap.

    border-collapse property.
    Possible values are:

    - `collapse`

      Borders are collapsed into a
    single border where possible.
    (border-spacing will be
    ignored and cells pushed
    together, and empty-cells
    properties will be ignored.)

    - `separate`

      Borders are detached from each
    other. (border-spacing and
    empty-cells will be obeyed.)

  - ### Styling Forms

    - ### Styling Text Inputs

      - `font-size`

        sets the size of the text entered by the user.

      - `color, background-color`

        `color` sets the text color, and `background-color` sets the background color of the input.

      - `border, border-radius`

        `border` adds a border around
        the edge of the input box, and
        `border-radius` can be used
        to create rounded corners (for
        browsers that support this
        property).

      - `:focus, :hover`

        The `:focus` pseudo-class is
        used to change the background
        color of the text input when it
        is being used, and the `:hover`
        psuedo-class applies the same
        styles when the user hovers over
        them.

      - `background-image`

        adds a background image to the box.
        Because there is a different
        image for each input, we are
        using an attribute selector
        looking for the value of the id
        attribute on each input.

    - ### Styling Submit Buttons

      - `color`

        `color` is used to change the color of the text on the button.

      - `text-shadow`

        text-shadow can give a 3D
        look to the text in browsers that
        support this property.

      - `border-bottom`

        has been used to make the bottom border of
        the button slightly thicker, which
        gives it a more 3D feel.

      - `background-color`

        can make
        the submit button stand out
        from other items around it.
        (Creating a consistent style
        for all buttons helps users
        understand how they should
        interact with the site.) A gradient
        background has been added for
        browsers that support gradients.

## Events

  - ### HOW EVENTS TRIGGER JAVASCRIPT CODE

    When the user interacts with the HTML on a web page, there are three steps involved in getting it to trigger some JavaScript code. Together these steps are known as event handling.

    1. Select t he elementnode(s) you want the
    script to respond to.

        For example, if you want to trigger a function when a user clicks on a specific link, you need to get the DOM node for that link element. You do this using a DOM query

    2. Indicate which event on the selected node(s) will
    trigger the response.

       Programmers call this binding a event to a DOM node.

    3. State the code you want to run when the event occurs.

  - ### THREE WAYS TO BIND AN EVENT TO AN ELEMENT

    1. HTML EVENT HANDLERS

        This is bad practice, but you
        need to be aware of it because
        you may see it in older code.

        Early versions of HTML included
        a set of attributes that could
        respond to events on the
        element they were added to.
        The attribute names matched
        the event names. Their values
        called the function that was to
        run when that event occurred.
        `i.g <a onclick="hide()">`

    2. TRADITIONAL DOM EVENT HANDLERS

        DOM event handlers were
        introduced in the original
        specification for the DOM.
        They are considered better than
        HTML event handlers because
        they let you separate the
        JavaScript from the HTML.

    3. **Event listeners** were introduced
        in an update to the DOM
        specification (DOM level 2,
        released in the year 2000).
        They are now the favored way of
        handling events.

        The syntax is quite different and,
        unlike traditional event handlers,
        these newer event listeners allow
        one event to trigger multiple
        functions. As a result, there
        are less likely to be conflicts
        between different scripts that
        run on the same page.

    