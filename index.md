---
title: Hello GitHub Pages!
---

Why must I have the title in front matter?!

This is index.md. This is my first GitHub Pages page. This is actually a README markdown file. Markdown makes it really *simple* and __clean__ to write documents without any special software or lengthy syntax. Just get it done!

Here is [link to the about page](about.md).

Here's some [markdown tutorial stuff](markdown.md).

Jekyll version
{{ site.github.versions.jekyll }}

## List of public repos

{% for repository in site.github.public_repositories %}
  * [{{ repository.name }}]({{ repository.html_url }})
{% endfor %}

## List of all posts

{% for post in site.posts %}
  * [{{ post.title }}]({{ post.url }})
{% endfor %}
