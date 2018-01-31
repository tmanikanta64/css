# BUILDING WITH BOOTSTRAP
### Connecting to Bootstrap
Before Bootstrap can work for us, we need to link to it.

In earlier lessons, we linked only to main.css. Now, in addition to main.css, we will link to a URL that hosts Bootstrap.

The HTML link element makes Bootstrap available to us. Remember that the link element is typically contained within HTML head tags.

<head>
  ... 
  <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.6/css/bootstrap.min.css"/>
  ...
</head>
Above, the href attribute is set to the URL https://maxcdn.bootstrapcdn.com/bootstrap/3.3.6/css/bootstrap.min.css.

Let's explore what Bootstrap can do for us.

# On the Grid
### One of the reasons Bootstrap and frameworks like it are so popular is because they offer grids. A grid makes it possible to organize HTML elements using preconfigured columns. Using a grid, you can customize responsive page layouts quickly and reliably.

The Bootstrap grid contains 12 equal-sized columns, as seen in the diagram on the right. HTML elements are arranged to span different numbers of columns in order to create custom page layouts.

In the diagram, observe the following:

Bootstrap's grid columns are represented by 12 vertical bars. The boxes represent HTML elements.


The words "container", "jumbotron", "col-sm-6" and "col-sm-3" refer to Bootstrap classes. 


The element with class "jumbotron" spans the entire width of the webpage, beyond the borders of the grid. 


Elements inside the second "container", such as "col-sm-6" and "col-sm-3" are contained within the grid columns. 


Elements labeled "col-sm-3" take up three grid columns; elements labeled "col-sm-6" take up six grid columns.




# Header/Navigation
Let's use Bootstrap's grid to create a simple header with navbar.

In the example code below, an HTML header element with Bootstrap's predefined container class is used:

<header class="container">
  ...
</header>
Inside the header, a row is created by using a div with Bootstrap's row class:

<header class="container">
  <div class="row">
  </div> 
</header>
Finally, the row is cut into two parts:

<header class="container">
  <div class="row">
   <h1 class="col-sm-4">Heading</h1>
   <nav class="col-sm-8 text-right">
    <p>nav item 1</p>
    <p>nav item 2</p>
    <p>nav item 3</p>
   </nav> 
 </div>
</header>
The first part consists of the h1 with Bootstrap's class col-sm-4. It will take up the first four columns on the grid. The second part consists of the nav element with class col-sm-8. It will take up the remaining eight grid columns. text-right indicates that text will be arranged on the right side of the nav.

1.
In index.html, on the line below the opening <body> tag, create a header element with Bootstrap's container class:

<header class="container">
  ...
</header>
Click Run to continue.

2.
Next, inside the opening <header class="container"> tag, create a div with the Bootstrap class row:

<header class="container">
  <div class="row">
  </div>
</header>
Click Run to continue.

3.
Now we'll cut the row into two parts.

The first part: inside the <div class="row"> tag, create an h1 with Bootstrap's class col-sm-4. The content for the h1 will be the company name. You can use "Skillfair" or anything you'd like:

<header class="container">
  <div class="row">
    <h1 class="col-sm-4">Skillfair</h1>
  </div>
</header>
Click Run to see the results in the web browser.

4.
Now for the second part of the row. One line below the h1 element, create a nav element with Bootstrap's class col-sm-8 text-right:

<header class="container">
  <div class="row">
    <h1 class="col-sm-4">Skillfair</h1>
    <nav class="col-sm-8 text-right">
    </nav>
 </div>
</header>
Click Run to continue.

5.
Finally, inside the opening <nav class="col-sm-8">, create three p elements. The content for each p will be a navigation item. You could use item names such as "newest", "catalogue" and "contact":

<header class="container">
  <div class="row">
    <h1 class="col-sm-4">Skillfair</h1>
    <nav class="col-sm-8 text-right">
      <p>newest</p>
      <p>catalogue</p>
      <p>contact</p>
    </nav>
 </div>
</header>
Click Run to see the compeleted header/navigation in the web browser.


# The Jumbotron
In addition to a header/navigation, many websites have a large showcase area featuring important content. Bootstrap refers to this as a jumbotron. Below is an example implementation of a jumbotron.

First, a new section element is created and assigned the jumbotron class:

<section class="jumbotron">

</section>
Next a div with the Bootstrap class container is used:

<section class="jumbotron">
  <div class="container">
  ... 
  </div>
</section>
A div with the Bootstrap class row text-center can center subsequent child elements which will contain text:

<section class="jumbotron">
  <div class="container">
    <div class="row text-center">
       ...
    </div>
  </div>
</section>
The ... is a placeholder for HTML elements containing text, such as h2, p or anchor elements.

Let's explore the jumbotron feature by creating our own below!

1.
In index.html, one line below the closing </header> tag, Create a section with the jumbotron class.

<section class="jumbotron">

</section>
Click Run. In the web browser, notice a large photo covering the main part of the webpage.

2.
Inside the opening <section class="jumbotron"> tag, create a div with the container class:

<section class="jumbotron">
  <div class="container">
  </div>
</section>
Don't forget your </div> closing tag!

Click Run to continue. There won't yet be a visual change in the web browser.

3.
To center text over the jumbotron image, create another div inside the container div. Give the new div a class of row text-center:

<section class="jumbotron">
  <div class="container">
    <div class="row text-center">
    ...
    </div>
  </div>
</section>
The ... is a placeholder for where text elements will go next.

Click Run to continue. There still will not be a visual effect on the web browser.

4.
Finally, add heading and anchor elements to the row.

The anchor element will have Bootstrap's btn btn-primary class, which will transform it into a button.

<section class="jumbotron">
  <div class="container">
    <div class="row text-center">
      <h2>Homemade Goods</h2>
      <h3>This Year's Best</h3>
      <a class="btn btn-primary" href="#" role="button">See all</a>
    </div>
  </div>
</section>
Click Run to see the elements centered over the jumbotron image in the web browser.

If you'd like, replace text between h2 , h3 and a tags with text of your choice.

Note: The anchor element's href attribute, #, is a placeholder for an actual URL.
