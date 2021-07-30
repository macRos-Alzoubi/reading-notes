# Node.js

## An Introduction to Node.js

### - What is node.js?

Node.js is an event-based, non-blocking, asynchronous I/O runtime that uses Google’s V8 JavaScript engine and libuv library.

### - In your own words, what is Chrome’s V8 JavaScript Engine?

It's open-source JavaScript engine that runs in Google Chrome and other Chromium-based web browsers.

And it is responsible for compiling JavaScript directly to native machine code that your computer can execute.

### - What does it mean that node is a JavaScript runtime?

This means that Node.js is a program we can use to execute JavaScript on our computers.

### - What is npm?

a package manager that comes bundled with Node.

### - What version of node are you running on your machine?

V14.17.0

### - What version of npm are you running on your machine?

7.20.3

### - What command would you type to install a library/package called ‘jshint’?

npm install jshint

### - What is node used for?

It can be used for programing many thing.

I.g:

- ## Chat applications

    Node.js is commonly used to develop real-time applications, also known as RTAs. Its asynchronous, event-driven nature, allows it to handle heavy input-output operations, which makes it much easier for Node.js developers to achieve the level of performance users have come to expect from modern real-time applications.

    When building chat applications with Node.js, it’s common to take advantage of the `Socket.IO library`, which enables real-time, bidirectional, and event-based communication between the browser and the server. With `Socket.IO`, it’s possible to build a group-chat application in less than 30 lines of code.

- ## Streaming applications

    Being one of the largest media-services providers in the world is not easy, especially when your job is to offer streaming content over 150 million users around the world, which is why Netflix moved half of its API to Node.js in 2018.

    Thanks to Node.js, **Netflix** finally has a common language for both **server-side and browser side**, and it benefits from the asynchronous non-blocking I/O capabilities that make real-time and streaming operations with Node.js so easy and efficient.

- ## Command-line applications

    In the world of JavaScript development, command-line applications don’t get much attention. However, the reality is that most larger organizations use at least some custom-made command-line tools.

    Thanks to libraries such as commander, yargs, and oclif, creating command-line applications with Node.js is simple, fast, and extremely cost-effective. As such, `Node.js` empowers developers who are not familiar with traditional backend languages to use `JavaScript` outside the web and develop various work automation solutions.

- ## Browser games

    Node.js can also be used for game development in combination with technologies such as `HTML5` and `Socket.IO` to create single and multiplayer games that work directly in the browser without the need to install any third-party plugins.

    Node.js provides game developers with several tools that make it easier to manage the complexity of multiplayer games, including EventEmitter, which can be used to raise and handle custom events.

    What’s more, Node.js allows developers to share a lot of code between the client and the server.

- ## Embedded systems

    The idea of using JavaScript to program microcontrollers and prototype internet of things devices may sound strange, but hardware programming is quickly emerging as a major use case of Node.js. There is now even a port of Node.js with far lower system requirements, called `low.js`, which allows Node.js to run on cheap, power-efficient microcontroller boards based on the ESP32-WROVER module.

    And with robust IoT and robotics development platforms like Tessel 2, leveraging all the libraries of Node.js to create useful devices in minutes has never been easier.

## Pair Programming

### - What are the 6 reasons for pair programming?

1. Greater efficiency
2. Engaged collaboration
3. Learning from fellow students
4. Social skills
5. Job interview readiness
6. Work environment readiness

### - n your experience, which of these reasons have you found most beneficial?

- #### Engaged collaboration

### - How does pair programming work?

pair programming commonly involves two roles: the Driver and the Navigator. The Driver is the programmer who is typing and the only one whose hands are on the keyboard. Handling the “mechanics” of coding, the Driver manages the text editor, switching files, version control, and—of course writing—code. The Navigator uses their words to guide the Driver but does not provide any direct input to the computer. The Navigator thinks about the big picture, what comes next, how an algorithm might be converted in to code, while scanning for typos or bugs. The Navigator might also utilize their computer as a second screen to look up solutions and documentation, but should not be writing any code.