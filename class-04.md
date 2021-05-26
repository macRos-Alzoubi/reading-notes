# HTML Links, JS Functions, and Intro to CSS Layout

- ## Links

    Links are the defining feature of the web
    because they allow you to move from
    one web page to another — enabling the
    very idea of browsing or surfing.

    Links are created using the `<a>` element. Users can click on anything
    between the opening `<a>` tag and the closing `</a>` tag. You specify
    which page you want to link to using the `href` attribute.

    When you link to a different website, the value of the href
    attribute will be the full web address for the site, which is
    known as an absolute URL.

    When you are linking to **other pages** within the same **site**, you do not need to specify the domain name in the URL. You
    can use a shorthand known as a **relative URL**.

    If all the pages of the site are in the same folder, then the value
    of the href attribute is just the name of the file.

    - ### Email Links

        To create a link that starts up
        the user's email program and
        addresses an email to a specified
        email address, you use the `<a>`
        element. However, this time the
        value of the `href` attribute starts
        with `mailto:` and is followed by
        the **email address** you want the
        email to be sent to.

    - ### Opening Links In New Window

      If you want a link to open in a
      new window, you can use the
      target attribute on the opening
      `<a>` tag. The value of this
      attribute should be `_blank`.

    - ### Linking to a Specific Part of the Same Page

      you need to identify the points in the page
      that the link will go to. You do this using the `id` attribute (which
      can be used on every HTML element). You can see that the
      `<h1>` and `<h2>` elements in this example have been given `id`
      attributes that identify those sections of the page.

      The value of the `id` attribute should start with a **letter** or an **underscore (not a number or any other character)** and, on a
      single page, no two `id` attributes should have the same value.

      To link to an element that uses an id attribute you use the `<a>`
      element again, but the value of the `href` attribute starts with
      the `#` symbol, followed by the value of the `id` attribute of the
      element you want to link to. In this example, `<a href="#top">`
      links to the `<h1>` element at the top of the page whose id
      attribute has a value of top.

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

- ## JS Functions, Methods, and Objects

  - ### FUNCTIONS & METHODS

    **Functions** consist of a series of statements that have been grouped together because they perform a specific task.
    A **method** is the same as a function, except methods are created inside **(and are part of) an object**.

    - **Structure**: 
      ```JS
      // function declaration
      function functioName(Parameter/s){
          // Code
      }

      // function expression
      let/ const functionName = function(Parameter/s){
          // Code
      };
      ```

  - ### OBJECTS

    objects are made up of **properties** and **methods**.

  - ### Function Call

    You can call a function by just type its name and pass any possible parameter/s inside of its parenthesis.

    - **i.g**: `functionName(parameter/s);`

  - ### FUNCTION DECLARATION

    A **function declaration** creates a function that you
    can ca ll later in your code.

    In order to call the function later in your code, you
    must give it a name, so these are known as **named
    functions**. Below, a function called area() is
    declared, which can then be called using its name.

  - ### FUNCTION EXPRESSION

    If you put a function where the interpreter would
    expect to see an **expression**, then it is treated as an
    expression, and it is known as a **function expression**.
    In function expressions, the name is usually omitted.

  - ### VARIABLE SCOPE

    - #### LOCAL VARIABLES

      When a variable is created inside a function using the
      var keyword, it can only be used in that function.
      It is called a **local** variable or **function-level** variable.
      It is said to have **local scope** or function-level scope.
      It cannot be accessed outside of the function in
      which it was declared. Below, area is a **local variable**.

    - #### GLOBAL VARIABLES

      If you create a variable outside of a function, then it
      can be used anywhere within the script. It is called a
      **global variable** and has **global scope**. In the example
      shown, wa 11 Size is a global variable.

