# Jekyll-Pages README

Put your doc somewhere under docs directory and it will be converted to HTML!
This is a Jekyll-based package similar to Github pages.

Acceptable input formats:

* markdown
* asciidoc

More information:

* Jekyll [variables](https://jekyllrb.com/docs/variables/)
* [Blogging primer](https://www.smashingmagazine.com/2014/08/build-blog-jekyll-github-pages/).
* [just-the-docs theme](https://just-the-docs.github.io/just-the-docs/)
* [Front matter](https://jekyllrb.com/docs/front-matter/)


## Installation

### Install rbenv

Having rbenv is NOT required but proved useful and therefore recommended.

Install [rbenv](https://github.com/rbenv/rbenv).  Then, if `rbenv install -l`
does not show the latest ruby versions this means your rbenv distribution is
obsolete,  as it was for me on Linux.  In such case
[install rbenv from github](https://github.com/rbenv/ruby-build).

Finally, add to your .zshrc:

```sh
#
# load rbenv
#
eval "$(rbenv init -)"
```

### Install ruby

```sh
$ rbenv install 3.1.1
$ rbenv global 3.1.1
$ rbenv versions
  system
* 3.1.1 (set by ~/.rbenv/version)
$ which ruby
~/.rbenv/shims/ruby
```

Then `gem install bundler`.

Then `bundle install`.

## Develop Content

1. Build the site and serve it locally: `bundle exec jekyll serve`
2. Follow instructions and point your browser at http://127.0.0.1:4000/
3. Learn how to publish to this site: http://127.0.0.1:4000/about

## Publish the Site

Build the site with `jekyll build --config _config.yml`.
This creates content in directory `_site`.

Copy contents of `_site` to your favorite hosting provider.
