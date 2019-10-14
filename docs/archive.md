---
layout: default
title: Archive
---

# Navigating the archive

* [Latest blog post](index.md)
* [All content in one page](all.md)
* [Download for offline view][dl]

# Search

Press `f3` on desktop or tap `find in page` on mobile to search for keywords on any page listed above.

# About the content

The content on this archive is written by {{ site.author.name }} (<a href="{{ site.other.about }}">about me</a>) and its licensed under <a href="{{ site.other.licenselink }}">{{ site.licensename }}</a>.




# Posts in reverse chronological oder

{% for post in site.posts %}

<div>
  {{ post.date | date: "%b %-d, %Y" }}
    »
  <span class='post-title'>
    <a href="{{ site.path }}{{ post.url }}">{{ post.title }}</a>
  </span>
</div>

{% endfor %}

[dl]: https://github.com/alex-esc/posts/archive/master.zip