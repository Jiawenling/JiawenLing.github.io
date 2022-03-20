---
layout: post
title: First Post - Using Jekyll
---

#Setting up Jekyll - using theme Hyde

First post should be dedicated to the setup of this static webpage - can't use it straight off the bat, unfortunately. Zero knowledge on Ruby, but thankfully plenty of tutorials out there.
Initial steps can be found [here](https://idratherbewriting.com/documentation-theme-jekyll/mydoc_publishing_github_pages.html) (thanks lots!)

If you chose Hyde, there are a few modifications to be made:

1. In config.yaml:
* Delete *relative permalinks*
* Insert the following:
  {% highlight js %}
  plugins:
  - jekyll-paginate
  - jekyll-gist
  {% endhighlight %}

2. Bundle init
3. Add the following to your Gemfile (which should be in your project folder):
   {% highlight js %}
   gem "jekyll"
   gem "jekyll-paginate"
   gem "jekyll-gist"
   gem "jekyll-sitemap"
   gem "jekyll-seo-tag"
   gem "webrick"
   gem "github-pages"
  {% endhighlight %}
4. bundle install
5. bundle exec jekyll serve
