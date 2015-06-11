# Introdution ot Boostrap

Bootstrap is one of the most popular frameworks for developing responsive websites. We will introduce Bootstrap this week so we can build [responsive](http://en.wikipedia.org/wiki/Responsive_web_design) sites. To be more specific, we will build our site again but this time using this framework focus on mobile first.

## Getting started

To get started, download the [zip file](https://github.com/twbs/bootstrap/releases/download/v3.3.4/bootstrap-3.3.4-dist.zip). This zip file has 3 folders: css, js, and fonts.

![Bootstrap folders](/images/bootstrap-folders.jpg)

Inside the css folder you will find six files, but we will only use `bootstrap.min.css`.

![Bootstrap minify css file](/images/bootstrap-min-css.jpg)

Inside the js folder you will find 3 files, but we will only use `bootstrap.min.js`.

![Bootstrap minify js file](/images/bootstrap-min-js.jpg)

For the fonts, we are not going to use them but if you wish to know more, visit this [page](http://getbootstrap.com/components/#glyphicons).

All you have to do is copy those files into your project's css and js folder.

![Project using bootstrap](/images/project-bootstrap.jpg)

## What we will cover in Bootstrap

Certainly there is a lot to talk about Bootstrap. It is a very extensive topic and I hope after this course you have the confidence to go back and learn the rest of the components Bootstrap has to offer. We will concentrate on learning the grid system, responsive utilities, and navigation. These three components will allow us to manipulate the elements on the website and target to different screen sizes. Bootstrap also changes the apperance of the rest of the HTML elements (e.g. h1, ul, button, etc) but we can gain the control by using a custom css file and adjusting things to our needs.

### Grid system

Bootstrap includes a responsive, mobile first fluid grid system that appropriately scales up to 12 columns according to the screen size. Grid systems are used for creating page layouts through a series of rows and columns that holds the content.

We will be making two distinctions: phone(sx) and everything above that such as tablet(sm), laptop(md) and desktops(lg). Now since we have 12 columns in our grid, we can make several combinations that add up to 12, for example:

```html
<!-- It's important to have a column combination encapsulated within a row to perform well -->
<!-- This will result in 3 columns. First one is 4 column, second 2 column, and third 6 column wide -->
<!-- The total of these columns adds up to 12 -->
<div class="row">
    <div class="col-sm-4">
        Content goes here
    </div>
    <div class="col-sm-2">
        Content goes here
    </div>
    <div class="col-sm-6">
        Content goes here
    </div>
</div>
```

When you define a container element like a `div` with a class attribute `col-sm-4` as an example, what it means is that it will have 4 columns wide from small, medium, and large screen sizes even if the last two were not determined and for an extra small screen there will be 12 columns wide or full width. By determining the number of columns for a specific screen size, screen sizes larger than that will inherit that number of columns and screen sizes smaller than that will be default to the 12 column width.

Dont worry if this is too complex just by reading it because there will be plenty of excersises during class.


If you wish to learn more, you can go and read the documentation [here](http://getbootstrap.com/css/#grid) and bring your questions to class.