# HTML Tables & JS Functions, Methods, and Objects

## Tables

  - ### What's a Table?

    A table represents information in a grid format.
    Examples of tables include financial reports, TV
    schedules, and sports results.

    - `<table>`

      The `<table>` element is used
      to create a table. The contents
      of the table are written out row
      by row.

    - `<tr>`

      You indicate the start of each
      row using the opening `<tr>` tag.
      (The `tr` stands for table row.)

      It is followed by one or more
      `<td>` elements (one for each cell
      in that row).
      At the end of the row you use a
      closing `</tr>` tag.

    - `<td>`

      Each cell of a table is
      represented using a `<td>`
      element. (The td stands for
      table data.)
      At the end of each cell you use a
      closing `</td>` tag.

  - ### How To Creat Table Headings

    The `<th>` element is used just
    like the `<td>` element but its
    purpose is to represent the
    heading for either a column or
    a row. (The th stands for table
    heading.)

  - ### What Is Spanning Columns?

    Sometimes you may need the
    entries in a table to stretch
    across more than one column.
    The colspan attribute can be
    used on a `<th>` or `<td>` element
    and indicates how many columns
    that cell should run across.

  - ### What Is Spanning Rows?

    You may also need entries in
    a table to stretch down across
    more than one row.
    The rowspan attribute can be
    used on a `<th`> or `<td>` element
    to indicate how many rows a cell
    should span down the table.

  - ### What Is Long Tables?

    There are three elements that
    help distinguish between the
    main content of the table and
    the first and last rows (which can
    contain different content).
    These elements help people
    who use screen readers and also
    allow you to style these sections
    in a different manner than the
    rest of the table (as you will see
    when you learn about CSS).

    - `<thead>`

      The headings of the table should
      sit inside the `<thead>` element.

    - `<tbody>`

      The body should sit inside the
      `<tbody>` element.

    - `<tfoot>`

      The footer belongs inside the
      `<tfoot>` element.

## JS Functions, Methods, and Objects

  - ### Creating an object: Constracter Notation.

    The `new` Keyword and the object **constructor** create a blank object.
    We can then add prperties and methods to the object.

    - ### i.g
    ```js
    var hotel = new Object();

    hotel.name = 'Green Garden';
    hotel.rooms = 45;
    hotel.blooked = 30;

    hotel.checkAvailability = function(){
        return this.rooms -this booked;
    };
    ```

   - ### Updating an object

     To update the value of properties, use dot notation or square brackets. They work on objects created using literal or constructor notation.
     To **delete** a property, use the `delete` **Keyword**.

     - ### i.g

       `hotel.name = 'Park', delete hotel.name`

  - ### Creating many objects: Constructor notation

    Sometime you will want several objects to represent similar thing. Object constructor can use a function as **template** for creating objects. First, Create the template with the object's properties and methods.

    - ### i.g

    ```js
    function Hotel(name, rooms, booked){
        this.name = name;
        this.rooms = rooms;
        this.booked = booked;

        this.checkAvailability = function(){
            return this.rooms - this.booked;
        };
    }


    var parkHotel = new Hotel('Park', 45, 30);
    ```

  - ### ADDING AND REMOVING PROPERTIES TO THE OBJECT

    Once you have created an object
    (using literal or **constructor**
    notation), you can add new
    properties to it.

    You do this using the dot
    notation.In this example, you can see that
    an instance of the hotel object
    is created using an object literal.

    Immediately after this, the
    hotel object is given two
    extra properties that show the
    facilities (whether or not it has
    a **gym** and/or a **pool**). These
    properties are given values that
    are **Booleans**.

    Having added these properties
    to the object, you can access
    them just like any of the objects
    other properties. Here, they
    update the value of the cl ass
    attribute on their respective
    elements to show either a check
    mark or a cross mark.
    To delete a property, you use
    the keyword delete, and then
    use dot notation to identify the
    property or method you want to
    remove from the object.
    In this case, the booked property
    is removed from the object.

  - ### `this` Keyword

    The keyword this is commonly used inside functions and objects.
    Where the function is declared alters what this means. It always refers
    to one object, usually the object in which the function operates.

    - ### A FUNCTION IN GLOBAL SCOPE

      When a function is created at the top level of a script
      (that is, not inside another object or function), then it
      is in the **global scope** or **global context**.
      The default object in this context is the **window
      object**. so when this is used inside a function in the
      global context it refers to the **window object**.

    - ### GLOBAL VARIABLES

      All global variables also become properties of the
      window object. so when a function is in the global
      context, you can access global variables using the
      window object, as well as its other properties.

    - ### A METHOD OF AN OBJECT

      When a function is defined inside an object, it
      becomes a method. In a method, this refers to the
      containing object.

    - ### FUNCTION EXPRESSION AS METHOD

      If a named function has been defined in global
      scope, and it is then used as a method of an object,
      this refers to the object it is contained within.