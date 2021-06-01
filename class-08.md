# HTML Layout

- ## Layout

  - ### Building Blocks

    CSS treats each HTML element as if it is in its
    own box. This box will either be a block-level
    box or an inline box.

    `Block-level boxes` start on a **new line** and act as the main building blocks of any **layout**, while `inline boxes` **flow between surrounding text**. You can control how much space each box takes up by setting the **width** of the boxes (and sometimes the height, too). To separate boxes, you can use `borders`, `margins`, `padding`, and `background` `colors`.

    - #### Block-level elements

      start on a new line

      - ##### Examples include

        `<h1> <p> <ul> <li>`

    - #### Inline elements

      flow in between surrounding text

      - ##### Examples include

        `<img> <b> <i>`

  - ### Containing Elements

    **If one block-level element sits inside another
    block-level element then the outer box is
    known as the containing or parent element.**

    It is common to group a number of elements together inside a `<div>`
    (or other block-level) element. For example, you might group together all of the elements that form the header of a site (such as the logo and the main navigation). The `<div>` element that contains this group of elements is then referred to as the containing element.

  - ### Controll ing the Position of Elements

    **CSS has the following ***positioning schemes*** that allow you to control the layout of a page: normal flow, relative positioning, and absolute positioning. You specify the positioning scheme using the position property in CSS. You can also float elements using the float property.**

    - #### Normal flow

      Every `block-level` element appears on a new line, causing
      each item to appear lower down the page than the previous one.
      Even if you specify the width of the `boxes` and there is space
      for two elements to sit side-byside, they will not appear next
      to each other. This is the default behavior (unless you tell the
      browser to do something else).


    - #### Relative Positioning

      This moves an element from the position it would be in normal
      flow, shifting it to the top, right, bottom, or left of where it
      would have been placed. This does not affect the position of
      surrounding elements; they stay in the position they would be in
      in normal flow.

    - #### Absolute positioning

      This positions the element in relation to its containing
      element. It is taken out of normal flow, meaning that it
      does not affect the position of any surrounding elements
      (as they simply ignore the space it would have taken up).
      Absolutely positioned elements move as users scroll up and
      down the page.

    - #### Fixed Positioning

      This is a form of absolute positioning that positions
      the element in relation to the browser window, as opposed
      to the containing element. Elements with fixed positioning
      do not affect the position of surrounding elements and they
      do not move when the user scrolls up or down the page.

    - #### Floating Elements

      Floating an element allows you to take that element out
      of normal flow and position it to the far left or right of a
      containing box. The floated element becomes a block-level
      element around which other content can flow.

      - #### Using Float to Place Elements Side-by-Side

        A lot of layouts place boxes
        next to each other. The float
        property is commonly used to
        achieve this.
        When elements are floated, the
        height of the boxes can affect
        where the following elements sit.

      - #### Clearing Floats

        The clear property allows you
        to say that no element (within
        the same containing element)
        should touch the left or righthand
        sides of a box. It can take
        the following values:

          - `left`

            The left-hand side of the box
            should not touch any other
            elements appearing in the same
            containing element.

          - `right`

            The right-hand side of the
            box will not touch elements
            appearing in the same containing
            element.

          - `both`

            Neither the left nor right-hand
            sides of the box will touch
            elements appearing in the same
            containing element.

          - `none`

            Elements can touch either side.

      - #### Parents of Floated Elements: Problem

        If a containing element only
        contains floated elements, some
        browsers will treat it as if it is
        zero pixels tall.

      - #### Parents of Floated Elements: Solution

        Traditionally, developers got
        around this problem by adding
        an extra element after the
        last floated box (inside the
        containing element). A CSS
        rule would be applied to this
        additional element setting the
        clear property to have a value
        of both. But this meant that an
        extra element was added to the
        HTML just to fix the height of the
        containing element.

        More recently, developers have
        opted for a purely CSS-based
        solution because it means that
        there is no need to add an extra
        element to the HTML page after
        the floated elements. The pure
        CSS solution adds two CSS rules
        to the containing element:
        - The overflow property is
        given a value auto.
        - The width property is set to
        100%.

      - #### Creating Multi-Column Layouts with Floats

        Many web pages use multiple
        columns in their design. This
        is achieved by using a `<div>`
        element to represent each
        column. The following three CSS
        properties are used to position
        the columns next to each other:

        - `width`

          This sets the width of the columns.

        - `float`

          This positions the columns next to each other.

        - `margin`

          This creates a gap between the columns.

    - ### Screen Sizes

      Different visitors to your site will have different sized screens that show different amounts of information, so your design needs to be able to work on a range of different sized screens.

    - ### Screen Resolution

      Resolution refers to the number of dots a screen shows per inch. Some devices have a higher resolution than desktop computers and most operating systems allow users to adjust the resolution of their screens.

    - ### Page Sizes

      Because screen sizes and display resolutions vary so much, web designers often try to create pages of around 960-1000 pixels wide (since most users will be able to see designs this wide on their screens).

    - ### Fixed Width Layouts

      Fixed width layout
    designs do not
    change size as the
    user increases
    or decreases
    the size of their
    browser window.
    Measurements tend
    to be given in pixels.

      - #### Advantages

        - Pixel values are accurate
        at controlling size and
        positioning of elements.

        - The designer has far greater
        control over the appearance
        and position of items on the
        page than with liquid layouts.

        - You can control the lengths
        of lines of text regardless of
        the size of the user's window.

        - The size of an image will
        always remain the same
        relative to the rest of the
        page.

      - #### Disadvantages

        - You can end up with big gaps
        around the edge of a page.

        - If the user's screen is a much
        higher resolution than the
        designer's screen, the page
        can look smaller and text can
        be harder to read.

        - If a user increases font sizes,
        text might not fit into the
        allotted spaces.

        - The design works best on
        devices that have a site or
        resolution similar to that of
        desktop or laptop computers.

        - The page will often take up
        more vertical space than a
        liquid layout with the same
        content.

    - ### Liquid Layouts

      Liquid layout designs
    stretch and contract
    as the user increases
    or decreases the
    size of their browser
    window. They tend to
    use percentages.

      - #### Advantages

        - Pages expand to fill the entire
        browser window so there are
        no spaces around the page
        on a large screen.

        - If the user has a small
        window, the page can
        contract to fit it without the
        user having to scroll to the
        side.

        - The design is tolerant of
        users setting font sizes larger
        than the designer intended
        (because the page can
        stretch).

      - #### Disadvantages

        - If you do not control the
        width of sections of the page
        then the design can look very
        different than you intended,
        with unexpected gaps around
        certain elements or items
        squashed together.

        - If the user has a wide
        window, lines of text can
        become very long, which
        makes them harder to read.

        - If the user has a very narrow
        window, words may be
        squashed and you can end up
        with few words on each line.

    - ### A Fixed Width Layout

      To create a fixed width layout,
    the **width** of the **main boxes** on
    a page will usually be specified
    in **pixels** (and sometimes their
    height, too).

      The fixed width layout will stay
    the same width no matter what
    size the browser window is,
    whereas the liquid layout will
    stretch (or shrink) to fill the
    screen.

    - ### A Liquid Layout

      The liquid layout uses
    **percentages** to specify the **width**
    of each box so that the design
    will stretch to fit the size of the
    screen.
    
    - ### Layout Grids

      Composition in any visual art (such as design, painting, or photography) is the placement or arrangement of visual elements — how they are organized on a page. Many designers use a grid structure to help them position items on a page, and the same is true for web designers.

      Grids set consistent proportions
    and spaces between items which
    helps to create a professional
    looking design.