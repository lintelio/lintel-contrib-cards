lintel-contrib-cards
====================

> Cards for lintel.

[![npm](https://img.shields.io/npm/v/lintel-contrib-cards.svg)](https://www.npmjs.com/package/lintel-contrib-cards)
[![Bower](https://img.shields.io/bower/v/lintel-contrib-cards.svg)](https://github.com/lintelio/lintel-contrib-cards)


## Getting Started
This module requires Lintel.

If you haven't used [Lintel](http://lintel.io/) before, be sure to check out the [Getting Started](http://lintel.io/getting-started) guide, as it explains how to install and use this module. Once you're familiar with that process, you may install this module with this command:

```shell
bower install lintel-contrib-cards --save
```

Once the module has been installed, you will have to load it in your main SASS file:

```scss
@import "bower_components/lintel-contrib-cards/sass/cards.scss"
```

You can use [wiredep](https://github.com/taptapship/wiredep) or [grunt-wiredep](https://github.com/stephenplusplus/grunt-wiredep) to automatically inject files in your build process.


## Variables
Check the vars file in the `sass` folder to see the full list of variables you can customize.

#### $card-padding-y
Default value: `$cushion-y-md`  

Change the default padding-top and padding-bottom.

#### $card-padding-x
Default value: `$cushion-x-md`  

Change the default padding-left and padding-right.

#### $card-header-padding-y, $card-body-padding-y, $card-footer-padding-y
Default value: `$card-padding-y`  

Change padding-top and padding-bottom for a specific part.

#### $card-header-padding-x, $card-bodx-padding-x, $card-footer-padding-x
Default value: `$card-padding-x`  

Change padding-left and padding-right for a specific part.

#### $card-bg
Default value: `#fff`  

Card background.

#### $card-border
Default value: `$border-base`  

Header and footer border.

#### $card-border-dark
Default value: `$border-dark`  

Card border.

#### $card-border-radius
Default value: `$border-radius-small`  

Card border-radius.

#### $card-header-text
Default value: `$text-base`  

Header text color.


## Examples

#### Base Card
```html
<div class="card">
  <div class="card-header">
    <h1 class="card-heading text-h5">
      Title
    </h1>
  </div>
  <div class="card-body">
    Body
  </div>
  <div class="card-footer">
    Footer
  </div>
</div>
```

#### Linked Title
```html
<h1 class="card-heading text-h5">
  <a href="#">Link Title</a>
  <small>Subtitle</small>
</h1>
```

#### Header Actions
Note: make sure there are no spaces between the actions and `.card-heading` otherwise there will be a bit of space before the card title. See how to [remove the space between inline-block elements](http://css-tricks.com/fighting-the-space-between-inline-block-elements/).

```html
<div class="card-header">
  <div class="card-header-actions">
    <div class="btn-group">
      <button class="btn" type="button">
        Cancel
      </button>
      <button class="btn btn-primary" type="button">
        Save
      </button>
    </div>
  </div><!--
  --><h1 class="card-heading text-h5">
    Card Title
  </h1>
</div>
```

#### Footer Actions
Note: make sure there are no spaces between the actions any optional text on the left. See how to [remove the space between inline-block elements](http://css-tricks.com/fighting-the-space-between-inline-block-elements/).

```html
<div class="card-footer">
  <div class="card-footer-actions">
    <div class="btn-group">
      <button class="btn" type="button">
        Cancel
      </button>
      <button class="btn btn-primary" type="button">
        Save
      </button>
    </div>
  </div><!--
  --><span class="text-muted">Last Saved: Right Now</span>
</div>
```


## Contributing
In lieu of a formal styleguide, take care to maintain the existing coding style. Add unit tests for any new or changed functionality. Lint and test your code using [Grunt](http://gruntjs.com/).


## License
Copyright (c) 2015 Marius Craciunoiu. Licensed under the MIT license.
