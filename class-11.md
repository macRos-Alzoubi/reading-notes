# HTML Images & Practical Information

## HTML Images

  - ## Controlling Sizes Of images in CSS

    You can control the size of an
    image using the `width` and
    `height` properties in CSS, just
    like you can for any other box.

    Specifying image sizes helps
    pages to load more smoothly
    because the HTML and CSS
    code will often load before the
    images, and telling the browser
    how much space to leave for an
    image allows it to render the rest
    of the page without waiting for
    the image to download.

  - ## AligNi ng images Using CSS

    1. The float property is added
    to the class that was created to
    represent the size of the image.

    2. New classes are created with
    names such as align-left or
    align-right to align the images
    to the left or right of the page.
    These class names are used in
    addition to classes that indicate
    the size of the image.

  - ## Centering images Using CSS

    By default, images are inline
    elements. This means that they
    flow within the surrounding text.
    In order to center an image, it
    should be turned into a blocklevel
    element using the display
    property with a value of block.

    Once it has been made into a
    block-level element, there are
    two common ways in which you
    can horizontally center an image:

    1. On the containing element,
    you can use the text-align
    property with a value of center.

    2. On the image itself, you can
    use the use the margin property
    and set the values of the left and
    right margins to auto.

  - ## Background Images

    - `background-image`

    The `background-image`
    property allows you to place
    an image behind any HTML
    element. This could be the entire
    page or just part of the page. By
    default, a background image will
    repeat to fill the entire box.

  - ## Repeating Images

    - `background-repeat, background-attachment`

      The` background-repeat` property can have four values:

       - `repeat`

         The background image is
        repeated both horizontally and
        vertically (the default way it
        is shown if the backgroundrepeat
        property isn't used).

          - `repeat-x`

            The image is repeated
            horizontally only (as shown in
            the first example on the left).

          - `repeat-y`

            The image is repeated vertically only.

          - `no-repeat`

            The image is only shown once.

      The `background-attachment`
      property specifies whether a
      background image should stay in
      one position or move as the user
      scrolls up and down the page. It
      can have one of two values:

        - `fixed`

          The background image stays in the same position on the page.

        - `scroll`

          The background image moves up and down as the user scrolls
          up and down the page.

  - ## Background Position

    - `background-position`

    When an image is not being
    repeated, you can use the
    background-position
    property to specify where in the
    browser window the background
    image should be placed.

    This property usually has a pair
    of values. The first represents
    the horizontal position and the
    second represents the vertical.

      - ### i.g

      ```css
      left top
      left center
      left bottom
      center top
      center center
      center bottom
      right top
      right center
      right bottom
      ```

  - ## shorthand for background property

    - `background`

      The background property acts
    like a shorthand for all of the
    other background properties
    you have just seen, and also the
    `background-color` property.

      The properties must be specified
    in the following order, but you
    can miss any value if you do not
    want to specify it.

      1. background-color
      2. background-image
      3. background-repeat
      4. background-attachment
      5. background-position

      - ### i.g

      ```css
      body {
          background: #ffffff url("images/tulip.gif")
          no-repeat top right;
        }
      ```

  - ## Image Rollovers & Sprintes

    Using CSS, it is possible to create
    a link or button that changes to a
    second style when a user moves
    their mouse over it (known as a
    rollover) and a third style when
    they click on it.

    This is achieved by setting a
    background image for the link or
    button that has three different
    styles of the same button (but
    only allows enough space to
    show one of them at a time).
    You can see the image we are
    using in this example on the
    right. It actually features two
    buttons on the one image.

    When the user moves their
    mouse over the element, or
    clicks on it, the position of the
    background image is moved to
    show the relevant image.

    When a single image is used
    for several different parts of an
    interface, it is known as a sprite.
    You can add the logo and other
    interface elements, as well as
    buttons to the image.

    The advantage of using sprites is
    that the web browser only needs
    to request one image rather than
    many images, which can make
    the web page load faster.

  - ### CSS3 Gradients

    - `background-image`

      CSS3 is going to introduce the
    ability to specify a gradient for
    the background of a box. The
    gradient is created using the
    background-image property
    and, at the time of writing,
    different browsers required a
    different syntax.

    Since it is not supported by all
    browsers, it is possible to specify
    a background image for the box
    first (which would represent the
    gradient) and then provide the
    CSS alternatives for browsers
    that support gradients.

  - ## Contrast of background images

    If you want to overlay text on a background image, the image must be low
    contrast in order for the text to be legible.

    1. ### High Contrast

       The majority of photographs have quite a high contrast, which
       means that they are not ideal for use as a background image.

    2. ### Low Contrast

       Image editing applications such as Photoshop and GIMP have
       tools that allow you to manually adjust your images to have lower
       contrast.

    3. ### Screen

       To overlay text on an image with high contrast, you can place a
       semi-transparent background color (or "screen") behind the
       text to improve legibility.

## Practical Information

  - ### Search Engine Optimization (SEO)

    **SEO** is a huge topic and several books have been written on the subject.
    The following pages will help you understand the key concepts so you can
    improve your website's visibility on search engines.

    - #### The Basics

      Search engine optimization (or
    SEO) is the practice of trying
    to help your site appear nearer
    the top of search engine results
    when people look for the topics
    that your website covers.

      At the heart of SEO is the idea of
    working out which terms people
    are likely to enter into a search
    engine to find your site and then
    using these terms in the right
    places on your site to increase
    the chances that search engines
    will show a link to your site in
    their results.

    - #### On-Page Techniques

      On-page techniques are the
    methods you can use on your
    web pages to improve their
    rating in search engines.

      The main component of this is
    looking at keywords that people
    are likely to enter into a search
    engine if they wanted to find
    your site, and then including
    these in the text and HTML code
    for your site in order to help the
    search engines know that your.

    - #### Off-Page Techniques

      Getting other sites to link to you
    is just as important as on-page
    techniques. Search engines help
    determine how to rank your
    site by looking at the number of
    other sites that link to yours.

      They are particularly interested
    in sites whose content is related
    to yours. For example, if you
    were running a website that
    sold fish bait, then a link from
    a hairdresser is not likely to be
    considered as relevant as one
    from an angling community.

  - ### How to Identify Keywords and Phrases

    Determining which keywords to use on your site can be one of the
hardest tasks when you start to think about SEO. Here are six steps that
will help you identify the right keywords and phrases for your site.


  1. #### Brainstorm

     List down the words that
    someone might type into
    Google to find your site. Be sure
    to include the various topics,
    products or services your site is
    about.

  2. #### Organize

      Group the keywords into
    separate lists for the different
    sections or categories of your
    website.
    For example, if your website
    was a pet shop you might have
    different categories for different
    animals (such as dogs, cats and
    rabbits).

  3. #### Research

      There are several tools that let
    you enter your keywords and
    then they will suggest additional
    keywords you might like to
    consider, such as:
    adwords.google.co.uk/
    select/KeywordToolExternal
    (When using this tool, select the
    "exact match" option rather than
    "broad match.")

  4. #### Compare

      It is very unlikely that your
    site will appear at the top of
    the search results for every
    keyword. This is especially true
    for topics where there is a lot
    of competition. The more sites
    out there that have already been
    optimized for a given keyword,
    the harder it will be for you to
    rise up the search results when
    people search on that term.

  5. #### Refine

      Now you need to pick which
    keywords you will focus on.
    These should always be the ones
    that are most relevant to each
    section of your site.

      If there is a phrase that is very
    relevant but you find there is a
    lot of competition, you should
    still use it. To improve the
    chances of your site being found
    you can look at whether there
    are other words that could be
    incorporated into a phrase. For
    example, if the information or
    service you offer on your website
    is location specific, then you will
    often find that incorporating
    your location into your keyword
    list will help people find you.

  6. #### Map

      Now that you have a refined list
    of keywords, you know which
    have the most competition, and
    which ones are most relevant,
    it is time to start picking which
    keywords you will use for each
    page.

      Pick 3-5 keywords or phrases
    that map to each page of your
    website and use these as the
    keywords for each page.

