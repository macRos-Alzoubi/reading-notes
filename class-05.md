# HTML

## Adding Images

  To add an image into the page
  you need to use an `<img>`
  element. This is an empty
  element (which means there is
  no closing tag). It must carry the
  following two attributes:

- ### `src`

    This tells the browser where
    it can find the image file. This
    will usually be a relative URL
    pointing to an image on your
    own site. (Here you can see that
    the images are in a child folder
    called images — relative URLs
    were covered on pages 83-84).

- ### `alt`

    This provides a text description
    of the image which describes the
    image if you cannot see it.

- ### `title`

    You can also use the title
    attribute with the `<img>` element
    to provide additional information
    about the image. Most browsers
    will display the content of this
    attribute in a tootip when the
    user hovers over the image.

## Height & Width of Images

- ### `height`

    This specifies the height of the
    image in pixels.

- ### `width`

    This specifies the width of the
    image in pixels.

## Three Rules for Creating Images

  1. Save images in the right format

      Websites mainly use images in
      jpeg, gif, or png format. If you
      choose the wrong image
      format then your image might
      not look as sharp as it should
      and can make the web page
      slower to load.

  2. Save images at the right size

     You should save the image at
     the same width and height it will
     appear on the website. If
     the image is smaller than the
     width or height that you have
     specified, the image can be
     distorted and stretched. If the
     image is larger than the width
     and height if you have specified,
     the image will take longer to
     display on the page.

  3. Use the correct resolution

     Computer screens are made up
     of dots known as pixels. Images
     used on the web are also made
     up of tiny dots. Resolution refers
     to the number of dots per inch,
     and most computer screens only
     show web pages at 72 pixels
     per inch. So saving images at
     a higher resolution results in
     images that are larger than
     necessary and take longer to
     download.

## Tools to Edit & Save Images

  The most popular tool amongst
  web professionals is Adobe
  Photoshop. (In fact, professional
  web designers often use this
  software to design entire sites.)
  The full version of Photoshop is
  expensive, but there is a cheaper
  version called Photoshop
  Elements which would suit the
  needs of most beginners.

## Image Formats

- ### JPEG

    Whenever you have many different
    colors in a picture you should use a `JPEG`.

- ### GIF

    Use `GIF` or `PNG` format
    when saving images
    with few colors or large
    areas of the same color.

## Vector Images

  Vector images differ from bitmap images and
  are resolution-independent. Vector images are
  commonly created in programs such as Adobe
  Illustrator.

- ### Scalable Vector Graphics (SVG)

    are a relatively new format used
    to display vector images directly
    on the web (eliminating the need
    to create bitmap versions of
    them), however its use is not yet
    widespread.

## Animated GIFs

  Animated GIFs show several frames of an
  image in sequence and therefore can be used to
  create simple animations.

## HTML5 Figure and Figure Caption

  Images often come with
  captions. HTML5 has introduced
  a new <`figure>` element to
  contain images and their caption
  so that the two are associated.
  You can have more than one
  image inside the `<figure>`
  element as long as they all share
  the same caption.

  The `<figcaption>` element has
  been added to HTML5 in order
  to allow web page authors to add
  a caption to an image.

