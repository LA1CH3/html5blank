# RPM Starter Theme

## Forked from [HTML5 Blank](http://html5blank.com)

This is a basic starter theme for Wordpress themes that will get you developing ASAP. Includes almost all your standard page templates and a fully loaded functions.php file, as well as Sass integration with Bourbon (mixin library), Bitters (CSS scaffolding) and Neat (Bourbon semantic grid system). Additionally you get to use Bower for front-end package management, as well as Gulp for build. This theme also includes: jQuery, Modernizr, Normalize.css, and Conditionizr. 

* Go to the Wordpress' theme folder (`.../wp-content/themes`)
* In CLI, run: `git clone https://github.com/LA1CH3/html5blank.git`
* `cd html5blank` and then run the following commands:
    - `npm install` (you need node/npm globally installed)
    - `bower install` (you need bower globally installed)
    - `bundle install` (you need ruby bundler for this)
    - `npm install --save-dev gulp` (if you dont have Gulp installed, you will need `npm install --global gulp` before this)
    - `cd src/css/sass/` and then run:
        + `bitters install`
        + `bourbon install`
        + `neat install`

**When using Neat:**
Uncomment the following line in _base.scss in sass/base:
`@import "grid-settings";`
You also need to change the import for neat-helpers inside _grid-settings.scss to "../neat/neat-helpers".

If you're unfamiliar, Gulp is used as our build tool, which will handle Sass compilation and concatenation, JSHint, minification, livereload for rapid development, and much more. 

* `gulp watch` will enable `livereload` and development version
* `gulp build` for distribute version with minified `js` and `css` files
* NOTE: `src` and `dist` folders can live happily together inside the same folder (`html5blank`) that in the `theme` folder. You'll have two different instances of the theme within `Appearance > Themes` panel inside the admin

This is a fork of html5blank, with the additions of a Gemfile that includes Bourbon, Bitters and Neat for more powerful CSS development. My hope is that this will provide a strong template for RPM theme development projects, allowing for a quick way to have a theme template up and ready for development.


