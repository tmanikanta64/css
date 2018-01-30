# A CLOSER LOOK AT CSS
### A Background Image
In CSS, the background-image property sets a background image of your choice for a given selector, as seen below.

``` .hero {
  background-image: url("https://s3.amazonaws.com/codecademy-content/projects/make-a-website/lesson-2/bg.jpg");
} ```
The CSS rule above assigns the image hosted at

https://s3.amazonaws.com/codecademy-content/projects/make-a-website/lesson-2/bg.jpg
to elements that have a class attribute set to hero.

To control the size of the chosen background image, use the property background-size as seen below:

``` .hero {
  background-image: url("https://s3.amazonaws.com/codecademy-content/projects/make-a-website/lesson-2/bg.jpg");
  background-size: cover;
} ```
Here, we have specified that we want the image to completely cover elements with the .hero class.


# Display: Flex
### In the web browser, the gallery images that were arranged neatly in rows are now stacked on the left side of the webpage.

The CSS display value that arranged the images, flex, has been removed. In addition to other capabilities, flex can be used to easily align multiple page elements horizontally.

In the example code below, there is a div with class parent:

<div class="parent">
   ...
</div>
To make children of the div align horizontally on the webpage, in CSS we can use:

.parent {
  display: flex;
}
Children elements of the div with class parent will now align horizontally. We can make sure no child element moves off the page by using flex-wrap: wrap;:

.parent {
  display: flex;
  flex-wrap: wrap;
}
Finally, to center rows of children elements, we can use justify-content: center;:

.parent {
  display: flex; 
  flex-wrap: wrap; 
  justify-content: center;
}
