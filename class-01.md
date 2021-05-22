
## How the Web Works?
  1. When you connect to the web,
  you do so via an Internet Service
  Provider (ISP). You type a
  domain name or web address
  into your browser to visit a site;
  for example: google.com.
  2. Your computer contacts a
  network of servers called
  Domain Name System (DNS)
  servers. These act like phone
  books; they tell your computer
  the IP address associated with
  the requested domain name.
  An IP address is a number
  of up to 12 digits separated
  by periods / full stops. Every
  device connected to the web
  has a unique IP address; it is
  like the phone number for that
  computer.
  3. The unique number that the
  DNS server returns to your
  computer allows your browser
  to contact the web server
  that hosts the website you
  requested. A web server is a
  computer that is constantly
  connected to the web, and is set
  up especially to send web pages
  to users.
  4. The unique number that the
  DNS server returns to your
  computer allows your browser
  to contact the web server
  that hosts the website you
  requested. A web server is a
  computer that is constantly
  connected to the web, and is set
  up especially to send web pages
  to users.

# HTML
  - ## What is HTML?
    - `HTML` stands for Hyper Text Markup Language.
    - `HTML` is the standard markup language for creating Web pages.
    - `HTML` describes the structure of a Web page.
    - `HTML` consists of a series of elements.
    - `HTML` elements tell the browser how to display the content.
    - `HTML` elements label pieces of content such as "this is a heading"`<h>`, "this is a paragraph"`<p>`, "this is a link"`<a>`, etc.
  
  - ## What is an HTML Element?
  An HTML element is defined by a start tag, some content, and an end tag:
  
  `<tagname>Content goes here...</tagname>`
    
    - ### Some Important Tag Elements:
      - The `<html>` element is the root element of an HTML page.
      - The `<head>` element contains meta information about the HTML page.
      - The `<title>` element specifies a title for the HTML page (which is shown in the browser's title bar or in the page's tab)
      - The `<body>` element defines the document's body, and is a container for all the visible contents, such as headings, paragraphs, images, hyperlinks, tables, lists, etc.
      - The `<h1>` element defines a large heading.
      - The `<p>` element defines a paragraph.

  - ## What is HTML Element Attribute?
  HTML attributes provide additional information about HTML elements.
    - All HTML elements can have __attributes__.
    - Attributes provide __additional information__ about elements.
    - Attributes are always specified in __the start tag__.
    - Attributes usually come in __name/value__ pairs like: `name="value"`.
    - i.g: `<img src="cat.jpg">`

  - ## What is HTML DOCTYPE?
  The __HTML DOCTYPE__ is used to specify the HTML document version used in the web browser.
    - The `<!DOCTYPE html>` declaration defines that this document is an HTML5 document.
  
  - ## How to use comments in HTML?
  To use comments in HTML We just type 

  `<!-- Write your comments here -->`
  __NOTE__: It can be very usefull in case of documenting a larg code or when work with ather developer on a project.

  - ## How to select HTML element?
    - ### __ID__ Attribute:
      It is used to
      uniquely identify that element
      from other elements on the
      page.
      It is important that no two
      elements on the same page
      have the same value for their id
      attributes.
    - ### __Class__ Attribute:
      The __HTML class__ attribute is used to specify a class for an HTML element.
      Multiple HTML elements can share the same class.
  
  - ## What is Block element and Inline element?
    - ### __Block Element__:
      - A __block-level__ element always starts on a new line.
      - A __block-level__ element always takes up the full width available (stretches out to the left and right as far as it can).
      - A __block level__ element has a top and a bottom margin, whereas an inline element does not.
      - i.g: `<div>Hello World</div>`
    
    - ### __Inline Element__:
      - An __inline element__ does not start on a new line.
      - An __inline element__ only takes up as much width as necessary.
      - i.g: __span tag__ `<p> some <span>Text</span></p>`
  
  - ## Grouping text & elements in block:
  The `<div>` element allows you to
  group a set of elements together
  in one block-level box.
    - i.g:
    ```
          <div id="header">
          <img src="images/logo.gif" alt="Anish Kapoor" />
          <ul>
          <li><a href="index.html">Home</a></li>
          <li><a href="biography.html">Biography</a></li>
          <li><a href="works.html">Works</a></li>
          <li><a href="contact.html">Contact</a></li>
          </ul>
          </div><!-- end of header --> 
    ```

  - ## Grouping text & elements inline:
  The `<span>` element acts like
  an inline equivalent of the `<div>`
  element. It is used to either:
    1. Contain a section of text
      where there is no other suitable
      element to differentiate it from
      its surrounding text.
    2. Contain a number of inline
      elements.
  
  - ## IFrame:
  An iframe is like a little window
  that has been cut into your
  page — and in that window you
  can see another page. The term
  iframe is an abbreviation of inline
  frame.

  One common use of iframes
  (that you may have seen on
  various websites) is to embed
  a Google Map into a page. The
  content of the iframe can be any
  html page (either located on the
  same server or anywhere else on
  the web).

  - ## `meta` __tags__:
  The `<meta>` tag allows you to supply all kinds of
  information about your web page.

  - ## __Escape characters__:
  Escape characters are used to include special
  characters in your pages such as `<`, `>`, and`©`.

  - ## HTML Layouts:
    - ### Traditional HTML Layouts
      For a long time, web page authors used `<div>` elements to group
      together related elements on the page (such as the elements that form a
      header, an article, footer or sidebar). Authors used class or id attributes
      to indicate the role of the `<div>` element in the structure of the page.
    
    - ### New HTML5 Layout Elements
      HTML5 introduces a new set of elements that allow you to divide up the
      parts of a page. The names of these elements indicate the kind of content
      you will find in them. They are still subject to change, but that has not
      stopped many web page authors using them already.
      - i.g: `<header> <main> <nav> <footer> <aside> `etc.

  - ## Who is the Site For?
  Every website should be designed for the
  target audience—not just for yourself or the
  site owner. It is therefore very important to
  understand who your target audience is.

    - __Target Audience__:
      - i__ndividuals__:
      You should ask yourself as the designer a few questions:
        - What is the age range of your target audience?
        - Will your site appeal to more women or men? What is the mix?
        - Which country do your visitors live in?
        - Do they live in urban or rural areas?
        - What is the average income of visitors?
        - What level of education do they have?
        - What is their marital or family status?
        - and more .....
      
      - __Companies__:
        - What is the size of the company or relevant department?
        - What is the position of people in the company who visit your site?
        - Will visitors be using the site for themselves or for someone else?
        - How large is the budget they control?


  - ## What is a __Site Maps__:
  a diagram of the pages that will be used
  to structure the site.

  - ## Why we use __WireFrames__?
  Wireframes allow you to organize the information that
  will need to go on each page.

  A wireframe is a simple sketch of the key
  information that needs to go on each page of a
  site. It shows the hierarchy of the information
  and how much space it might require.

