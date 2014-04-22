# Project Hub template for [Jekyll](https://github.com/jekyll/jekyll)

Author: Julie Ng ([@jng5](http://twitter.com/jng5))  
Date: April 2014  
Version: 0.1.0  

In December 2013, [Brad Frost](http://bradfrostweb.com/) introduced Project hubs as a way to consolidate design and development materials for client projects on [24ways.org](http://24ways.org/2013/project-hubs/).

I adopted project hubs as a semi-interactive project log for my client projects. Because I update these reports regularly, I wanted to automate my workflow with a static site generator.

## Installation

  1. Install jekyll on your machine with `gem install jekyll`
  2. Clone this repository with `git clone https://github.com/jng5/jekyll-hub-template`
  3. `cd` into created directory and run `jekyll serve --watch`
  4. Start sass to compile css `sass --watch css/styles.scss:css/styles.css`
  5. To build, run `jekyll build`


## Structure / Configuration

#### Site

`_config.yml`

  * Site name
  * Site description

#### Layout

  * `layouts/default.html` - basic page markup
  * `index.html` - project entries markup

#### Stylesheets

To customize your design:

  * `css/layout.scss` - generic site layout
  * `css/base.scss` - typgraphy, colors
  * `css/hub.scss` - basic design of entries, etc. based on [Dan Mall's Project hub template](https://github.com/danielmall/project-hub).


You should not need to touch the following files:

  * `css/styles.css` - the generated  is the only file included by the site.
  * `css/styles.scss` - source file that only imports other CSS files.
  * `css/normalize.css` - normalize.css reset

## Future entries

To mark a post as a future, i.e. *not-yet-completed* phase, include the `future` property in the entries frontmatter:

    ---
    title: Development
    date: 2014-03-01
    future: true
    ---

## Demo

<img src="https://jng5.github.io/jekyll-hub-template/images/template-large.png" alt="Template preview: desktop" style="height:200px;">

Project demo: 
[http://jng5.github.io/jekyll-hub-template/](http://jng5.github.io/jekyll-hub-template/)


## Misc.

### Why another project hub project?

Instead of static front-end templates, I wanted:

  * automate project entries, without editing markup.
  * integrate automatic update of website using static site generator
  * strip down design and markup to allow for easy customization, based on client, agency, etc.
  * share CSS source with others

### Why Jekyll?

I chose [Jekyll](https://github.com/jekyll/jekyll) instead of my usual [Middleman](http://middlemanapp.com) to keep this as simple as possible. Jekyll automatically handles future posts without having to toggle drafts, etc.

## Credits

  * Included [normalize.css](https://github.com/necolas/normalize.css) is a project by [Nicolas Gallagher](http://nicolasgallagher.com/)
  * Based on [Project Hub template](https://github.com/danielmall/project-hub) by [Dan Mall](http://danielmall.com/)


## License

Copyright (c) 2014 [Julie Ng](http://julie.io/)

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
