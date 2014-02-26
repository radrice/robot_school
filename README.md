# Welcome to ROBOT SCHOOL
Robot school is a generic rails app intended for front end caveman learning.

## Front end features
The greatest of the front end frontier reside here.
### Sass project structure
The structure of the `assets/stylesheets` folder borrows heavily from [The Sass Way](thesassway.com/beginner/how-to-structure-a-sass-project) and Github's [CSS Styleguide](https://github.com/styleguide/css). Robot School's hierarchy follows a similar pattern:

    Stylesheets
      - Globals : anything original and pure sass (vars/mixins)
      - Partials : anything else, up to you how it's structured
      - Vendor : 3rd party stuffs
      application.css.scss : the manifest for everything

### Ham-fisted implementations of Sass(SCSS) libraries
Within `app/assets/stylesheets` is a proprietary `vendor` directory. This directory features some of the universe's favorite UI frameworks, not as gems, but as mooshy, flexible SCSS manifests. __Why?__ This way you can pick and choose, mix and match library components. Edit variables, fuck up mixins, the front end framework is your hackable oyster.

Pick any library you want by commenting in/out its manifest under the  `// Vendor` sub heading in `application.css.scss`.

#### Bootstrap (SCSS)
Appropriated from the ["Official Sass port of Bootstrap"](https://github.com/twbs/bootstrap-sass), this ported library lives in the `bootstrap` directory within `stylesheets/vendor`. Pick and choose your favorite parts within the `bootstrap.scss` manifest.

Be warned, its dependent fonts are locateds in `assets/fonts`. Hackery!

#### Foundation (SCSS)
Ripped directly from ZURB's [Foundation Repo](https://github.com/zurb/foundation), the `foundation` directory within `stylesheets/vendor` has an SCSS manifest that references all components of the framework. Comment out what you don't want to use.
