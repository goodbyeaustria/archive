---
layout:     default
permalink:  /index.html     # note: should be add by jekyll-readme-index plugin (not working for now?)
---


# [Vienna.html](http://austriacodes.github.io/vienna.html)

**Website Builder & Designer Meetup in Austria, Vienna • Wien • Vídeň • Beč**

{% include members.html %}


Static is the New Dynamic // Jekyll • Middleman • Hugo • Metalsmith • Gatsby & Friends // Join Us (Free) // No Database Required // We ♥ HTML & CSS.


<!--
We're back! Join us.
-->

Happy New Year. Prosit 2018!



Free. Everyone Welcome.





### Join us

[Add yourself to the Vienna.html Members Directory](signup.md) - free; no database required - just some YAML ;-)

<!--
[Add Members Here]
  -->





### Past meetups

**2016**

#### \#6 - Tuesday, November 22nd

- **Markdown in Action: Building Courses (incl. Presentations, Pages, Handouts) for the Web and Print (PDF) w/ kramdown (webgen+Prawn)**  [(Sample Course)](http://www.mat.univie.ac.at/~praxis/sosem16/vorlesung.html) by [Thomas Leitner](speakers#thomas.leitner)
    - Summary: How do you create presentation slides for a course and provide the information in various formats? The most obvious way would probably
      be to use a tool like Microsoft PowerPoint or LibreOffice Impress which can export the slides as handouts. However, this is a manual process
      where some steps can be forgotten. And the whole thing is not really web friendly.

      There are other ways if you are a hacker and tinkerer. We like to
      automate things. By using Markdown as the source format

      * we can easily produce HTML slides using one of the various
        Javascript presentation solutions,
      * provide the contents as a normal HTML pages for easy searching
        and online viewing, and
      * provide a print friendly output format, in this case PDF.

      In this talk Thomas will show you how to combine the static website
      generator webgen, the Markdown library kramdown and the PDF generation
      library Prawn to do these things.
    - Bio: {{ site.data.speakers[ 'thomas.leitner' ].bio }}

- **Jekyll in Action Case Study - Inside Travis Foundation** [(Site Source)](https://github.com/travis-ci/travis-foundation) by [Laura Gaetano](speakers#laura.gaetano) [(Travis Foundation)](http://foundation.travis-ci.org)
  - Covers how to use datafiles (in YAML) e.g. [projects.yml](https://github.com/travis-ci/travis-foundation/blob/gh-pages/_data/projects.yml), how to customize your website theme and more.
  - Bio: {{ site.data.speakers[ 'laura.gaetano' ].bio }}

- **Jekyll in Action Case Study - Inside PunkRockDev.com** [(Site Source)](https://github.com/punkrockdev/punkrockdev.github.io) by [Dražen Lučanin](speakers#drazen.lucanin)
  - Summary: Notes on Dražen's web development portfolio website - PunkrockDev.com - e.g. tios on how to use gulp for image optimization; cloudshare for HTTPs (for custom domains on GitHub Pages) and Google AdWords tweaks to get traffic and more.
  - Bio: {{ site.data.speakers[ 'drazen.lucanin' ].bio }}


#### \#5 - Wednesday, October 19th

- **Getting Started w/ Jekyll ('n' GitHub Pages) - Hello, Jekyll! 'n' Hello, Minima!** by [Gerald Bauer](speakers#gerald.bauer)

#### \#4 - Tuesday, June 28th

- **Using PostCSS with Static Site Builders** by [Max Stoiber](speakers#max.stoiber)
  - Bio: {{ site.data.speakers[ 'max.stoiber' ].bio }}
- **Real World Static Site Showcase I - Inside ColorSnapper - Changelog Generation w/ Metalsmith.js and a Custom Plugin** by [Andrey Okonetchnikov](speakers#andrey.okonetchnikov)
  - Summary: An insight look about a hand-crafted Metalsmith plugin, that is, [`metalsmith-remote-json-to-files`](https://github.com/okonet/metalsmith-remote-json-to-files ) that lets you fetch JSON from remote URLs, transform and inject as files into the metalsmith pipeline and how it gets used to automate the [changelog](http://colorsnapper.com/changelog) generation for the [ColorSnapper](http://colorsnapper.com) site.
  - Bio: {{ site.data.speakers[ 'andrey.okonetchnikov' ].bio }}
- **Real World Static Site Showcase II - Inside Contentful - Turn Your Blog Posts into Facebook Instant Articles w/ Middleman** by [Rouven Weßling](speakers#rouven.wessling) [(Contentful)](https://contentful.com)
  - Summary: [Facebook Instant Articles](https://instantarticles.fb.com) is a new way for any publisher - including you ;-) - to create fast, interactive articles on (mobile) Facebook.  Rouven will show how you can prepare and auto-build Facebook Instant Articles web feeds (in RSS) from your blog stories (in Markdown) with  the Middleman static site builder as [working live on the Contentful blog](https://www.contentful.com/blog/2016/05/13/facebook-instant-articles-and-contentful). Rouven will discuss alternative strategies and go through some of the possibilities and limitations of Facebook Instant Articles. PS: Rouven will start off with a short intro about [what's Contentful anyways?](https://contentful.com) And how you can use the Contentful service to manage your (static site) content.
  - Bio: {{ site.data.speakers[ 'rouven.wessling' ].bio }}
- **Real World Static Site Showcase III - Inside Chip Shop - Build Your Silicon Empire - Build A Cards Game w/ Jekyll (n Markdown)** by [Chris Ward](speakers#chris.ward)
  - Summary: An insight look on how to build a [print-at-home Chip Shop (offline) board game](http://www.chrischinchilla.com/print-at-home-chip-shop-released) with printed paper cards (72 products, 76 events and 36 personalities) that let you run a computer company in the 80's to build your silicon empire. Learn how to turn [cards in markdown files](https://github.com/GregariousMammal/Chip-Shop) as used on the game website into [high-quality printable PDFs](http://www.chrischinchilla.com/creating-a-game-with-markdown-pandoc-latex-and-pdfjam) for a premium pre-boxed or print-yourself card deck version and much more.
  - Bio: {{ site.data.speakers[ 'chris.ward' ].bio }}
- **Why you would (not) want to build your own static site generator** by [Matthias Beitl](speakers#matthias.beitl)
  - Summary: It's a brave new world of static site generators out there. So why would you write your own when [this is your competition](http://www.staticgen.com)? We'll look into the pros and cons. And pitfalls.
  - Bio: {{ site.data.speakers[ 'matthias.beitl' ].bio }}

#### \#3 - Tuesday, April 26th

- **Static site generating for podcasting with Octopress** by [Stefan Haslinger](speakers#stefan.haslinger), [Aua-Uff-Code Podcast](https://aua-uff-co.de) [(Site Source)](https://github.com/aua-uff-code/aua-uff-co.de)
   - Summary: An overview of the current state of podcast publishing (problems, challenges, requirements) and how some of the issues can be resolved by Octopod, a static site generator (based on Jekyll and parts of Octopress) dedicated to podcasting. Stefan will go into details of secure and quick publishing (static, https, rsync) and show off some nice features of Octopod (Twitter, Disqus, Flattr + Podlove Webplayer integrations) in a live demo. Furthermore  will encourage you getting started with podcasting via a minimal setup and introduce you to the Viennese podcasting community (Podcasting meetup, Biertaucher podcast).
   - Bio: {{ site.data.speakers[ 'stefan.haslinger' ].bio }}
- **Real World Static Site Show Case - [Tierarztpraxis Kaisterstrasse](http://tierarztpraxis-kaiserstrasse.at)** [(Site Source)](https://github.com/richardtraindl/tierarztpraxis-kaiserstrasse.at) by [Richard Traindl](speakers#richard.traindl)
  - Summary: A insight look at a small business website for a veterinary practice in Vienna built using the Jekyll static site builder; uses a JavaScript picture gallery and includes some breakpoints for a (simple) hand-coded responsive (mobile) design.  
  - Bio: {{ site.data.speakers[ 'richard.traindl' ].bio }}


#### \#2 - Tuesday, February 23rd

- **Building Page Layouts with Susy Grid** by [Bernhard Benke](speakers#bernhard.benke)
    - Bio: {{ site.data.speakers[ 'bernhard.benke' ].bio }}
- **Using Markdown (HTML "Shortcodes" in Plain Vanilla Text) with the kramdown Library and Tools** by [Thomas Leitner](speakers#thomas.leitner)
    - Bio: {{ site.data.speakers[ 'thomas.leitner' ].bio }}
- **Building Books with Gutenberg - a Web Typography Starter Kit - and Jekyll - a Static Site Builder** by [Gerald Bauer](speakers#gerald.bauer)
    - Bio: {{ site.data.speakers[ 'gerald.bauer' ].bio }}


**2015**

#### \#1 - Tuesday, November 24th

- **Static Site Builders of the Year 2015 Awards** by [Gerald Bauer](speakers#gerald.bauer)
    - Middleman or Jekyll? Metallsmith or Wintersmith? Pelican or Nikola? Emacs or Vim? Let's look at the world's greatest (free) static site builders.   
- **CSS Pub Quiz** by [Floor Drees](speakers#floor.drees)
    - Test your styling sense. Fun guaranteed ;-)   
      Bio: {{ site.data.speakers[ 'floor.drees' ].bio }}
- **XSL/T - Generating Static Sites Like It's 1999** by [Sebastian Gräßl](speakers#sebastian.graessl)
    - Bio: {{ site.data.speakers[ 'sebastian.graessl' ].bio }}




### More Groups

See the Awesome Austria page for more.
