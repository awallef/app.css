# app.css

app.css is a compass-based, BEM, OOCSS framework using parts of inuit.css

It is a [Compass](http://www.compass-style.org) based, Object Oriented framework that is full of objects and
abstractions.

app.css is built on a [BEM](http://bem.info/)-style naming convention and
honed based on [work done by Nicolas Gallagher](https://gist.github.com/1309546).

app.css use only little parts of [inuit.css](https://www.github.com/csswizardry/inuit.css)
such as mixins, helpers, headings and smallprint.  Thanks to Harry Roberts for his nice work!

## Requires
- ruby and [Compass](http://www.compass-style.org) see install page

## Install
The command line install of app.css is _incredibly_ simple:

    $ git clone --recursive git@github.com:awallef/app.css.git your-project-folder/your-css-folder/app.css
    $ cd your-project-folder/your-css-folder/app.css
    $ ./watch

when you need you are happy with your css then run:
  
    $ ./minimify

## folder structure

    your-project-folder/
        your-css-folder/
            app.css/
                core/
                default.scss
                themes/
                    default/
                        folders-you-like/
                        _inc.scss
            default.css
    index.html

## usage
The main concept is to design as many theme you need.
Whene you create a theme.scss file inside app.css folder, then create a new folder
inside themes with the same name as your new theme. Compass will generate a new css
file theme.css inside your css folder. So all the code stays in app.css folder and only
the result will be generated for use in your html files.

## About BEM
I suggest you to follow the following name convention:
    
    .block{}
    .block__element{}
    .block--modifier{}
    
    .person{}
    .person__hand{}
    .person--female{}
    .person--female__hand{}
    .person__hand--left{}

## Inuit.css the basics
more ( or less :) docs here: [inuit.css](https://www.github.com/csswizardry/inuit.css)

### helpers you may want use:
    
    Add/remove floats
    .float--right 
    .float--left
    .float--none
    
    Text alignment
    .text--left
    .text--center
    .text--right

    Font weights
    .weight--light
    .weight--normal
    .weight--semibold
    
    Add/remove margins
    .push
    .push--top
    .push--right
    .push--bottom
    .push--left
    .push--ends
    .push--sides
    
    .push-half
    .push-half--top
    .push-half--right
    .push-half--bottom
    .push-half--left
    .push-half--ends
    .push-half--sides

    .flush
    .flush--top
    .flush--right
    .flush--bottom
    .flush--left
    .flush--ends
    .flush--sides
    
    more on inuit.css...
    
### Cool mixins

    font-size($font-size, $line-height:true)
    
    headings($from: 1, $to: 6)
    
    vendor($property, $value...)
    
    truncate($truncation-boundary)
    
    arrow($arrow-edge, $arrow-location, $arrow-color, $border-color: $arrow-color)
    ( my favorite :) This mixin creates a CSS arrow on a given element
    
    ...
    
## License

Copyright 2013 Wallef Antoine

Licensed under the Apache License, Version 2.0.

---

** Hura **   
    
