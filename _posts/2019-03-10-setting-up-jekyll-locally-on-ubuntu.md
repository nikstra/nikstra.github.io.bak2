---
layout: post
title:  "Setting up Jekyll locally on Ubuntu"
date:   2019-03-10 19:43:52 +0100
categories: jekyll ubuntu
---
First note, how I actually got started with this site locally on my Linux Mint 18.3 installation. Following the [Setting up your GitHub Pages site locally with Jekyll][gh-pages-locally] guide I got stuck at [Step 3 (optional): Generate Jekyll site files][generate-jekyll-site]. It says to run:
{% highlight shell %}
$ bundle exec jekyll _3.3.0_ new NEW-JEKYLL-SITE-REPOSITORY-NAME
> New jekyll site installed in /Users/octocat/NEW-JEKYLL-SITE-REPOSITORY-NAME.
{% endhighlight %}
However, this resulted in "Could not locate Gemfile or .bundle/ directory". I found suggestions that "ruby-all-dev" needed to be installed on Ubuntu but it was already installed. After some trial and error I found that leaving out "bundle exec" from the command line made it work. Just running:
{% highlight shell %}
$ jekyll new nikstra.github.io
{% endhighlight %}
successfully created the site.

[gh-pages-locally]: https://help.github.com/en/articles/using-jekyll-as-a-static-site-generator-with-github-pages
[generate-jekyll-site]: https://help.github.com/en/articles/setting-up-your-github-pages-site-locally-with-jekyll#step-3-optional-generate-jekyll-site-files

