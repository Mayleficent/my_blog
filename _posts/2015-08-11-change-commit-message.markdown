---
layout: post
title:  "How to edit recent commit message before pushing to github"
date:   2015-08-11
---
You can change the most recent commit message using the <code>git commit --amend </code> command.

{% highlight ruby %}
1. Open your command line and navigate to the repository that you want to change the commit message
2. type git commit --amend -m "New commit message"
3. type git status to see whether your commit message is changed or not
{% endhighlight %}
