
##You Bet Your Bootstrap!
It's pretty easy to soup up your site with some Bootstrap. This walkthrough will take you through the necessary steps to integrate Bootstrap to get your site looking slick and professional.

**1. Set Up Your Bare Bones Site**
Start by creating an `index.html` site. Copy the following HTML code into your `index.html` document:
```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1">

    <title>Steph's Teenage Mutant Ninja Turtle Fan Site</title>

  </head>
  <body>

  </body>
</html>
```
**2. Include Bootstrap CSS**
Within the `<head>` tag, under the `<title>` tag, copy this link to the Bootstrap CSS.
```html
<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.1/css/bootstrap.min.css">
```
**3. Include jQuery and Bootstrap JavaScript Libraries**
Include the source code for jQuery and Bootstrap Javascript **right before the closing** `</body>` **tag**. This code gives your site cool animations and added functionalities to make for a better user experience.
```html
<!-- Bootstrap core JavaScript
================================================== -->
<!-- Placed at the end of the document so the pages load faster -->
<script src="https://ajax.googleapis.com/ajax/libs/jquery/1.11.1/jquery.min.js"></script>
<!-- Latest compiled and minified JavaScript -->
<script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.1/js/bootstrap.min.js"></script>
```
**4. Add Internet Explorer support**
There are a lot of different browsers people use nowadays, so sometimes we need to include extra code to make sure our site displays correctly on every browser. Here's what you need to to add to make sure everything functions properly if the user is on Internet Explorer. Add it to the **bottom of your** `<head>` **section before the closing** `</head>` **tag**.
```html
<!--[if lt IE 9]>
      <script src="https://oss.maxcdn.com/html5shiv/3.7.2/html5shiv.min.js"></script>
      <script src="https://oss.maxcdn.com/respond/1.4.2/respond.min.js"></script>
    <![endif]-->
```
**5. Set Up Your Container**
To make sure we're assigning the right styles to the right content, it's important to wrap content in containers. Web developers often use `<div>` tags to draw an imaginary box around a chunk of HTML. This defines a section of code separate from the rest of the code. Our first container is going to wrap up all the code in the body. So **right after your opening** `<body>` **tag**, paste the following code. Make sure **Everything** you add to the body after this point goes inside this tag!
```html
<div class="container">
  <!-- MAKE SURE EVERYTHING YOU WANT FOR YOUR BODY GOES INSIDE THIS TAG! -->
</div>
```
**6. Add in Cool Stuff: Navigation Bar**
Now comes the fun part. We'll start adding in different components to spruce up our website. Check out the Bootstrap documentation to see the variety of elements you can play around with. Basically all you need to do is copy the html code from the documentation and throw it into your project. The essence of Bootstrap is that Bootstrap has a bunch of class selectors that are added html elements that assign the pre-defined styles to that particular element.

Let's add a navigation bar first. A navigation bar is important to keep your users from getting lost on your site. Add this code as the first line under the `<div class="container">` tag, and don't forget to link to other pages on your site in each of the `<a>` tags.
```html
<div class="navbar navbar-default navbar-static-top" role="navigation">
    <div class="container">

        <div class="navbar-header">
            <button type="button" class="navbar-toggle" data-toggle="collapse" data-target=".navbar-collapse">
            <span class="sr-only">Toggle navigation</span>
            <span class="icon-bar"></span>
            <span class="icon-bar"></span>
            <span class="icon-bar"></span>
            </button>
            <a class="navbar-brand" href="index.html">Home</a>
        </div>

        <div class="navbar-collapse collapse">
            <ul class="nav navbar-nav">
                <li class="active">
                    <a href="#">Turtles</a>
                </li>
                <li>
                    <a href="#">Movie</a>
                </li>
                <li>
                    <a href="#">Legacy</a>
                </li>
            </ul>
        </div><!--/.nav-collapse -->

    </div>
</div>
```
**7. Add in Cool Stuff: A Heading**
Headings let a user know where they are. Let's add a heading underneath the navigation bar, like so:
```html
<div class="page-header">
    <h1>Steph's Sweet Teenage Mutant Ninja Fan Page</h1>
</div>
```
**8. Add in Cool Stuff: A Table**
Here's a standard table that has information about the different ninja turtles. The added Bootstrap classes give the table visual pizzazz.
```html
<table class='table table-hover table-responsive table-bordered'>
  <tr>
    <th>Turtle</th>
    <th>Color</th>
    <th>Personality</th>
  </tr>
  <tr>
    <td>Michelangelo</td>
    <td>Orange</td>
    <td>Best turtle. Comedian of the bunch.</td>
  </tr>
  <tr>
    <td>Leonardo</td>
    <td>Blue</td>
    <td>Courageous leader. Oldest child syndrome.</td>
  </tr>
  <tr>
    <td>Raphael</td>
    <td>Red</td>
    <td>The bad boy. Very New York attitude.</td>
  </tr>
  <tr>
    <td>Donatello</td>
    <td>Purple</td>
    <td>Techy and smart. Probs a good programmer.</td>
  </tr>
</table>
```
## Code Recap
You can see all the code for the site in the `index.html` file included in this repository. This is a very simple implementation of Bootstrap's features. Have fun exploring the different Bootstrap elements and incorporating them into your projects. Remember, the key to Bootstrapping your site is adding the Bootstrap classes to HTML tags that enclose your content.

## Resources
+ <a href="http://getbootstrap.com/">Twitter Bootstrap</a>: documentation
+ <a href="http://bootstrapbay.com/blog/bootstrap-3-carousel-tutorial/">Bootstrap Carousel Tutorial</a>

<p data-visibility='hidden'>View <a href='https://learn.co/lessons/hs-bootstrap-walkthrough' title='You Bet Your Bootstrap!'>You Bet Your Bootstrap!</a> on Learn.co and start learning to code for free.</p>
