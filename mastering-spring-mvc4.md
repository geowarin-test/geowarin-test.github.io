---
layout: page
title: Mastering Spring MVC 4
icon: book
---

<a href="https://www.packtpub.com/application-development/mastering-spring-mvc-4">
    <amp-img class="right" src="/assets/images/book/thumb.jpg" layout="fixed" width="130px" height="160px" />
</a>
  
Hello, dear visitor. I know why you're here!

You want to learn how to create a complete Spring web application with
oauth support, security, file upload and distributed sessions.

You want to master the principles of REST and develop a clean API with top-notch
exception handling and following the best practices.

You also want to deploy it in the cloud and for it to be fully tested with
both unit and end-to-end tests.

What a coincidence! I just wrote the book
[you are looking for](https://www.packtpub.com/application-development/mastering-spring-mvc-4)!

If you want to have a look at what you will be building,
its source code is available [on github](https://github.com/Mastering-Spring-MVC-4)
and it is deployed [on heroku](http://masterspringmvc.herokuapp.com/)

{% for post in site.categories['Master Spring MVC 4'] reversed %}
<article class="post" itemscope itemtype="http://schema.org/BlogPosting" role="article">
    <div class="article-item">
        <header class="post-header">
            <h2 class="post-title" itemprop="name"><a href="{{ site.baseurl }}{{ post.url }}" itemprop="url">{{ post.title }}</a></h2>
        </header>
        <section class="post-excerpt" itemprop="description">
            <p>{{ post.excerpt | strip_html | truncatewords: 50 }}</p>
        </section>
        <div class="post-meta">
            <time datetime="{{ post.date | date_to_long_string }}">{{ post.date | date_to_long_string }}</time>
        </div>
    </div>
</article>
{% endfor %}