## COLOR

  - ### Foreground Color

    The color property allows you
    to specify the color of text inside
    an element. You can specify any
    color in CSS in one of three ways:

      - ### rgb values

        These express colors in terms
        of how much red, green and
        blue are used to make it up. For
        example: `rgb(100,100,90)`.

    - ### hex codes

        These are six-digit codes that
        represent the amount of red,
        green and blue in a color,
        preceded by a pound or hash `#`
        sign. For example: `#ee3e80`

    - ### color names

        There are 147 predefined color
        names that are recognized
        by browsers. For example:
        `DarkCyan`.

  - ### Background Color

    - ### background-color

      CSS treats each `HTML` element
      as if it appears in a box, and the
      `background-color` property
      sets the color of the background
      for that box.
      You can specify your choice of
      background color in the same
      three ways you can specify
      foreground colors: `RGB values`,
      `hex codes`, and `color names`.

  - ### Contrast

    When picking foreground and background
    colors, it is important to ensure that there is
    enough contrast for the text to be legible.

    - ### Low Contrast

      Text is harder to read when
      there is low contrast between
      background and foreground
      colors.

      For long spans of text, reducing
      the contrast a little bit improves
      readability.

    - ### High Contrast

      Text is easier to read when
      there is higher contrast between
      background and foreground
      colors.

      If you want people to read a lot
      of text on your page, however,
      then too much contrast can
      make it harder to read, too.

    - ### Medium Contrast

      For long spans of text, reducing
      the contrast a little bit improves
      readability.

      You can reduce contrast by
      using dark gray text on a white
      background or an off-white text
      on a dark background.

  - ### CSS 3: Opacity

    - ### opacity, rgba

      CSS3 introduces the opacity
      property which allows you to
      specify the opacity of an element
      and any of its child elements.
      The value is a number between
      0.0 and 1.0 (so a value of 0.5
      is 50% opacity and 0.15 is 15%
      opacity).

      The CSS3 rgba property allows
      you to specify a color, just like
      you would with an RGB value,
      but adds a fourth value to
      indicate opacity. This value is
      known as an alpha value and is
      a number between 0.0 and 1.0
      (so a value of 0.5 is 50% opacity
      and 0.15 is 15% opacity). The
      rgba value will only affect the
      element on which it is applied
      (not child elements).

## TEXT

  - ### Typeface Terminology

    - ### Serif

      Serif fonts have extra details on
      the ends of the main strokes of
      the letters. These details are
      known as serifs.

    - ### Sans-Serif

      Sans-serif fonts have straight
      ends to letters, and therefore
      have a much cleaner design.

    - ### Monospace

      Every letter in a monospace (or
      fixed-width) font is the same
      width. (Non-monospace fonts
      have different widths.)

  - ### Specifying Typefaces

    The `font-family` property
    allows you to specify the
    `typeface` that should be used for
    any text inside the element(s) to
    which a `CSS` rule applies.
    The value of this property is the
    name of the typeface you want
    to use.

  - ### Size Of Type

    The `font-size` property enables
    you to specify a size for the
    font. There are several ways to
    specify the size of a font. The
    most common are:

    - ### **pixels**

      Pixels are commonly used
      because they allow web
      designers very precise control
      over how much space their text
      takes up. The number of pixels is
      followed by the letters px.

    - ### **percentages**

      The default size of text in
      browsers is 16px. So a size of
      75% would be the equivalent of
      12px, and 200% would be 32px.

    - ### **ems**

      An em is equivalent to the width


  - ### `@font-face`

    `@font-face` allows you to use
    a font, even if it is not installed
    on the computer of the person
    browsing, by allowing you to
    specify a path to a copy of the
    font, which will be downloaded if
    it is not on the user's machine.

    Because this technique allows
    a version of the font to be
    downloaded to the user's
    computer, it is important that the
    license for the font permits it to
    be used in this way.

  - ### `font-weight`

    The `font-weight` property
    allows you to create bold text.
    There are two values that this
    property commonly takes:

    -  ### `normal`

      This causes text to appear at a
      normal weight.

    - ### `bold`

      This causes text to appear bold.

  - ### `font-style`

    - ### `normal`

      This causes text to appear in a
      normal style (as opposed to italic
      or oblique).

    - ### `italic`

      This causes text to appear italic.

    - ### `oblique`

      This causes text to appear
      oblique.

  - ### `text-transform`

    The text-transform property
    is used to change the case of
    text giving it one of the following
    values:

    - ### `uppercase`

      This causes the text to appear
      uppercase.

    - ### `lowercase`

      This causes the text to appear
      lowercase.

    - ### `capitalize`

      This causes the first letter of
      each word to appear capitalized.