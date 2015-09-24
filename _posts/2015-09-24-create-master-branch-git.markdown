---
layout: post
title:  "How to create master branch based off gh-pages branch "
date:   2015-09-24
---
Recently I have cloned a Jekyll theme that only has the branch gh-pages. I have completely customized the theme by pushing all my changes to that gh-pages branch. And I wonder can I create a new master branch from that gh-pages branch, and here is the solutions for it.

<h4>To create a new local master branch based off the <em>local</em> gh-pages branch</h4>

{% highlight ruby %}
1. Open your command line and navigate to the repository that you want to create the branch
2. git checkout gh-pages     # switch to the gh-pages branch
3. git branch -d master      # delete current (old) local master branch
4. git checkout -b master    # create new master from gh-pages and switch to it
{% endhighlight %}

Keep in mind that the second command will delete your local master branch to make room for the new one you wish to create. So if you already have a local master branch you should make sure you really want to replace it. However, if you don't have  a local master branch like my case, you don't have to worry about it.

<h4>To create a new local master branch based off the <em>remote</em> gh-pages branch</h4>

{% highlight ruby %}
1. Open your command line and navigate to the repository that you want to create the branch
2. git checkout gh-pages                     # switch to the gh-pages branch
3. git branch -d master                      # delete current (old) local master branch
4. git checkout -b master origin/gh-pages    # create new master from gh-pages
{% endhighlight %}
