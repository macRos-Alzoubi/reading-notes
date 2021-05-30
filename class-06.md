# JS Object

## Object Literals

  - ## WHAT IS AN OBJECT?

    Objects group together a set of variables and functions to create a model of a something you would recognize from the real world. In an object, variables and functions take on new names.

    - ### PROPERTIES

      IN AN OBJECT: VARIABLES BECOME KNOWN AS **PROPERTIES**
      
       If a variable is part of an object, it is called a **property**. Properties te ll us about the object, such as the name of a hotel or the number of rooms it has. Each individual hotel might have a different name and a different number of rooms.

    - ### METHODS 

      IN AN OBJECT: FUNCTIONS BECOME KNOWN AS **METHODS**

      If a function is part of an object, it is called a **method**. Methods represent tasks that are associated with the object. For example, you can check how many rooms are available by subtracting the number of booked rooms from t he total number of rooms.

  - ## How To Create An Object

    Literal notation is the easiest and most popular way to create objects.

    The object is the curly braces and their contents.The object is stored in a variable called hotel, so you would refer to it as hotel objet.

    Separate each key from its value using colon, Seperate each property and method with a comma.

  - ## How To Access An Object

    We can access the properties or methods of an object using dot notation.
    We can also access properties using square brakets.

## Document Object Model (DOM)

The **Document Object Model (DOM)** specifies
how browsers should create a model of an HTML
page and how JavaScript can access and update the
contents of a web page while it is in the browser window.

- ### MAKING A MODEL OF THE HTML PAGE

  When the browser loads a web page, it
  creates a model of the page in memory.

  The **DOM** specifies the way in which the
  browser should structure this model using
  a DOM tree.

  The **DOM** is called an object **model**
  because the model (the DOM tree) is
  made of objects.

  Each object represents a different part of
  the page loaded in the browser window.

- ### ACCESSING AND CHANGING THE HTML PAGE

  The DOM also defines methods and
  properties to access and update each
  object in this model, which in turn updates
  what the user sees in the browser.

  **Application Programming Interface (API)**.

  User interfaces let humans interact with
  programs; **APls** let programs (and scripts)
  talk to each other. The DOM states what
  your script can "ask the browser about the
  current page, and how to tell the browser
  to update what is being shown to the user.

  - ## THE DOCUMENT NODE

    Every element, attribute, and piece of text in the
    HTML is represented by its own DOM node.
    At the top of the tree a document node is added; it
    represents the entire page.

    When you access any element, attribute, or text
    node, you navigate to it via the document node. It is
    the starting point for all visits to the DOM tree.

  - ## ELEMENT NODES

    HTML elements describe the structure of an HTML
    page. (The `<h l > - <h6>` elements describe what
    parts are headings; the `<p>` tags indicate where
    paragraphs of text start and finish; and so on.)
    To access the DOM tree, you start by looking for
    elements. Once you find the element you want, then
    you can access its text and attribute nodes if you
    want to. This is why you start by learning methods
    that allow you to access element nodes, before
    learning to access and alter text or attributes.

  - ## ATTRIBUTE NODES

    The opening tags of HTML elements can carry
    attributes and these are represented by attribute
    nodes in the **DOM** tree.

    Attribute nodes are not children of the element thar
    carries them; they are part of that element. Once
    you access an element, there are specific JavaScript
    methods and properties to read or change that
    element's attributes. For example, it is common to
    change the values of cl ass attributes to trigger new
    CSS rules that affect their presentation.

  - ## TEXT NODES

    Once you have accessed an element node, you
    can then reach the text within that element. This is
    stored in its own text node.

    Text nodes cannot have children. If an element
    contains text and another child element, the child
    element is not a child of the text node but rather
    a child of the containing element. (See the `<em>`
    element on the first `<l i >` item.) This illustrates how
    the text node is always a new branch of the DOM
    tree, and no further branches come off of it.

  - ## HOW TO WORK WITH THE DOM TREE

    Accessing and updating the DOM tree involves two steps:
    1. Locate the node that represents the element you want to work with.
    2. Use its text content, child elements, and attributes.

    - ### STEP 1: ACCESS THE ELEMENTS

      Here are three common ways to select an individual element:

        - `get El ement Byld ()`

          Uses the value of an element's id attribute (which should be
          unique within the page).

        - `querySelector()`

          Uses a CSS selector, and returns the first matching element.

        - `getElementsByClassName()`

          Selects all elements that have a specific value for their class attribute.

        - `getElementsByTagName()`

          Selects all elements that have the specified tag name.

        - `querySelectorAll()`

          Uses a CSS selector to select all matching elements.

        - `parentNode`

          Selects the parent of the current element node (which will return just one element).

        - `previousSibling / nextSibling`

          Selects the previous or next sibling from the DOM tree.

        - `firstChild / lastChild`

          Select the first or last child of the current element.

    - ### STEP 2: WORK WITH THOSE ELEMENTS

      Here is an overview of methods and properties that work with the elements:
      
      - ### ACCESS/ UPDATE TEXT NODES

        The text inside any element is
        stored inside a text node. To
        access the text node above:
        1. Select the `<l i >`element
        2. Use the fi rstChi l d property
        to get the text node
        3. Use the text node's only
        property (nodeValue) to get
        the text from the element

        `nodeValue`

          This property lets you access or update contents of a text node.

    - ### WORK WITH HTML CONTENT

      One property allows access to
      child elements and text content:
      `innerHTML`

      Another just the text content:
      `textContent`

      Several methods let you create
      new nodes, add nodes to a tree,
      and remove nodes from a tree:
      `create Element()`,
      `createTextNode()`,
       And `appendChi l d () / removeChi l d ()`
      This is called DOM manipulation.

    - ### ACCESS OR UPDATE ATTRIBUTE VALUES

      Here are some of the properties
      and methods you can use to
      work with attributes:
      `className /id`
      Lets you get or update the value
      of the class and id attributes.

      `hasAttribute()`, 
      `getAttribute()`, 
      `setAttribute()`, 
      `removeAttribute()`, 
      The first checks if an attribute
      exists. The second gets its value.
      The third updates the value.
      The fourth removes an attribute.