# Javascript
- ## What is __Javascript__:
   is a scripting language that enables you to create dynamically updating content, control multimedia, animate images, and pretty much everything else. 

   - ### What is a __Script__:
  A script is a series of instructions that a
  computer can follow to achieve a goal.
  
  - ### How to write a script
  To write a script, you need to first
  state your goal and then list the
  tasks that need to be completed in
  order to achieve it.
  1. DEFINE THE GOAL:

    First, you need to define the task you want to
    achieve. You can think of this as a puzzle for the
    computer to solve.

  2. DESIGN THE SCRIPT:

    To design a script you split the goal out into a
    series
    of tasks that are going to be involved in solving this
    puzzle. This can be represented using a flowchart.
  
  3. CODE EACH STEP:

    Each of the steps needs to be written in a
    programming language that the compu ter
    understands. In our case, this is JavaScript.

- ## EXAMPLES OF JAVASCRIPT IN THE BROWSER
  - Forms
  - Slideshows
  - Filtering data
  - Reload part of a page
- ## __OBJECTS & PROPERTIES__:
  - ### __Object__ (things):
   In computer programming, each physica l thing in
   the world can be represented as an __object__. There are
   two different __types__ of objects here: a hotel and a car.
  
  - ### __PROPERTIES__ (CHARACTERISTICS):
   Both of the cars share common characteristics.
   In fact, all cars have a make, a color, and engine
   size. You could even determine their current
   speed. Programmers call these characteristics the
   __properties__ of an object.

  - ### Each object can have its own:
    - Properties
    - Events
    - Methods

- ## __EVENTS__:
  - ### What is Events:
   JavaScript's interaction with HTML is handled through events that occur when the user or the browser manipulates a page.

   Programmers choose which events they respond to.
   When a specific event happens, that event can be
   used to trigger a specific section of the code.

- ## __METHODS__:
  - ### What is METHODS:
   Methods typically represent how people (or other
   things) interact with an object in the real world.
  - ### WHAT DOES A METHOD DO?
   The code for a method can contain lots of
   instructions that together represent one task.

