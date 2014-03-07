---
layout: documentation
category: documentation
level: ninja
title: How the wiki works
---

This wiki is powered by Jekyll. Jekyll is a  ...


Thanks to Jekyll, pages are written using the Markdown syntax.

<div class="alert alert-info">
    <strong>Ninja Tip: </strong>
    The framework used for the theme is <strong>Bootstrap 3</strong>. So if want, you are free to use any features of Bootstrap, you can add them directly in your markdown file by using html syntax. But don't forget, between html tags, Markdown will not works.
</div>


In the root there are two main point to care of. The ```_config.yml``` file which describes the configuration of the wiki and the ```_posts``` folder where you find the markdown version of each webpages.

Here is the first annoying point of using jekyll, you have to respect a given format for the name of your page where you add the date of creation in the page name: ```yyyy-mm-dd-your-page-name.md``` for example ```2012-12-21-the-end-of-the-world-is-close.m``

<div class="alert alert-success">
    <strong>Kitty Tip: </strong>
    If you are using prose.io to create a page, this naming convention will be done automatically so you don't care about :)
</div>

```console
_posts
    |documentation
    |tutorial
media
_config.yml
```
