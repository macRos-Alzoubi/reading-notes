# Wireframe: 
is a practice used by UX designers which allows them to define and plan the information hierarchy of their design for a website, app, or product.

- I.g of wireframe design software 
  - Invision
  -  Balsamiq

- There are a number of ways different designers can  structure the process from design to implementation:
  - Wireframe > Interactive Prototype > Visual > Design
  - Sketch > Code
  - Sketch > Wireframe > Hi-Def Wireframe > Visual > Code
  - Sketch > Wireframe > Visual > Code

- The best tools for wireframing:
  - UXPin: UXPin has a wide range of functionalities.
  - InVision: InVision allows you to get feedback straight from your team and users through.
  - Wireframe.cc: Wireframe.cc provides you with the          technology to create wireframes really quickly within your browser.

# HTML:
HTML is a markup language that defines the structure of your content. HTML consists of a series of elements, which you use to enclose, or wrap, different parts of the content to make it appear a certain way, or act a certain way. The enclosing tags can make a word or image hyperlink to somewhere else, can italicize words, can make the font bigger or smaller, and so on. 
- i.g: ``` <p>My cat is very grumpy</p> ```


- Anatomy of an HTML element:
  1. **The opening tag**: This consists of the name of the element, wrapped in opening and closing ***angle brackets***. This states where the element begins or starts to take effect.
  2. **The closing tag**: This is the same as the opening tag, except that it includes a forward slash before the element name. This states where the element ends.Failing to add a closing tag is one of the standard beginner errors and can lead to strange results.
  3. **The content**: This is the content of the element.
  4. **The element**: The opening tag, the closing tag, and the content together comprise the element. ```<element> content </element> ```
   - **Elements can also have attributes** :
   Attributes contain extra information about the element that you don't want to appear in the actual content.
   ```<element attribute="some-value"> content </element> ```

- **Nesting elements**:
  You can put elements inside other elements too — this is called nesting.
   - i.g: ```<p>My cat is <span>very</span> grumpy.</p> ```

- **Empty elements**: Some elements have no content and are called      empty elements. Take the ```<img>``` element for example
  - i.g: ``` <img src="images/firefox-icon.png" alt="My test image"> ```

- **Anatomy of an HTML document**:
  ```
  <!DOCTYPE html>
  <html>
    <head>
      <meta charset="utf-8">
      <title>My test page</title>
    </head>
    <body>
      <img src="images/firefox-icon.png" alt="My test image">
    </body>
  </html>
  ```
  - ```<DOCTYPE html> ```: It tells the browser that we are using HTML5.
  - ```<html> </html> ```: the ```<html>``` element. This element wraps all the content on the entire page and is sometimes known as the root element.
  - ``` <head></head> ```:  the ```<head>``` element. This element acts as a container for all the stuff you want to include on the HTML page that isn't the content you are showing to your page's viewers. This includes things like **keywords** and a page description that you want to appear in search results, **CSS** to style our content, character set declarations, and more.
  - ``` <meta charset="utf-8"> ```: This element sets the character set your document should use to UTF-8 which includes most characters from the vast majority of written languages. Essentially, it can now handle any textual content you might put on it. There is no reason not to set this and it can help avoid some problems later on.
  - ``` <title></title> ```: the ```<title>``` element. This sets the title of your page, which is the title that appears in the browser tab the page is loaded in. It is also used to describe the page when you bookmark/favorite it.
  - ``` <body></body> ```:  the ````<body>``` element. This contains all the content that you want to show to web users when they visit your page, whether that's text, images, videos, games, playable audio tracks, or whatever else.
  
# Semantics:
Semantics refers to the meaning of a piece of code — for example "what effect does running that line of JavaScript have?", or "what purpose or role does that HTML element have" (rather than "what does it look like?".) 

- **Semantics in JavaScript**:
In JavaScript, consider a function that takes a string parameter, and returns an ```<li>``` element with that string as its textContent. Would you need to look at the code to understand what the function did if it was called build('Peach'), or createLiWithContent('Peach')?
- **Semantics in CSS**:
In CSS, consider styling a list with li elements representing different types of fruits. Would you know what part of the DOM is being selected with ```div > ul > li, or .fruits__item?```
- **Semantics in HTML**:
  In HTML, for example, the ```<h1>``` element is a semantic element, which gives the text it wraps around the role (or meaning) of "a top level heading on your page."
