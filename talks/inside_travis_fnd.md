
> Note: Talk by Laura Gaetano ([@alicetragedy](https://twitter.com/alicetragedy)) 
> converted (by "hand") from PDF to Markdown. 
> Thanks Laura!


title: Inside Travis Foundation


# Contents

- Hello, I'm Laura.
- Travis Foundation Site
- Site Redesign
- What is jekyll?
  - Setup and Requirements
  - Liquid
- Using data files
- Themes
  - Using an existing theme
  - Creating your own theme
- The magic of Sass
  - Using variables for colours and breakpoints
  - Functions (use built-in functions or create your own)
  - Use inheritance to keep your code DRY
- Resources
  - Jekyll
  - CSS


# Hello, I'm Laura.

- Manager at Travis Foundation
- Organiser (vienna.rb, ROSSConf, RGSoC)
- Developer
- Artist

# Travis Foundation Site

[add screenshoot]

(Source: [foundation.travis-ci.org](http://foundation.travis-ci.org))


# Site Redesign

- Static pages and a blog
- Easy to use vs. lightweight
- Not too technical vs. allow for external contributions


# What is Jekyll?

- A static site generator
- Written in Ruby

<!-- break -->

- Lightweight
- Easily set up
- Customisable


# Setup and Requirements

- Ruby
- Ruby gems

<!-- break -->

- `gem install jekyll`
- `jekyll serve - -watch`


# Liquid

- templating engine created by Shopify

<!-- break -->

- filters and helpers out of the box
- Objects, variables, operators
- Control flow and iteration


# Using data files

```yaml
- 1:
  title: "Rails Girls Summer of Code"
  text: "Rails Girls Summer of Code funds women around the world to work full-time over summer on open-source software projects."
  image: "/images/rebrand/rgsoc.png"
  link: "/projects/rgsoc/"
- 2:
  title: "Diversity Tickets"
  text: "As part of our diversity consulting, we give conference organisers the possibility to provide underrepresented minorities in tech with free diversity tickets for their conference."
  image: 
  link: "/projects/diversity-tickets"
...
```

(Source: [_data/projects.yml](https://github.com/travis-ci/travis-foundation/blob/gh-pages/_data/projects.yml)


# Using data files

- supported data files: YAML, JSON, CSV
- add your data files to a `_data` folder
- data can be accessed using the `{{site.data}}` variable


# Themes

- Lots of free themes available
- Clone/Fork the theme repo and go


# Using an existing theme

- Themes are starting to be packaged as gems; easier setup
- Can get started right away
- Easy to play around with and build on top

<!-- break -->

- Sometimes difficult to customise to your needs
- Might have a lot of extra code/styling you don't need


# Creating your own theme

- Clean up/override all the Jekyll default theme styles
- Use a reset or normalize stylesheet
- Use Sass (it's built-in!)
- Create templates according to use cases
- Use partials where you can


# The magic of Sass

Using variables for colours and breakpoints

```sass
$bp-s: 460px
$bp-m: 800px
$bp-ml: 960px
$bp-l: $gridMaxWidth
```

(Source: [stylesheets/main.sass](https://github.com/travis-ci/travis-foundation/blob/gh-pages/stylesheets/main.sass)


# The magic of Sass

Functions (use built-in functions or create your own)

```sass
@function grid-calc($colNumber, $totalColumns)
  $result: percentage(($colNumber / $totalColumns))
  @if $result == 0%
    $result: 0
  @return $result
```

(Source: [stylesheets/main.sass](https://github.com/travis-ci/travis-foundation/blob/gh-pages/stylesheets/main.sass)


# The magic of Sass

Use inheritance to keep your code DRY

```sass
.icon-mail
  @extend %bg-icon
  width: .9em
  height: .9em
  background:
    image: url(/images/rebrand/email-icon.svg)
```

```sass
.icon-twitter
  @extend %bg-icon
  width: 1em
  height: 1em
  background:
    image: url(/images/rebrand/twitter-icon.svg)
```

(Source: [stylesheets/_footer.sass](https://github.com/travis-ci/travis-foundation/blob/gh-pages/stylesheets/_footer.sass)


# Resources: Jekyll

- Official Jekyll Site: [jekyllrb.com](https://jekyllrb.com)
- More about Liquid: [shopify.github.io/liquid](https://shopify.github.io/liquid/)
- Jekyll Themes: [jekyllthemes.org](http://jekyllthemes.org/)


# Resources: CSS

- Eric Meyer’s Reset CSS: [meyerweb.com/eric/tools/css/reset](http://meyerweb.com/eric/tools/css/reset/)
- Normalize.css: [necolas.github.io/normalize.css](https://necolas.github.io/normalize.css/)
- Sass Guide & Documentation: [sass-lang.com](http://sass-lang.com)


# Thank you!
