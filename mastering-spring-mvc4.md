---
layout: page
title: Mastering Spring MVC 4
permalink: /mastering/
---

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