- ## 6 Reasons for Pair Programming

  Iterative loops. Code reviews. Fast feedback. Error checking and linting. These are software engineering practices that have proven to dramatically improve the quality of code developers produce. What if you can could get all of this, instantaneously, while typing code line by line and character by character? You can, with pair programming, a technique common to many agile work environments.

  - ###  How does pair programming work?

    pair programming commonly involves two roles: the Driver and the Navigator. The Driver is the programmer who is typing and the only one whose hands are on the keyboard. Handling the “mechanics” of coding, the Driver manages the text editor, switching files, version control, and—of course writing—code. The Navigator uses their words to guide the Driver but does not provide any direct input to the computer. The Navigator thinks about the big picture, what comes next, how an algorithm might be converted in to code, while scanning for typos or bugs. The Navigator might also utilize their computer as a second screen to look up solutions and documentation, but should not be writing any code.

  - ### Why pair program?

    While learning to code, developers likely study several programming languages. Similar to a foreign language class, there are four fundamental skills that help anyone learn a new language: Listening: hearing and interpreting the vocabulary Speaking: using the correct words to communicate an idea Reading: understanding what written language intends to convey Writing: producing from scratch a meaningful

    Pair programming touches on all four skills: developers explain out loud what the code should do, listen to others’ guidance, read code that others have written, and write code themselves.

    1. Greater efficiency
    It is a common misconception that pair programming takes a lot longer and is less efficient. In reality, when two people focus on the same code base, it is easier to catch mistakes in the making. Research indicates that pair programing takes slightly longer, but produces higher-quality code that doesn’t require later effort in troubleshooting and debugging (let alone exposing users to a broken product). So, in the long-run, it’s often actually more efficient than two people working on separate features. When coming up with ideas and discussing solutions out loud, two programmers may come to a solution faster than one programmer on their own. Also, when the pair is stuck, both programmers can research the problem and reach a solution faster. Researches also identified pairing enhances technical skills, team communication, and even enjoyability of coding in the workplace.

    2. Engaged collaboration
        When two programmers focus on the same code, the experience is more engaging and both programmers are more focused than if they were working alone. It is harder to procrastinate or get off track when someone else is relying on you to complete the work. Popping open your Facebook timeline is just that less enticing when someone else is looking at your screen.

        Another important aspect of learning to program is knowing when to ask for help. We advise our students to spend no more than fifteen minutes stuck on a problem before asking a teaching assistant or instructor for help. When developers pair program, they rely more on each other and can often find a solution together without needing to ask for additional help. Ultimately, this boosts overall confidence.

    3. Learning from fellow students
        Everyone has a different approach to problem solving; working with a teammate can expose developers to techniques they otherwise would not have thought of. If one developer has a unique approach to a specific problem, pair programming exposes the other developer to a new solution.

        Often times, the developers in a pairing have different skill sets. If one programmer is more experienced in a certain skill, they can teach a student who is less familiar with that area. The less experienced developer benefits from the experienced developer’s knowledge and guidance, and the latter benefits from explaining the topic in their own words, further solidifying their own understanding.

    4. Social skills
        Pair programming is great for improving social skills. When working with someone who has a different coding style, communication is key. This can become more difficult when two programmers have different personalities. Pair programming not only improves programming skills, but can also help programmers develop their interpersonal skills. When just grabbing the keyboard and taking over isn’t an option, getting good at finding the right words is a skill unto itself.

        This has long-term career impacts. As much as employers want strong programmers, they know it’s essential to hire people who can work well with others.

    5. Job interview readiness
        A common step in many interview processes involves pair programming between a current employee and an applicant, either in person or through a shared screen. They will carry out exercises together, such as code challenges, building a project or feature, or debugging an existing code base. By doing so, companies can get a better feel for how an applicant will fit into the team and their collaboration style.

        For most roles, the ability to work with and learn from others and stellar communication skills are as (or more!) important to a company than specific technical skills. Pair programming strengthens all of those skills.

    6. Work environment readiness
        Many companies that utilize pair programing expect to train fresh hires from CS-degree programs on how they operate to actually deliver a product. Code Fellows graduates who are already familiar with how pairing works can hit the ground running at a new job, with one less hurdle to overcome.